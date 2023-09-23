#chaîne_d_action_chaine_d_energie
Les convertisseurs statiques, composés de composants électriques de puissance, permettent l'échange d'énergie entre au moins deux systèmes électriques en assurant :
- Une fonction de conversion de l'énergie électrique en rendant compatible les caractéristiques (tension, courant et fréquence) de ces deux systèmes. 
- Une fonction de contrôle de cet échange d'énergie. 

## Structure générales des convertisseurs statiques 
Un convertisseur statique est constitué d'interrupteurs qui vont interconnecter périodiquement une source d'entrée et une de sortie.   
### Règles d'association des sources
#### Configurations interdites 
![[image associations interdites.png]]
#### Configurations autorisées 
![[image associations autorisees.png]]
### Cellule de commutation
Structure à deux interrupteurs. Lorsque les sources d'entrée / sortie sont de diffèrent nature, les règles précèdent nous force à utiliser deux interrupteurs.
### Interrupteurs 
![[image interrupteurs.png|300]]
#### Régime statique et nombre de segments 
Caractéristique statique : composée des segments sur lesquels son point de fonctionnement $(v_{k}, i_{k})$ peut se déplacer.
![[image regime statique.png|300]]
#### Régime dynamique
Caractéristique dynamique : Trajectoire suivie par le point de fonctionnement pour passer d'un point situé sur un segment à un point situé sur un autre segment. 
![[image regime dynamique.png|300]]

## Composants semi-conducteurs utilisées 
#### La diode
Amorçage et blocage spontanées.
 ![[image diode.png|500]]
 #### Le transistor MOS
 ![[image transistor MOS.png|550]]
 Commandé en tension par $v_{GS}$ : 
 - $v_{GS}>0$, état passant, $v_{DS}=0$, $i_{DS}>0$ 
 - $v_{GS}=0$, état ouverte, $v_{DS}>0$ et $i_{DS}=0$ 
#### Le transistor IGBT 
![[image transistor IGBT.png|550]]
Commandé en tension par $v_{GE}$ :
- $v_{GE}>0$, état passant, $v_{CE}=0$ et $i_{C}>0$ 
- $v_{GE} \leq 0$, état ouverte, $v_{CE}>0$ et $i_{C}=0$
#### Association transistor plus diode antiparallèle 
![[image transistor plus diode.png]]
