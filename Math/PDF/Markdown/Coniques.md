## Coniques
### Définition par foyer, directrice et excentricité
Soient $D$ une droite, $F \notin D$ un point du plan et $e>0$ un réel.
$C = \{ M | d(M,F) = e \cdot  d(M,D) \}$ : conique de foyer $F$, de directrice $D$ et d'excentricité $e$.
- La droite orthogonale à la directrice $D$ passant par le foyer $F$ est l'axe focal de la conique.
Paramètre de la conique :  $p = e \cdot  d(F,D)$ 
### Équation cartésienne
Dans le repère orthonormé $(F,\overrightarrow{i}, \overrightarrow{j})$ avec $\overrightarrow{i}$ qui dirige l'axe optique. 
L'équation de la conique de foyer $F$, de directrice $D$ et d'excentricité $e$ est :
$x^{2}+y^{2} = (ex+p)^{2}$
### Types de conique 
#### Parabole : $e=1$
![[image conique parabole.png|638]]
L'équation de la parabole dans le repère orthonormé d'origine $S$ sommet de la parabole est : 
$Y^{2}=2pX$
#### Ellipse : $0<e<1$
![[image ellipse conique.png]]
Équation de l'ellipse dans le repère orthonormé d'origine $O$ centre  de l'ellipse :
$\displaystyle  \frac{X^{2}}{a^{2}} + \frac{Y^{2}}{b^{2}} = 1$
- Demi-grand axe : $a$
- Demi-petit axe :  $b$
- $a^{2} = b^{2}+c^{2}$ 
##### Paramétrage de l'ellipse
La courbe paramétrée $\displaystyle t \longmapsto \Big( X(t) = a \cos(t), Y(t) = b \sin(t) \Big)$ est un paramétrage $C^{1}$ régulière de l'ellipse de centre $O$, de demi-grand axe $a$ et de demi-petit axe $b$.
#### Hyperbole : $e>1$
![[image hyperbole conique.png]]
L'équation de l'hyperbole dans le repère orthonormé d'origine $O$ centre de l'hyperbole ou $\overrightarrow{i}$ dirige l'axe focal est :
$\displaystyle \frac{X^{2}}{a^{2}} - \frac{Y^{2}}{b^{2}} = 1$
- $c^{2}=a^{2}+b^{2}$
- Demi-axe focal : $a$
- Demi-axe transverse : $b$ 
- Asymptotes : $\displaystyle Y = \pm \frac{b}{a}X$
##### Paramétrage usuel de l'hyperbole
Paramétrage $C^{1}$ régulière de l'hyperbole de centre $O$ :
$t \longmapsto \Big( X(t)= a \epsilon \,ch(t), Y(t) = b \,sh(t) \Big)$ 
- Avec $\epsilon \in \{ -1,1 \}$

## Réduction des coniques 
### Équation générale d'une conique 
Une courbe du plan est une conique si elle admet dans un repère orthonormal $(O,\overrightarrow{i},\overrightarrow{j})$ :
$ax^{2}+2bxy+cy^{2}+dx+ey+f = 0$ 
- avec $(a,b,c) \neq (0,0,0)$ 
Soit $U = \begin{pmatrix} x \\ y \end{pmatrix}$ ,  $S = \begin{pmatrix} a & b \\ b & c \end{pmatrix}$  et $L = \begin{pmatrix} d & e \end{pmatrix}$.
On peut l'écrire en forme matriciel :
$U^{T}SU+LU+f=0$
#### Équation réduite  
Soit $\lambda_{1}$ et $\lambda_{2}$ les valeurs propres de $S$. 
Si $\lambda_{1} \neq 0$ et $\lambda_{2} \neq 0$ :
$\lambda_{1}X_{1}^{2}+\lambda_{2}X_{2}^{2} + K = 0$
### Type d'une conique
Type ellipse : $\lambda_{1}\lambda_{2}>0$
Type hyperbole : $\lambda_{1}\lambda_{2}<0$
Type parabole : $\lambda_{1}\lambda_{2}=0$
### Hyperbole équilatère 
La courbe d'équation $xy=k$ est une hyperbole avec $a=b$ et des asymptotes orthogonales dite hyperbole équilatère. 