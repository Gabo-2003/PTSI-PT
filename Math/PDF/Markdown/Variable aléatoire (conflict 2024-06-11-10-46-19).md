#probabilite 

## Variables aléatoires discrètes 
![[image VAD.png|400]]
Soit $(\Omega, \mathcal{A})$ un espace probabilisable, $E$ quelconque. Une VAD est une application de la forme : 
$$\begin{align*} X : &\Omega \longrightarrow E \\  x &\longmapsto X(x) \end{align*}$$
- Si $E \subset \mathbb{R}$ : $X$  est une VA discrète réelle.
- Si $X(\Omega)$ fini : $X$ est une VA finie.
- $X(\omega)$ ensemble de valeurs prises par $X$. Il doit être au plus dénombrable
- $X^{-1}(\{ x \}) \in \mathcal{A}$ signifie que $X^{-1}(\{ x \}) = (X=x)$ est un événement.
### Image d'une VA par une fonction
Soit une fonction $f : E \longrightarrow F$ avec $F$ quelconque.
Alors $f \circ X$ est une VAD. On la note $f(X)$.

## Loi d'une VA discrète
### Probabilité
Si $X$ est une VAD sur $(\Omega, \mathcal{A})$. Alors l'applicaton 
$$\begin{align*}  P_{x} : P(X(\Omega)) &\longrightarrow [0,1]  \\ A &\longmapsto P(X \in A)\end{align*}$$
est une probabilité appelle loi de $X$. 
- $\displaystyle \forall A \subset X(\Omega), \; P_{X}(A) = P(X \in A)= \sum_{x \in A}P(X=x)$
- La famille $(\{ X=x \})_{x \in X(\Omega)}$ est une système complete d'événements. 

