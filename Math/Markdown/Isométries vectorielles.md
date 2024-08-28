Dans tout le chapitre $E$ est un espace euclidien.
## Isométries vectorielles 
### Définition et caractérisation 
Soit $f \in \mathcal{L}(E)$ et $\mathcal{B}$ une base orthonormé de $E$.
$f$ est un isomorphisme vectorielle de $E$ si : 
$\forall x \in E, \quad \| f(x) \|  = \| x \|$  (conservation de la norme)
$\Leftrightarrow  \forall (x,y) \in E^{2}, \quad (f(x) | f(y)) =(x | y)$   (conservation du produit scalaire)
$\Leftrightarrow f(\mathcal{B})$ est une base orthonormé de $E$. 
$\Leftrightarrow Mat_{\mathcal{B}}(f)=M$ est orthogonal $\Leftrightarrow MM^{T}=I_{n}$
### Symétries orthogonales 
Soit $F$ un sev de $E$.
La symétrie orthogonale $s_{F}$ par rapport à $F$ est la symétrie de base $F$ et de direction $F^{\perp}$.
- Les symétries orthogonales sont des isométries. Si une symétrie est une isométrie alors c'est une symétrie orthogonal. 
- Réflexion : symétrie orthogonale par rapport à un hyperplan $H$ de $E$.
![[image symetrie orthogonal.png|300]]
### Sous-espaces stables et sous-espaces propres 
Soit $f$ une isométrie de $E$ et $f(F) \subset F$ :
$\implies f(F^{\perp} ) \subset F^{\perp}$
Les valeurs propres *réelles* possibles d'une isométrie sont : $-1$ out $1$.
- $f(E_{\lambda }^{\perp} ) \subset E_{\lambda }^{\perp}$
### Groupe orthogonal d'un espace euclidien
$O(E)$ ensemble des isométries vectorielles de $E$. 
- $id_{E} \in O(E)$.
- Si $f,g \in O(E)$, alors $f \circ g \in O(E)$.
- $O(E) \subset \mathcal{GL}(E)$. Alors si $f \in O(E)$, $f$ est une automorphisme de $E$ et $f^{-1}$ est une isométrie de $E$.

## Matrices orthogonales
### Définition 
Soit $A$ de $\mathcal{M}_{n}(\mathbb{R})$. On muni $\mathbb{R}^{n}$ du produit scalaire canonique. 
$A$ est orthogonal 
$\Leftrightarrow A^{T}A = I_{n}$
$\Leftrightarrow A$ est inversible et $A^{-1} = A^{T}$ 
$\Leftrightarrow$ $A^{T}$ est orthogonal.	
$\Leftrightarrow \det(A) \in \{ -1,1 \}$
$\Leftrightarrow$ les colonnes de $A$ forment une base orthonormé de $\mathbb{R}^{n}$
$\Leftrightarrow$ les lignes de $A$ forment une base orthonormé de $\mathbb{R}^{n}$
- Une base de $E$ est orthonormée $\Leftrightarrow$ il existe une matrice de passage orthogonal d'une autre base orthonormée de $E$. 
### Orientation d'une isométrie
Isométrie vectorielle direct : $\det(f) = +1$.
- Appelles aussi rotations
Isométrie vectorielle indirect : $\det(f) = -1$.
Groupe spécial direct orthogonal $SO(E)$ : isométries vectorielles directes de $E$. 
### Orientation de l'espace
On oriente l'espace $E$ en choisissant une base orthonormée $\mathcal{B}_{0}$ qu'on dit "directe". Toutes les bases qui ont la même orientation (la matrice de passage entre $\mathcal{B}_{0}$ et l'autre base a $\det(P)=+1$) sont directe et les autres sont indirectes. 

## Reduction des matrices symétriques réelles 
- Les sous espaces propres d'une matrice symétrique sont orthogonaux 
- Lemme : Le polynôme caractéristique d'une matrice symétrique est scindé sur $\mathbb{R}$. 

## Théorème spectral 
Toute matrice symétrique réelle $S$ est diagonalisable dans une base orthonormale.
C'est à dire, Il existe une matrice orthogonal $P$ et une matrice diagonale réelle $D$ telle que :
$D = P^{T} S P$ 

## Isométries vectorielles en dimension 2
### Rotations en dimension 2
Les éléments de $SO_{2}(\mathbb{R})$ sont les matrices $\displaystyle R(\theta) = \begin{pmatrix} \cos(\theta) & -\sin(\theta) \\ \sin(\theta) & \cos(\theta) \end{pmatrix}$
- $R(\theta)R(\theta') = R(\theta+\theta')$
### Classification
Soit $f \in O(E)$.
- Soit $\ker(f-id_{E}) = \{ 0 \}$ : $f$ est une rotation.
- Soit $\ker(f-id	_{E}) = Vect(u)$ : $f$ est la réflexion par rapport à la droite $Vect(u)$.
- Soit $\ker(f-id_{E}) = \mathbb{R}^{2}$ : $f = id_{E}$ 

## Isométries vectorielles en dimension 3
### Orientation d'un plan
On choisit une un vecteur $a$ de $H^{\perp}$. Alors, les bases directes de $H$ sont les bases $U$ telles que $(U,a)$ est directe dans $E$.
### Réduction des isométries en dimension 3
Soit $f$ une isométrie de $\mathbb{R}^{3}$. Il existe une BON $\mathcal{B}$ de $E$ tel que :
$Mat_{\mathcal{B}}(f) = \begin{pmatrix} \pm 1 & 0 & 0 \\ 0 & \cos(\theta) & -\sin(\theta) \\ 0  & \sin(\theta) &\cos(\theta)  \end{pmatrix}$
### Classification
#### Isométrie directe : Rotation vectorielle 
On dit que $f$ est la rotation d'axe $E_{1}(f)$ orienté par $e_{1}$ et d'angle $\theta$.
$f$ est une rotation :
$\Leftrightarrow det(Mat_{\mathcal{B}}(f)) = 1$ 
$\Leftrightarrow$ Il existe une BON $(e_{1},e_{2},e_{3})$ et $\theta \in \mathbb{R}$ tels que : $Mat_{\mathcal{B}}(f) = \begin{pmatrix} + 1 & 0 & 0 \\ 0 & \cos(\theta) & -\sin(\theta) \\ 0  & \sin(\theta) &\cos(\theta)  \end{pmatrix}$
- Si $f \neq id$, l'ensemble de vecteurs invariants $E_{1}(f)= \ker(e_{1})$ qu'on appelle "axe de rotation" et $\theta$ ne dépend que de l'orientation de $e_{1}$.
Soit $v$ un vecteur $\perp$ à l'axe de rotation qui est dirigée par le vecteur normé $e_{1}$ :
- $f(v) = \cos(\theta) v + \sin(\theta) e_{1} \wedge v$ 
![[image rotation vectorielle.png]]
#### Isométries indirectes : Réflexion
$f \in O(E)$ est une réflexion :
$\Leftrightarrow \dim(Ker(f-id_{E})) = 2$
- Il existent plus de isométries indirectes mais ils sont HP.
