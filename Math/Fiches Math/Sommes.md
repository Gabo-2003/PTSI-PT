#algebre #suites
## Règles de calcul
- $\displaystyle \sum_{k=1}^{n} (a_{k}+b_{k})=\sum_{k=1}^{n} a_{k} +\sum_{k=1}^{n} b_{k}$ 
- $\displaystyle  \sum_{k=1}^{n} \lambda a_{k}=\lambda \sum_{k=1}^{n} a_{k}$ 
- $\displaystyle  \sum_{k=1}^{n} a_{k}\times b_{k} \neq \sum_{k=1}^{n} a_{k} \times \sum_{k=1}^{n} b_{k}$
- $\displaystyle  \frac{1}{\displaystyle  \sum_{k=1}^{n} a_{k}} \neq \sum_{k=1}^{n} \frac{1}{a_{k}}$
### Changement d'indice 
- Ecrire la relation entre les deux indices
- Changer les bornes de sommations
- Changer l'expression contenue dans la somme

## Somme d'une suite arithmétique ou géométrique 
- $\displaystyle \sum_{k=1}^{n} k = \frac{n(n+1)}{2}$
- $\displaystyle \sum_{k=1}^{n} k^{2}=\frac{n(n+1)(2n+1)}{6}$ 
- $\displaystyle\sum_{k=1}^{n} k^{3}= (\frac{n(n+1)}{2})^{2}$ 
- $\displaystyle \forall x \neq 1, \sum_{k=0}^{n} x^{k}=\frac{1-x^{n+1}}{1-x}$ si $x=1$ alors  $\displaystyle \sum_{k=0}^{n} x^{k}=n+1$ 
### Suite arithmétique 
$\begin{cases} u_{n+1}=u_{n}+r \\ u_{n}=u_{0}+nr\end{cases}$ 
- $\displaystyle \sum_{k=0}^{n} u_{k}=(n+1)u_{0}+ \frac{n(n+1)}{2}r= \frac{n+1}{2}(u_{0}+u_{n})$
### Suite géométrique
$\begin{cases} u_{n+1}=u_{n}q \\ u_{n}=u_{0}q^{n}\end{cases}$ 
- $\displaystyle \sum_{k=p}^{n} u_{k}= \frac{u_{p}- u_{n+1}}{1-q}$

## Somme télescopique 
$\displaystyle \sum_{k=0}^{n} f(k+1)-f(k)=f(n+1)-f(0)$

## Somme double
### Somme rectangulaire 
$\displaystyle S=\sum_{i=1}^{n} \sum_{j=1}^{p} a_{i,j}=\sum_{j=1}^{p} \sum_{i=1}^{n} a_{i,j} = \sum_{\underset{1 \leq j \leq p}{1 \leq i \leq n} } a_{i,j}$ 
### Somme triangulaire
$\displaystyle S=\sum_{i=1}^{n} \sum_{j=1}^{i} a_{i,j}= \sum_{1 \leq j \leq i \leq n} a_{i,j}=\sum_{j=1}^{n} \sum_{i=j}^{n} a_{i,j}$
### Produit de deux sommes finies
$\displaystyle \sum_{k=1}^{n} a_{k} \times \sum_{j=1}^{p} b_{j}=\sum_{k=1}^{n} \sum_{j=1}^{p} a_{k}b_{j} =\sum_{j=1}^{p}\sum_{k=1}^{n} a_{k}b_{j}$

## Quelques formules
### Combinaisons 
- $\displaystyle \begin{pmatrix} n \\ p \end{pmatrix} = \frac{n!}{p!(n-p)!}$ 
- $\displaystyle \begin{pmatrix} n \\ 0 \end{pmatrix} =1 , \begin{pmatrix} n \\ 1 \end{pmatrix} =n , \begin{pmatrix} n \\ 2 \end{pmatrix} = \frac{n(n-1)}{2}$ 
- $\begin{pmatrix} n \\ p \end{pmatrix} = \begin{pmatrix} n \\ n-p \end{pmatrix}$ 
- $\begin{pmatrix} n+1 \\ p \end{pmatrix} = \begin{pmatrix} n \\ p \end{pmatrix} + \begin{pmatrix} n  \\ p+1 \end{pmatrix}$ 
### Triangle de Pascal 
![[image triangle de pascal.png|400]]
### Formules du binôme de Newton 
- $(a+b)^{2}=a^{2}+2ab + b^{2}$ 
- $(a+b)^{3}=a^{3}+3a^{2}b + 3ab^{2} + b^{3}$ 
- $\displaystyle (a+b)^{n} = \sum_{k=0}^{n} \begin{pmatrix} k \\ n \end{pmatrix} a^{n-k} b^{k} =\sum_{k=0}^{n} \begin{pmatrix} k \\ n \end{pmatrix} a^{k} b^{n-k} \quad (a,b) \in \mathbb{R}$
### Identité remarquable $a^{n}-b^{n}$ 
- $a^{2}-b^{2}=(a-b)(a+b)$ 
- $a^{3}-b^{3}=(a-b)(a^{2}+ab+b^{2})$ 
- $\displaystyle a^{n}-b^{n}= (a-b)\sum_{k=0}^{n-1} a^{k}b^{n-1-k}$
## Signe produit $\Pi$ 
- $\displaystyle n!=\prod_{k=1}^{n} k$
- $\displaystyle p^{n}=\prod_{k=1}^{n} p$ 
- $\displaystyle \ln(\prod_{k=1}^{n} a_{k})= \sum_{k=1}^{n}\ln(a_{k})$ 
- $\displaystyle \exp(\sum_{k=1}^{n}a_{k})= \prod_{k=1}^{n} \exp(a_{k})$ 