## Lois usuelles 
### Lois finies
#### Loi uniforme 
$X \sim \mathcal{U}([[1,n]])$   si :
- $X(\Omega) = [[1,n]]$ 
- $\forall k \in [[1,n]]$,  $P(X=x) = \frac{1}{n}$ 
Espérance : $\displaystyle E(X) = \frac{n+1}{2}$
Variance  : $\displaystyle V(X) = \frac{n^{2}-1}{12}$ 
#### Loi de Bernoulli 
$X \sim \mathcal{B}(p)$ si :
- $X(\Omega) = \{0,1 \}$
- $\displaystyle P(X=1) = p$
Espérance : $E(X)=p$              
Variance : $V(X)=pq$ 
#### Loi binomiale 
Si on a $n$ expériences indépendantes à 2 issues : soit "succès ", avec $P(\text{"succès"})=p \in]0,1[$, soit "échec"). Si $X$ est la VAR qui compte le nombre de succès, alors $X \sim \mathcal{B}(n,p)$  :
$\displaystyle \begin{cases} X(\Omega)= [[0,n]] \\ \displaystyle P(X=k)= \binom{n}{k}p^{k}q^{n-k} \end{cases}$ 
Espérance : $E(X)=np$         
Variance : $V(X)=npq$ 
### Loi géométrique 
Si $X$ est le temps d'attend du première succcès d'une épreuve à 2 issues de probabilité de succès $p$. Alors $X \sim \mathcal{G}(p)$. 
Soit $p \in ]0,1[$, $X \sim \mathcal{G}(p)$ si :
- $X(\Omega) = \mathbb{N}^{*}$  
- $\forall k \in \mathbb{N}^{*}$, $P(X=k) = p(1-p)^{k-1}$ 
Espérance : $E(X) = \frac{1}{p}$
Variance : $V(X) = \frac{q}{p^{2}}$ 
### Loi de Poisson
Soit $\lambda >0$,  $X \sim \mathcal{P}(p)$ si :
- $X(\Omega) = \mathbb{N}$
- $\forall k \in \mathbb{N}$,   $\displaystyle P(X=k) = e^{-\lambda} \frac{\lambda^{k}}{k!}$ 
Espérance : $E(X) = \lambda$ 
Variance : $V(X) = \lambda$
## Couples de variables aléatoires discrètes
### Définition  
Soit $X,Y$ deux VA discrètes sur  $(\Omega , \mathcal{A})$.
Alors l'application $Z : \omega \longrightarrow	(X(\omega ), Y(\omega ))$ est une VA discrète. 
#### Image par une fonction 
Soit :
- $X : \Omega \longrightarrow E$
- $Y : \Omega \longrightarrow F$ 
deux VA discrètes.
Soit $f : E \times  F \longrightarrow G$ une fonction. 
Alors $f(X,Y) : \omega \longmapsto f(X(\omega ) , Y(\omega ))$ est une VA discrète. 
- Valable pour $n$ variables aléatoires.
### Loi conjointe
$P(X = x , Y = y) = P( (X=x) \cap (Y=y) )$
### Lois marginales
$\displaystyle  P(X=n) = \sum_{y \in Y(\Omega )} P( (X=n), (Y=y)) =  \sum_{y \in Y(\Omega )} P(Y=y)P_{(Y=y)}(X=n)$
- C'est la formule de probabilité totale. 
### Loi conditionnelle 

### Covariance 
- $cov(X,Y)=E((X-E(X))(Y-E(Y))) = E(X \cdot Y)-E(X) \cdot E(Y)$
- Si $X$ indépendante de $Y$, $cov(X,Y)=0$
- $V(X+Y)=V(X)+V(Y)+2\:cov(X,Y)$ 
- Si $X_{1}, \ldots, X_{n}$ indépendantes : $\displaystyle V\left(\sum_{i=1}^{n} X_{i}\right)= \sum_{i=1}^{n}V(X_{i})$  

## Variables aléatoires indépendantes 
### indépendance de VA discrètes
Soit $X$, $Y$ deux VA discrètes sur $(\Omega , \mathcal{A})$.
On dit que $X$ et $Y$ sont indépendantes si :
$\forall A \subset X(\Omega ), \forall B \in Y(\Omega ), \quad P( (X \in A) \cap (Y\in B) ) = P(X \in A) \cdot  P(Y \in B)$
- Dans ce cas, soit $f$ et $g$ définies sur $X(\Omega )$ et $Y(\Omega )$ respectivement, alors $f(X)$ et $g(Y)$ sont indépendantes. 
- On peut faire l'extension pour $n$ variables.
### Lemme de coalitions 
Soit $X_{1}, X_{2}, \ldots, X_{n}$ des VA discrètes indépendantes sur $(\Omega , \mathcal{A})$. Alors les variables aléatoires de la forme :
$f(X_{1}, \ldots, X_{p}), g(X_{p}, \ldots, X_{n})$ sont indépendantes.
### Suite de variables aléatoires indépendantes 
Soit $(\Omega , \mathcal{A}, P )$ et $(X_{n})_{n \in \mathbb{N}}$ une suite de VA discrètes de $\Omega$ dans $(E_{n})_{n \in \mathbb{N}}$. 
Les variables $(X_{n})$ sont indépendantes lorsque tout sous-famille finie extrait de  cette suite est une famille de variables aléatoires indépendantes.

## Espérance d'une VA discrète réelle 
$E(X)$ est un indicateur de de position de la VA $X$
### Variable aléatoire d'espérance finie
Soit $X$ une VA discrète sur $(\Omega, \mathcal{A} )$.
On a l'énumération $X(\Omega ) = \{ x_{n} \setminus n \in \mathbb{N} \}$.
On dit que $X$ admet une espérance lorsque $\displaystyle \sum _{n \in \mathbb{N}} x_{n} P(X=x_{n})$ converge ==absolument==.
Alors l'espérance de $X$ est : $\displaystyle E(x) = \sum_{n=0}^{+\infty } x_{n}P(X= x_{n})$. 
`La convergence absolue est nécessaire pour que l'espérance ne dépende pas de l'énumération de $X(\Omega )$`
### Formule de transfert 
Soit la VA $f(X)$, elle a une espérance si la série $\displaystyle  \sum _{n \in \mathbb{N}} f(x_{n}) P(X=x_{n})$ est absolument convergente. Dans ce cas :
- $\displaystyle E(f(X)) = \sum_{n=0}^{+\infty } f(x_{n})P(X=x_{n})$
#### Pour un couple 
Soit la VA $g(X,Y)$, on énumère $X(\Omega ) \times  Y(\Omega ) = \{ (u_{n}, v_{n}) \setminus n \in \mathbb{N} \}$. Alors :
- $\displaystyle  E(g(X,Y)) = \sum_{n=0}^{+\infty } g(u_{n}, v_{n})P(X=u_{n}, Y = v_{n})$
### Propriétés 
- L'espérance est linéaire : $E(aX+bY) = aE(X) + b E(X)$.
- Si $E(x) = 0$, alors $X$ est centrée.
- Si $X$ est à valeurs positifs, $E(X)\geq 0$.
- L'espérance est croissante. 
- Si $X$ et $Y$ sont indépendantes et admettent des espérances, alors : $E(XY) = E(X) E(Y)$

## Variance et écart-type
$V(X)=E((X-E(X))^{2})$ 
- $V(X)=E(X^2)-(E(X))^{2}$
- $V(aX+b)=a^{2}V(X)$ 
## Inégalités probabilistes 
### inégalité de Markov
Soit $X$ une VAR positive et $a>0$ 
- $\displaystyle P(X \geq a) \leq \frac{E(X)}{a}$
### Inégalité de Bienaymé-Tchebychev 
$\forall \varepsilon > 0$ 
- $\displaystyle P(|X-E(X)|\geq \varepsilon) \leq \frac{V(X)}{\varepsilon^{2}}$  