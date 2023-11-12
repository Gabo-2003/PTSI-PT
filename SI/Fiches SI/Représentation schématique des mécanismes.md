#representation_et_schematisation 
 ### Mécanisme
 Ensemble des pièces mécaniques reliées entre elles par des liaisons, en vue de réaliser une fonction déterminée. 
 ### Solide indéformable 
 Solide où quels que soient les points $A$ et $B$ de $(S)$, la distance $AB$ reste constante au court du temps $t$. 

## Paramétrage de la position d'un solide par rapport à un repère 
### Nombre de paramètres indépendante 
- Si on donne la position de $3$ points du solide sa position est parfaitement déterminée.
- On a donc $9$ paramètres qui sont dépendantes avec $\begin{align*} \| \overrightarrow{O_{1}O_{2}} \| &= cste \\ \| \overrightarrow{O_{1}O_{3}} \| &= cste \\ \| \overrightarrow{O_{2}O_{3}} \| &= cste \end{align*}$   car le solide est indéformable.
- Le nombre de paramètres indépendantes est le nombre de paramètres moins le nombre de relations de dépendance.  
- Donc $9-3=6$ paramètres indépendantes.
### Paramétrage
Pour définir la position de $(S)$ par rapport à $R(O,\overrightarrow{x_{0}}, \overrightarrow{y_{0}},\overrightarrow{z_{0}})$ il faut lier $(S)$ à $R_{1}(O_{1},\overrightarrow{x_{1}}, \overrightarrow{y_{1}},\overrightarrow{z_{1}})$ et ensuite, définir la position de $R_{1}$ par rapport à $R$. 
- Il faut 3 paramètres pour positionner l'origine et 3 paramètres pour l'orienter. 

## Modélisation des liaisons 
### Degrés de liberté
Nombre de mouvements indépendantes de translation et de rotation suivant $(0,\overrightarrow{x}), (0,\overrightarrow{y}), (0,\overrightarrow{z})$ que la liaison autorise. 
### Modèles de liaison
#### Il faut définir pour tout liaison :
- La définition
- Le repère local
- Les mouvement relatifs que la liaison autorise
- Les schématisations planes et / ou spatiales normalisés. 

|          | Plan                | Cylindrique        | Sphère |
| -------- | ------------------- | ------------------ | ------ |
| Sphère   | Ponctuelle          | linéaire annulaire | rotule |
| Cylindre | linéaire rectiligne | Pivot glissant     |        |
| Plan     | Appui plan          |                    |        |
![[Pasted image 20230813135633.png|300]]
- Deux contact plan : Glissière 
- Contact cylindre / cylindre + plan / plan : pivot  
 ![[image model liaison 2.png|200]]
 ![[image liaisons.png]]
## Schéma cinématique 
- Regrouper les pièces opérant le même mouvement.
- Définir les liaisons entre ces ensembles.
- Produire le graphe des liaisons en précisant les points et axe caractéristiques. 
- Reproduire par un schéma cinématique ce graphe. 