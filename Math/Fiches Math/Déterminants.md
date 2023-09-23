## Déterminant d'une matrice carrée de taille $n$
### Définition
$\exists ! \, f: \mathcal{M}_{n}(\mathbb{K})\longrightarrow \mathbb{K}$ qui vérifie
- $f(mat(C_{1}, \dots , C_{i} + \lambda C_{j}, \ldots, C_{n})) = f(mat(C_{1}, \ldots, C_{i}, \ldots , C_{n})) + \lambda f(mat(C_{1}, \ldots, C_{j}, \ldots , C_{n}))$ 
- $f(mat(C_{1}, \ldots, C_{i}, \ldots, C_{j}, \ldots, C_{n}))= -f(mat(C_{1}, \ldots, C_{j}, \ldots, C_{i}, \ldots, C_{n}))$ 
- $f(I_n)=1$
L'application $f$ s'appelle déterminant et il est noté : $det$ 
- $\det(A) = \begin{vmatrix} a_{1,1}  & \cdots &  a_{1,n} \\ \vdots  &   & \vdots \\ a_{n,1}  &  \cdots & a_{n,n} \end{vmatrix}$ 
### Propriétés 
Soit $A \in \mathcal{M}_{n}(\mathbb{K})$ 
- Si $A$ possède deux colonnes égales, $\det(A)=0$. 
- Si $A$ possède deux colonnes proportionnelles, $\det(A)=0$.
- Si les colonnes de $A$ forment une famille liée, $\det(A)=0$ 
- $A$ inversible $\Leftrightarrow \det(A) \neq 0$ 
- Si $A$ inversible, alors $\displaystyle\det(A^{-1})= \frac{1}{\det(A)}$. 
Soit $(A,B) \in \mathcal{M}_{n}(\mathbb{K})^{2}$  et  $\lambda \in \mathbb{K}$
- $\det(AB)=\det(A)\det(B)$
- $\det(\lambda A)=\lambda^{n}\det(A)$ 
Soit le système linéaire $AX=B$ d'inconnue $X \in \mathbb{K}^{n}$ avec $A \in \mathcal{M}_{n}(\mathbb{K})$ et $B \in \mathbb{K}^{n}$ :
- $\exists!$ solution $\Leftrightarrow \det(A) \neq 0$, dans ce cas, on parle d'un système de Cramer.
- $AX=O_{\mathbb{K}^{n}}$ admet une infinité de solutions $\Leftrightarrow \det(A)=0$. 
### Calculs de déterminants 
- Le déterminant est invariant par transvection : $C_{i} \leftarrow  \lambda C_{i}+C_{j}$   ou  $L_{i} \leftarrow  \lambda L_{i}+L_{j}$. 
- Le déterminant change de signe à chaque transposition : $C_{i} \leftrightarrow C_{j}$ ou $L_{i} \leftrightarrow L_{j}$ . 
- $\det(mat(C_{1}, \ldots, \alpha C_{i}, \ldots, C_{n}))= \alpha \det(mat(C_{1}, \ldots, C_{i}, \ldots, C_{n}))$ 
- Le déterminant d'une matrice triangulaire est égal au produit des coefficients sur la diagonale. 
- Si $A=\begin{pmatrix} a & b  \\ c  & d \end{pmatrix}$ alors $\det(A)=\begin{vmatrix} a & b  \\ c & d \end{vmatrix}=ad-bc$ 
#### Développement suivant une ligne ou une colonne en dimension 3
$\begin{vmatrix} x_{1} & y_{1} & z_{1}  \\ x_{2} & y_{2} & z_{2}  \\ x_{3} & y_{3} & z_{3} \end{vmatrix}= x_{1} \begin{vmatrix} y_{2} & z_{2} \\ y_{3}&z_{3} \end{vmatrix}- y_{1} \begin{vmatrix} x_{2} & z_{2} \\ x_{3}&z_{3} \end{vmatrix} + z_{1}\begin{vmatrix} x_{2} & y_{2} \\ x_{3}&y_{3} \end{vmatrix}$ 
- On peut développer un déterminant suivant n'importe quelle ligne ou colonne si on respecte la règle des signes : $\begin{pmatrix} +  & - & +  \\ -  & +  & -  \\ +  & - & + \end{pmatrix}$ 

## Déterminant d'une famille de $n$ vecteurs
Soit $E$ une $\mathbb{K}.e.v$ de dimension $n$
- Déterminant d'une famille $(u_{1}, u_{2}, \ldots , u_{n})$ dans la base $B$ : $\det_{B}(u_{1}, u_{2}, \ldots, u_{n})$ 
Soit $B$ une base de $E$ 
- Une famille $B'$ de $n$ vecteurs est base de $E \Leftrightarrow \det_{B}(B') \neq 0$ 

## Déterminant d'un endomorphisme
C'est le déterminant de la matrice associe (le det ne dépend de la base) 
Soit $f$ et $g$ deux éléments de $\mathcal{L}(E)$ et $\lambda \in \mathbb{K}$ 
- $\det(f \circ g)= \det(f)\det(g)$
- $\det(id_{E})=1$
- $\det(\lambda f)= \lambda^{n}\det(f)$ 
- $f$ automorphisme de $E \Leftrightarrow \det(f) \neq 0$ alors $\det(f^{-1})= \frac{1}{\det(f)}$ 
