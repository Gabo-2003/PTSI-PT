#matrice 
On note une matrice $A=(a_{ij})_{\begin{align*}  1 \leq i \leq n \\ 1 \leq j \leq p \end{align*}}$ avec $n$ lignes et $p$ colonnes 
## Opérations sur les matrices 
### Addition de deux matrices 
$A+B=(a_{ij}+b_{ij})_{\begin{align*}  1 \leq i \leq n \\ 1 \leq j \leq p \end{align*}}$ 
### Multiplication par un scalaire 
$\lambda A= (\lambda a_{ij})_{\begin{align*}  1 \leq i \leq n \\ 1 \leq j \leq p \end{align*}}$ 
### Multiplication matricielle 
![[image multiplication de matrices.png|300]] 
Soit $A=(a_{ik})_{\begin{align*}  1 \leq i \leq n \\ 1 \leq k \leq p \end{align*}}$ et $B=(b_{kj})_{\begin{align*}  1 \leq k \leq p \\ 1 \leq j \leq q \end{align*}}$  
- Le nombre de colonnes de $A$ doit être égal au nombre de lignes de $B$. 
- $C=AB=(c_{ij})_{\begin{align*}  1 \leq i \leq n \\ 1 \leq j \leq q \end{align*}}$ 
- $\displaystyle c_{ij}=\sum_{k=1}^{p}a_{ik}b_{kj}$ 
- Les matrices sont distributives et associatives.
- $AB \neq BA$ en général.
### Transposition 
Si $A=(a_{ij})$ alors $A^{T}=(a_{ij}')=(a_{ji})$
- $(A+B)^{T}=A^{T}+B^{T}$,  $(\lambda A)^{T}=\lambda A^{T}$,  $(\lambda A + \mu B)^{T}=\lambda A^{T} + \mu B^{T}$, $(AB)^{T}=B^{T}A^{T}$ 
### Opérations élémentaires 
Chaque opération élémentaire correspond à la multiplication par une matrice particulière. A Gauche pour les lignes, à droite pour les colonnes. 
#### La transposition 
Echange de 2 lignes : $L_{i} \leftrightarrow L_{j}$ ; de 2 colonnes $C_{i} \leftrightarrow C_{j}$ 
#### La transvection 
Pour $\lambda \in \mathbb{K}$ : $L_{i} \leftarrow L_{i}+\lambda L_{j}$  ou  $C_{i} \leftarrow C_{i}+\lambda C_{j}$ 
#### La dilatation 
Pour $\lambda \in \mathbb{K}^{*}$ : $L_{i} \leftarrow \lambda L_{i}$ ou $C_{i} \leftarrow \lambda C_{i}$ 

## Systèmes linéaires 
Soit le système $(S) \Leftrightarrow AX=B$
- Si on trouve le même nombre de rang et de pivot, alors $A^{-1}$ existe.

## Matrices Carrée 
### D'ordre $n$
$\mathcal{M}_{n}(\mathbb{K})$ Est l'ensemble des matrices carrées
- Diagonal si $\forall i \neq j$,  $a_{ij}=0$ 
- Triangulaires supérieurs si $\forall i > j, a_{ij}=0$ 
- Triangulaires inferieurs si $\forall i < j, a_{ij}=0$ 
- Symétriques si $A^{T}=A, a_{ij}= a_{ji}$
- Antisymétriques si $A^{T}=-A$
- Si $AB=BA$ Alors on peut appliquer le [[Sommes#Formules du binôme de Newton|binôme de Newton]].  

## Matrices carres inversibles 
$A$ est inversible si il existe $B$ ; $A \times B = B \times A = I_{n}$
- Chacune des matrices des opérations élémentaires est inversible.
- $A$ est inversible $\Leftrightarrow AX=B$ a une unique solution.