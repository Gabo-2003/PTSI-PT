## Produit scalaire 
### Définition d'un produit scalaire 
Soit $E$ un $\mathbb{R}.e.v$.
Alors l'application $\phi : E \times E \longrightarrow \mathbb{R}$ est un produit scalaire de $E$ si il est :
- Symétrique : $\forall (x,y) \in E^{2}, \quad \phi (x,y) = \phi (y,x)$.
- Bilinéaire :
	- Linéaire à gauche.
	- Linéaire à droite.
	- Définie positive : $\phi (x,x)\geq 0$ et $\phi (x,x)=0 \implies x=0$.
### Espaces préhilbertiens et euclidiens
#### Espace préhilbertiens réel : 
Tout espace vectoriel réel $E$ muni d'un produit scalaire $(. | .)$.
#### Espace euclidien 
Espacé préhilbertien réel de dimension finie.
#### Produits scalaires au programme
Sur $\displaystyle C([a,b], \mathbb{R}) : \quad \quad \left< f,g \right> = \int_{a}^{b} fg$.
Sur $\displaystyle C([a,b], \mathbb{R}) : \quad \quad \left< f,g \right> = \int_{a}^{b} w(t) f (t) g (t) \; d{t}$ avec $w$ continue strictement positive sur $[a,b]$.
Sur $\displaystyle \mathbb{R}[X] : \quad \quad \left< P, Q \right> = \int_{a}^{b} \tilde{P} \tilde{Q}$.
Produit canonique de $\mathbb{R}_{n}[X] : \quad \quad \left< u,v  \right> = \sum_{k=1}^{n}  u_{k} v_{k}$ avec $u = (u_{1},u_{2}, \ldots) \in \mathbb{R}^{n}$ et pareil pour $v$.
Sur $\mathcal{M}_{n}(\mathbb{R}) = \left< A,B \right> = tr(A ^{T} B)$

### Norme associe à un produit scalaire
Soit $E$ un espace préhilbertien réel de produit scalaire $(. | .)$.
La norme euclidienne de $(. | .)$ est l'application $N_{2} : E \longrightarrow \mathbb{R}_{+}$ :
- $N_{2}(x) =\lVert x \rVert = \sqrt{(x | x) }$ 
- $\lVert kx \rVert = |k| \lVert x \rVert$   avec $k$ un réel.
- $\lVert x + y \rVert ^{2} = \lVert x \rVert ^{2} + 2 (x | y) + \lVert y \rVert ^{2}$
### Inégalités 
#### Inégalité triangulaire 
Soit $E$ un espace préhilbertien réel de produit scalaire $(. | .)$ :
$\forall x,y \in E$,         $\lVert x+y \rVert \leq \lVert x \rVert  + \lVert y \rVert$
- On a égalité si $x$ et $y$ sont positivement liés.
#### Inégalité de Cauchy-Schwarz 
Soit $E$ un espace préhilbertien réel de produit scalaire $(. | .)$ :
$\forall (x,y) \in E$,      $|(x | y) | \leq \lVert x \rVert \cdot \lVert y \rVert$
- On a égalité si $x$ et $y$ sont liés.

