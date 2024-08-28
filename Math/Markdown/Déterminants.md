## Déterminant d'une matrice carrée de taille $n$
### Linéarité par rapport aux colonnes 
$f$ est linéaire à la colonne $C_{j}$ si $\forall \alpha \in \mathbb{K}, \forall M \in M_{n}(\mathbb{K}), \forall C'_{j}$ :
- $f(C_{1}| \dots | C_{i} + \lambda C_{j}| \ldots| C_{n})) = f(C_{1}| \ldots| \underbrace{C_{i}| \ldots | C_{n}) + \lambda f(C_{1}| \ldots| C_{j}}_{\text{trasposition}} | \ldots | C_{n})$ 
### Antisymétrie par rapport aux colonnes
- $\forall i, j$   $f(C_{1}| \ldots| C_{i}| \ldots| C_{j}| \ldots| C_{n}))= -f(C_{1}| \ldots| C_{j}| \ldots| C_{i}| \ldots| C_{n}))$ 
### Théorème d'existance et unicité du determinant
$\exists ! \, f: \mathcal{M}_{n}(\mathbb{K})\longrightarrow \mathbb{K}$ qui vérifie
- $f$ linéaire par rapport à tous les colonnes de sa variable.
- $f$ antisymétrique par rapport à tous les colonnes de sa variable.
- $f(I_n)=1$
L'application $f$ s'appelle déterminant et il est noté : $det$ 
- $\det(A) = \begin{vmatrix} a_{1,1}  & \cdots &  a_{1,n} \\ \vdots  &   & \vdots \\ a_{n,1}  &  \cdots & a_{n,n} \end{vmatrix}$ 
### Propriétés 
Soit $(A,B) \in \mathcal{M}_{n}(\mathbb{K})^{2}$  et  $\lambda \in \mathbb{K}$
- Si $A$ possède deux colonnes égales, $\det(A)=0$ 
- Si $A$ possède deux colonnes proportionnelles, $\det(A)=0$
$\Rightarrow$ Si les colonnes de $A$ forment une famille liée, $\det(A)=0$ 
- $\det(\lambda A)=\lambda^{n}\det(A)$ 
#### Operations élémentaires
#### Matrices inversibles 
- $A$ inversible $\Leftrightarrow \det(A) \neq 0$ 
Soit le système linéaire $AX=B$ d'inconnue $X \in \mathbb{K}^{n}$ avec $A \in \mathcal{M}_{n}(\mathbb{K})$ et $B \in \mathbb{K}^{n}$ :
- $\exists!$ solution $\Leftrightarrow \det(A) \neq 0$, dans ce cas, on parle d'un système de Cramer.
- $AX=O_{\mathbb{K}^{n}}$ admet une infinité de solutions $\Leftrightarrow \det(A)=0$. 
#### Déterminant d'un produit
- $\det(AB)=\det(A)\det(B)$
#### Déterminant de l'inverse
- Si $A$ inversible, alors $\displaystyle\det(A^{-1})= \frac{1}{\det(A)}$ 
#### Déterminant de la transposée
- $\det(A^{\intercal})= \det(A)$  
### Calculs de déterminants 
- Le déterminant est invariant par transvection : $C_{i} \leftarrow  \lambda C_{i}+C_{j}$   ou  $L_{i} \leftarrow  \lambda L_{i}+L_{j}$. 
- Le déterminant change de signe à chaque transposition : $C_{i} \leftrightarrow C_{j}$ ou $L_{i} \leftrightarrow L_{j}$ . 
- $\det(mat(C_{1}, \ldots, \alpha C_{i}, \ldots, C_{n}))= \alpha \det(mat(C_{1}, \ldots, C_{i}, \ldots, C_{n}))$ 
- Le déterminant d'une matrice triangulaire est égal au produit des coefficients sur la diagonale. 
- Si $A=\begin{pmatrix} a & b  \\ c  & d \end{pmatrix}$ alors $\det(A)=\begin{vmatrix} a & b  \\ c & d \end{vmatrix}=ad-bc$ 
#### Développement suivant une ligne ou une colonne en dimension 3
$\begin{vmatrix} x_{1} & y_{1} & z_{1}  \\ x_{2} & y_{2} & z_{2}  \\ x_{3} & y_{3} & z_{3} \end{vmatrix}= x_{1} \begin{vmatrix} y_{2} & z_{2} \\ y_{3}&z_{3} \end{vmatrix}- y_{1} \begin{vmatrix} x_{2} & z_{2} \\ x_{3}&z_{3} \end{vmatrix} + z_{1}\begin{vmatrix} x_{2} & y_{2} \\ x_{3}&y_{3} \end{vmatrix}$ 
- On peut développer un déterminant suivant n'importe quelle ligne ou colonne si on respecte la règle des signes : $\begin{pmatrix} +  & - & +  \\ -  & +  & -  \\ +  & - & + \end{pmatrix}$ 

## Déterminant d'un endomorphisme, d'une famille de vecteur 
### Déterminant d'une famille de $n$ vecteurs
Soit $E$ une $\mathbb{K}.e.v$ de dimension $n$ de base $B$.
- $\det_{B}(x_{1}, \ldots x_{n}) = \det(Mat(x_{1}, \ldots x_{n}))$
- $\det_{B}(B)=1$
- $\det_{B}(x_{1}, \ldots, x_{n}) = \det(P_{B \to B'}) \det_{B'}(x_{1}, \ldots, x_{n})$
### Déterminant d'un endomorphisme
$\det(f) = \det(Mat_{B}(f))$
Le déterminant d'un endomorphisme ne dépende pas de la base
Soit $f$ et $g$ deux éléments de $\mathcal{L}(E)$ et $\lambda \in \mathbb{K}$ 
- $\det(f \circ g)= \det(f)\det(g)$
- $\det(id_{E})=1$
- $\det(\lambda f)= \lambda^{n}\det(f)$ 
- $\det_{B}(f(x_{1}), \ldots, f(x_{n})) = \det(f) \det_{B}(x_{1}, \ldots, x_{n})$
- Deux matrices semblables ont le même determinant
### Caractérisation des automorphismes
$f$ automorphisme de $E \Leftrightarrow \det(f) \neq 0$ alors $\det(f^{-1})= \frac{1}{\det(f)}$ 
