#probabilite 
## Couple de VAR
Un couple de variables aléatoires est une variable aléatoire. 
### Loi d'une couple 
$P(X=x_{i},Y=y_{j}) = P_{ij}$ 
#### Méthode 
1- Déterminer l'ensemble de valeurs prises par $X$ et $Y$. 
2- Calculer $P_{ij}$.

| $X / Y$          | $0$ | $1$ | Distribution $X$ |
| ---------------- | --- | --- | ---------------- |
| $0$              |     |     |                  |
| $1$              |     |     |                  |
| Distribution $Y$ |     |     | $1$                 |
#### Lois marginales 
C'est les lois de probabilité des variables $X$ et $Y$. 
- $\displaystyle P(X=x_{i})= \sum_{j \in J} P(X=x_{i},Y=y_{j})$ 
- $P(Y=y_{j})= \sum_{i \in I} P(X=x_{i}, Y=y_{j})$ 

## Independence 
- $X$ indépendante de $Y \Leftrightarrow P(X=x_{i}, Y=y_{j})=P(X=x_{i}) \cdot P(Y=y_{j})$ 
- Si $X$ et $Y$ indépendantes et $f$ définie sur $X(\Omega)$ et $g$ définie sur $Y(\Omega)$, $f(x)$ et $g(x)$ indépendantes.
- Si $X_{1}, X_{2}, \ldots, X_{n}$ mutuellement indépendantes et $\sim \mathcal{B}(p,n)$, alors $X_{1} + X_{2} + \ldots + X_{n} \sim \mathcal{B}(p,n)$ 

## Esperance 
$\displaystyle E(X,Y)= \sum_{i \in I} \sum_{j \in J} x_{i} y_{j} P(X=x_{i}, Y=y_{j})$ 
- Le [[Variable aléatoire discrète finis#Théorème de transfert|théorème de transfert]] se généralise. 
- Si $X$ indépendante de $Y$, $E(X \cdot Y )=E(X) \cdot E(Y)$ 

## Covariance 
- $cov(X,Y)=E((X-E(X))(Y-E(Y))) = E(X \cdot Y)-E(X) \cdot E(Y)$
- Si $X$ indépendante de $Y$, $cov(X,Y)=0$
- $V(X+Y)=V(X)+V(Y)+2\:cov(X,Y)$ 
- Si $X_{1}, \ldots, X_{n}$ indépendantes : $\displaystyle V\left(\sum_{i=1}^{n} X_{i}\right)= \sum_{i=1}^{n}V(X_{i})$  