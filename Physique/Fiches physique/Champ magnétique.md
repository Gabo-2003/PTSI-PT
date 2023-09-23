#chapitre28 #magnetique
## Champ  
Tout fonction de l'espace et du temps que représente la valeur d'une grandeur physique.
### Champ scalaire :
Caractérisé par une nombre (et unité):
### Champ vectoriel :
Grandeur caractérisé par une direction. Dans l'espace, il est équivalente à 3 champs scalaires.
### Uniforme :
Si sa valeur est la même pour tout point.
### Stationnaire : 
Si la valeur en tout point de l'espace ne dépend que de $t$.
### Lignes de champs :
Courbes tangentes au vecteur $\vec{S}$ en tout point et orienté dans la direction du vecteur.
- Pas d'angles, peuvent pas se croiser, pas d'info sur la norme.
![[image lignes de champ.png|700]]

## Champ magnétique 
### Cartographie du champ $\vec{B}$
#### Champ créé par un fil rectiligne 

| ![[image fil rectiligne.png]] | ![[image main droite fil rectiligne.png]] |
| ------------------------------------ | ------------------------------------ |
- Plus on s'éloigne du fil, moins le champ génère est intense.
#### Champ créé par une spire

| ![[image champ spire.png\|300]] | ![[image main droite spire.png\|300]] |
| ------------------------------- | ------------------------------------- |

#### Champ créé par un solénoïde
![[image champ solenoide.png|300]]
#### Champ créé par un aimant permanent
![[image champ aimant permanent.png|300]]
### Propriétés des lignes de champ
- Ils sont des courbes fermés.
- Ils s'enroulent autour de leur sources.
- L'intensité du champ augmente si les lignes voisins se rapprochent.

## Symétries et invariances d'un champ magnétique créé par une distribution de courante. 
> [!quote]- Principe de Curie
> "Lorsque certaines causes produisent certains effets, les éléments de symétrie des causes doivent se retrouver dans les effets produits"
### Symétries 
- Un plan de symétrie de la distribution de courante est un plan d'antisymetrie du champ $\vec{B}$ crée par ces courantes.
- Un plan d'antisymétrie de la distribution de courante est un plan de symétrie du champ $\vec{B}$ crée par ces courantes.
### Invariances
- Le champ créé par une distribution invariante par translation le long d'un axe $(oz)$ ne dépend pas de la coordonné $z$ : $\vec{B}=\vec{B}(x,y,z_{1})=\vec{B}(x,y,z_{2})=\vec{B}(x,y)$. 
- La norme du champ crée par une distribution invariante par rotation autour d'un axe $(oz)$ ne dépend pas de la coordonné $\theta$ : $\lVert \vec{B}(r,\theta_{1},z) \rVert = \lVert \vec{B}(r,\theta_{2},z) \rVert =  \frac{\partial B}{\partial \theta} (r, \theta, z) = 0$ 
### Conséquence sur la direction du champ 
- Le champ $\vec{B}$ en tout point d'un plan d'antisymetrie de la distribution de courant est compris dans ce plan (le vecteur).
- Le champ $\vec{B}$ en tout point d'un plan de symétrie de la distribution de courant est normal à ce plan (le vecteur).

## Moment magnétique 
### Moment d'une spire : 
$\vec{\mu}=I \vec{S}=IS \vec{n}$ en $A \cdot m^{2}$
- $\vec{S}$ surface du cercle selon la règle de la main droite. 
### Moment d'une solénoïde :
Somme du moment de chaque spire.
### Moment magnétique d'une aimant :
$\displaystyle \vec{M} = \frac{\vec{\mu}}{V}$ 
- L'aimantation est au moment magnétique ce que la masse volumique est à la masse 