## Orthogonalité
### Vecteurs et sous-espaces orthogonaux
Soit $E$ un espace préhilbertien réel muni du produit scalaire $(. | .)$.
- Soit $x,y \in E$ : $x \perp y \Leftrightarrow (x | y) =0$
- Soit $F$ et $G$ deux sev de $E$ :   $F\perp G \Leftrightarrow \forall (x,y) \in G \times F,  \quad (x | y) =0$
- Il n'y a que le vecteur nul qui est orthogonaux a tout vecteur de l'espace.
- Une famille $(F_{i})_{i \in [[1,n ]]}$ de sev orthogonaux est en somme directe.
### Orthogonal d'un sev
Soit $F$ un sev de $E$.
Orthogonal de $F$ :   $F^{\perp} = \{ x \in E | \forall y \in F, (x | y) =0\}$.
- $F^{\perp}$ est un sev de $E$. 
Soit $F$ et $G$ deux sev de $E$ :
- $F \subset G \implies F^{\perp} \subset G^{\perp}$
- $F \cap F^{\perp} =\{ \overrightarrow{0} \}$
- $F \subset (F^{\perp} )^{\perp}$
Un vecteur $x$ de $E$ appartient a $F^{\perp} \Leftrightarrow$ $x$ est orthogonal a tout vecteur d'une famille génératrice de $F$.
### Familles orthogonales 
- Une famille de vecteurs est dite orthogonal si tous les vecteurs de la famille sont orthogonaux entre eux.
- Une famille orthogonal finie de vecteurs non nuls est libre.
#### Théorème de Pythagore 
Si $(x_{1}, x_{2}, \ldots, x_{p})$ est une famille orthogonal de $E$, alors :
$\displaystyle \left\| \sum_{i=1}^{p} x_{i} \right\|^{2} = \sum_{i=1}^{p} \| x_{i} \|  ^{2}$
- $\| x_{1} + x_{2} + \ldots + x_{p} \|^{2} = \| x_{1} \|  ^{2} + \| x_{2} \|  ^{2} + \ldots + \| x_{p} \|  ^{2}$
- Pour $p>2$ la réciproque est fausse.
### Algorithme d'orthonormalisation de Gram-Schmidt 
Soit $(u_{1}, \ldots, u_{p})$ une famille libre, alors il existe une famille orthonormale $(e_{1}, \ldots, e_{p})$ tel que :
- $Vect(u_{1}, \ldots, u_{p}) = Vect(e_{1}, \ldots, e_{p})$
- $e_{i} \in (u_{1}, \ldots, u_{p})$ 
![[image algo gram-schmidt.png|500]]
### Existence de bases orthonormées dans un espace euclidien 
Soit $E$ une espace euclidien et $(e_{i})_{i \in [ [1,n] ]}$ une base orthonormale de $E$.
- Tout espace euclidien non réduit à $\{ \overrightarrow{0} \}$ admet une base orthonormée. 
#### Coordonnées dans une base orthonormée
$\forall x \in E$, $\displaystyle x = \sum_{i=1}^{n} (x | e_{i}) e_{i}$
#### Expression du produit scalaire dans une BON
$\forall (x,y) \in E^{2}$, $\displaystyle (x | y) = \sum_{i=1}^{n} (x | e_{i})  (y | e_{i})$
- Dans une base orthonormale tout se ramène au produit scalaire canonique.

## Projection orthogonale sur un s.e.v de dimension finie
### Supplémentaire orthogonal 
Soit $F$ un sev de dimension finie d'un espace vectoriel préhilbertien de $E$, alors $E = F \oplus F^{\perp}$.
### Projection orthogonale sur un sev de dimension finie 
#### Definition
Soit $F$ un sev de dimension finie de $E$ préhilbertien. La projection orthogonale sur $F$ est la projection sur $F$ de direction $F^{\perp}$.
Soit $(f_{1}, \ldots f_{p})$ une base orthonormé de $F$. Alors 
$\forall x \in E$,    $\displaystyle p_{F}(x) = \sum_{i=1}^{p} (x | f_{i}) f_{i}$ 
#### Méthode rapide
![[image projection orthogonal.png|300]]
Soit $(v_{1},v_{2}, \ldots, v_{m})$ une famille génératrice d'un sev $F$ d'un espace euclidien $E$.
Le projeté orthogonal de $x \in E$ sur $F$ est l'unique vecteur $y \in F$ tel que :
$\forall i \in [ [1,m] ]$, $(z | v_{i})=(x-y | v_{i}) = 0 \Leftrightarrow (x | v_{i}) = (y | v_{i})$
### Distance d'un point à un sev 
Soit $E$ un espace préhilbertien. 
Soit $F$ un sev de dimension finie de $E$.
$x \in E, \quad \displaystyle d(x,F)= \| x- p_{F}(x) \|  = \inf_{y \in F} \| x-y \|$