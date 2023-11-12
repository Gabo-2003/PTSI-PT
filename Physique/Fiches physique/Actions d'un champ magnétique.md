#chapitre29 #magnetique
## Forces de Laplace
$\boxed{d \vec{F_{L}}=I \vec{dl} \wedge \vec{B}}$ 
- Perpendiculaire à la direction du courante et du champ $\vec{B}$
- Proportionnelle à la longueur du conducteur et à l'intensité du champ.
### Rails de Laplace
Tige rectiligne conductrice libre de glisser le long de deux rails conducteurs.
![[image rails de laplace.png|400]]
- Résultant des Forces de Laplace : $R_{L}=IBL \vec{e_{x}}$
#### Circuit fermé :
- Resultant nulle
#### Puissance :
$d \mathcal{P} (d \vec{F_{L}})=d \vec{F_{L}}\cdot \vec{v}$
- Non nulle et donc cette force peut fournir un travail.

## Couple et puissance de $\vec{F_{L}}$ pour une spire
- Couple : $\vec{\Gamma} =I\vec{S}\wedge \vec{B} = \vec{\mu} \wedge \vec{B}$ 
- Puissance : $\mathcal{P}_{L}=-BIS\dot{\theta}\sin(\theta)$ 

## Actions d'un champ magnétique uniforme sur un aimant
Les forces de Laplace ne permettent pas de décrire les forces subies par un aimant  permanent. Mais $\vec{\Gamma} = \vec{\mu} \wedge \vec{B}$ reste valable. 
### Positions d'équilibre de l'aimant : $\vec{\Gamma}=\vec{0}$
- Parallèle ($\vec{\mu}$ et $\vec{B}$ même sens) : $\theta = 0$ stable
- Antiparallèle : $\theta=\pi$ instable
### Effet moteur
On peut générer un champ magnétique tourant en un point à l'aide de deux solénoïdes d'axes perpendiculaires.
- $\vec{B}=I_{0}K \begin{pmatrix} \cos(\omega_{0} t)  \\ \sin(\omega_{0} t)  \\ 0 \end{pmatrix}$

## Lois de l'induction
Comment un champ magnétique peut provoquer l'apparition d'un courante dans un circuit fermé.
### Induit
portion de circuit dans laquelle un courante électrique est généré.
### Inducteur 
Système créant le champ magnétique à l'origine du phénomène d'induction
### Induction statique ou motionnelle 
#### Statique 
Induit supposé rigide et fixe. $\vec{B}$ varie avec le temps due à un mouvement de l'inducteur ou variation de la courante
#### Motionnelle 
Champ stationnaire. Variation de $\vec{B}$ due au mouvement ou déformation de l'induit 
### Flux magnétique 
C'est une grandeur physique mesurable caractérisant l'intensité et la répartition spatiale du champ magnétique. 
- $\boxed{\phi_{s}= \int \int_{M \in S} \vec{B}(M)\vec{dS}}$ en $Wb$ weber
#### Pour une spire :
$\phi_{s}=\vec{B}\cdot \vec{S} = BS \cos(\theta)$ 
- Le flux est d'autant plus grand que le vecteur "rentre" dans la surface. nul si le vecteur est dans le plan de la surface 
- Flux positive si le vecteur "rentre" (selon la main droite) et négative sinon
#### Pour un solénoïde
$\phi_{tot}= \mu \phi_{i}$ avec $\mu$ le [[Champ magnétique#Moment magnétique|moment magnétique]].  
### Loi de Faraday
Relie le courant induit dans un circuit fermé à la variation de flux magnétique via la notion de force électromotrice (f.é.m.) induit. 
- $\boxed{e(t)=- \frac{d\Phi}{dt}}$  
### Loi de Lenz
Les effets des phénomènes d'induction s'opposent aux causes qui leur ont donnée naissance.