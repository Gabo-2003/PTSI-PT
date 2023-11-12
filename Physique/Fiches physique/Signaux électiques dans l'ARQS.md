#chapitre1 #electricite #signal
## Charge et courante électrique
### Charges électrique:
Propriété permettant modéliser les interactions électromagnétique 
- $q=ne$
- $e=1,6 \cdot 10^{-19}$ 
### Courante électrique: 
Mouvement d'ensemble ordonnée de charges électriques.
#### Direction
- sens conventionnelle du courante: du plus ver le moins.
- sens des électrons : inverse du sens conventionnelle
#### Intensité
Débit de charge qui traverse la section. 
- $\displaystyle i(t)= \frac{d q}{d t}$ 
- $q= \int_{t_{0}}^{t_{1}}i(t)dt$ charge transité entre $t_{0}$ et $t_{1}$ 
#### Régime stationnaire: 
Ne dépende pas du temps. 
#### Régime variable:
Dépende du temps, courant pas constant. 


## Potentiel et tension
### Potentiel électrique:
$V$ est le potentiel électrique qui dépende de la position 
Energie Potentielle électrique: $E_{pe}=qV$

### Tension:
Différence de potentiel électrique entre deux points.
- $U_{BA}=V_{A}-V_{B}$ Tension entre les points $B$ et $A$.

## Approximation des Régimes Quasi-Stationnaires (ARQS)
Consiste a négliges les phénomènes de propagation des signaux 
- $\tau \approx \frac{L}{C}$ avec $L$ la longueur des fils et $C$ la célérité de la lumière
- $\frac{L}{C}<<T$ ou $L << CT$ 

## Dipôles 
Composant relié au circuit via deux bornes 
Caractérises par $i(t)$, $u(t)$, $P(t)$
### Puissance, conventions et caractéristiques:
#### Puissance:
$\displaystyle P(t)=\frac{dE}{dt}$    $P$ échangé entre dipôle et circuit
#### Convention générateur:
$P_{cédé}=u(t)i(t)$ cédé par le dipôle
#### Convention récepteur:
$P_{reçue}=u(t)i(t)$ reçue par le dipôle
#### Caractéristique d'un dipôle:
$P$ Relation $u=f(i)$

### Resistance (récepteur): 
Oppose l'écoulement du courante.
- Caractéristique (loi d'Ohm): $u(t)=Ri(t)$
- Puissance: $P(t)=Ri^{2}(t)=\frac{u^{2}(t)}{R}$
- Elle ne restitue jamais de l'énergie, seulement recevoir 

### Condensateurs (récepteur):
 $\boxed{\text{On a toujours continuité de la tension aux bornes d'un condensateur.}}$
- $q(t)=C  u(t)$   $C$ en farad
- Caractéristique: $i(t)=C \frac{du(t)}{dt}$ 
- Puissance : $P(t)= \frac{dE_{elec}(t)}{dt}$     énergie électrique stocke
- $E_{elec}(t)=\frac{1}{2}Cu^{2}(t)$ 

### Bobines (récepteur):
$\boxed{\text{Le courant traversant une bobine est toujours continue.}}$
- [[Induction Statique#Force électromotrice auto-induite|Caractéristique :]] $u(t)=L \frac{di(t)}{dt}$
- Puissance : $P(t)=L \frac{di}{ft} \times i(t) = \frac{dE_{mag}(t)}{dt}$
- Energie : $E_{mag}(t)=\frac{1}{2}Li^{2}(t)$

### Générateurs de tension (générateur):
Générateur ideal: tension $e(t)$ indépendant du reste du circuit
- $u(t)=e(t)$ 
Source réelle, modèle de thévenin :
- $u=e-Ri$
- $i(t)= \frac{e-u}{R_{g}}$ 
![[image modele thevenin.png|300]]

## Lois de Kirchhoff
### Lois de nœuds : 
La somme algébrique des intensités des courants qui entrent par un nœud est égale à la somme algébrique des intensités des courants qui en sortent.
- car la charge $q(t)$ est constante : $\frac{dq}{dt}=0$
### Loi des Mailles :
La somme algébrique des tensions le long d'un contour fermé est nulle.
- $U_{AA}=U_{AB}+U_{BC}+U_{CD}+U_{DA}=0$
### Association des résistances 
#### En série :
- $R_{eq}=\sum R_{i}$ 
##### Pont diviseur de tension :
- $\displaystyle U_{n} = \frac{R_{n}}{R_{eq}} U$ 
- $\displaystyle U_{1} = \frac{R_{1}}{R_{1}+R_{2}} U$
![[image pont diviseur tension.png |300]]
#### En parallèle :
- $\frac{1}{R_{eq}}= \sum \frac{1}{R_{eq}}$
##### Pont diviseur de courant
- $\displaystyle U = \frac{R_{eq}}{R_{n}} i$
- $\displaystyle i_{1} = \frac{R_{2}}{R_{1}+R_{2}} i$ 

![[image pont diviseur de courante.png]]