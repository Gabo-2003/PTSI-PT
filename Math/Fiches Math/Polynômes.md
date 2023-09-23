### Opérations 
- $\displaystyle \lambda A + \mu B = \sum_{n=0}^{+ \infty} (\lambda a_{n}+ \mu b_{n})X^{n}$ 
- $\deg(A+B)\leq \max(\deg(A), \deg(B))$ 
- $\displaystyle AB= \sum_{n=0}^{+ \infty} a_{k} b_{n-k} X^{n}$ 
- $\deg(AB)=\deg(A)+\deg(B)$

## Divisibilité 
### $P$ de $\mathbb{K}[X]$ irréductible si :
 - $\deg(P) \leq 1$
 - Seulement divisible par $1$ et $P$.
### Division euclidienne :
- $\exists (Q,R) \in \mathbb{K}[X]^{2} ; A=BQ+R$
- $\deg(R)<\deg(B)$ 

## Racines
- $a$ de $\mathbb{K}$ racine de $P$ si $\tilde{P}(a)=0$ 
- $P=Q(X-a)-\tilde{P}(a)$ avec $\tilde{P}(a)=0$ 
### Ordre de multiplicité
Le plus grand $m ; (x-a)^{m} / P$ 
### Polynôme scindé
Si il peut se mètre sur la forme de produits de polynômes de degré $1$. 
### Relation entre coefficients et racines 
- $\displaystyle x_{1}+ x_{2}+ \ldots + x_{n} = - \frac{a_{n-1}}{a_{n}}$ 
- $\displaystyle x_{1} x_{2} \ldots x_{n} = (-1)^{n} \frac{a_{0}}{a_{n}}$ 

## Dérivation 
$P=(X-a)^{m}$ 
Si $0 \leq k \leq m$   $P^{(k)}= \frac{m!}{(m-k)!} (X-a)^{m-k}$ 
### Formule de Taylor 
$\displaystyle P = \sum_{k \in \mathbb{N}} \tilde{P}(\alpha) \frac{(X- \alpha)^{k}}{k!}$  
### Formule de Mac-Laurin 
$\displaystyle P= \sum \tilde{P}(0) \frac{X^{k}}{k!}$ 
$a$ racine de $P \Leftrightarrow \tilde{P}(a)=\tilde{P}'(a) = \tilde{P}^{(m-1)}(a)=0$   et  $\tilde{P}^{(m)}(a)=0$ 

## Factorisation en $\mathbb{C}[X]$
- Tout polynôme non-constante de $\mathbb{C}[X]$ admet au moins 1 racine.
- Tout polynôme de $\mathbb{C}[X]$ est scindé.
- Tout polynôme de degré $n \geq 0$ admet exactement $n$ racines.
- Les polynômes irréductibles sont de degré 1. 

## Factorisation en $\mathbb{R}[X]$ 
- Scindé dans $\mathbb{R}[X] \Leftrightarrow$ toutes ses racines sont réels 
- Polynômes irréductibles : $\begin{cases} \text{dégré 1} \\ \text{dégré 2 discriminant négatif} \end{cases}$ 

## Décomposition en éléments simples
- $\displaystyle F(X) = \frac{A(X)}{B(X)} = \frac{B(X)Q(X)+R(X)}{B(X)} = Q(X)+ \frac{R(X)}{B(X)}$ 
- $\displaystyle \alpha_{k}= \frac{A(p_{k})}{B'(p_{k})}$ 