## Variance d'une VADR
Soit $X$ une VA discrète réelle telle que $X^{2}$ est d'espérance finie. 
- Si $X^{2}$ est d'espérance finie, alors $X$ est d'espérance finie.
- La variance et l'écart-type sont des indicateurs de dispersion autour de $E(X)$
### Variance
On appelle variance le réel positif :
$V(X) = E \Big( (X-E(X))^{2} \Big)$
#### Propriétés 
- Formule de Koenig-Huygens : $V(X) = E(X^{2}) - E(X)^{2}$ 
- Une translation d'une VA ne modifie pas sa variance : $V(aX+b) = a^{2}V(X)$ 
### Écart-type
Moyenne des écarts quadratiques de la moyenne. C'est le réel positif :
$\sigma (X) = \sqrt{V(S)}$
- VA réduit : $\displaystyle Y = \frac{X}{\sigma (X)} \implies \sigma (Y) = 1$.
- VA centrée :  $Y = X-E(X) \implies E(Y) = 0$. 
- VA centrée et réduit : $\displaystyle Y = \frac{X-E(X)}{\sigma (X)}$.
### Inégalité Cauchy-Schwarz 
Soit $X$ et $Y$ deux VAD telles que $X^{2}$ et $Y^{2}$ admettent une espérance. 
$\Big( E(XY) \Big) ^{2} \leq E(X^{2}) E(Y^{2})$
### Covariance 
Soient $X,Y$ deux VAD admettent une variance. Alors  $XY$ admet une espérance alors on appelle covariance de $X$ et $Y$ :
$cov(X,Y) = E \Big( (X-E(X)) (Y-E(Y)) \Big) = E(XY) - E(X)E(Y)$ 
- Si $cov(X,Y) = 0$ : $X$ et $Y$ sont décorrélées.
- Si $X$ et $Y$ sont indépendantes  $\Rightarrow cov(X,Y) = 0$ (sous réserve d'existence).  
#### Propriétés 
- Bilinéaire.
- Symétrique.
- Positif : $cov(X,X) = V(X)\geq 0$
### Variance d'une somme 
Soit $X$ et $Y$ deux VA admettant une variance, alors $X+Y$ admet une variance qui est : 
$V(X+T) = V(X)+V(Y) + 2 cov(X,Y)$ 
Pour $n$ VAD on a : 
$\displaystyle  V(X_{1} + X_{2} + \ldots + X_{n}) = \sum _{1\leq i, j\leq n} cov(X_{i}, X_{j}) = \sum_{i=1}^{n} V(X_{i}) +2 \sum_{1\leq i<j\leq n} cov(X_{i}, X_{j})$ 

## Fonction génératrice 
### Définition 
Soit $X$ une VAD ==à valeurs dans== $\mathbb{N}$ .
La fonction génératrice de $X$ (lorsque définie) est :
$\displaystyle G_{X}(t) = E(t^{X}) = \sum_{n=0}^{+\infty } t^{n} P(X=n)$ 
- Le rayon de convergence de  $G_{X}$ est $\geq 1$.
- $G_{X}(1)=1$.
- $X \sim Y \Leftrightarrow G_{X} = G_{Y}$. 
### Fonction génératrices des lois usuelles
#### Loi d'une VA
$\displaystyle P(X=n) = \frac{G_{X}^{(n)}}{n!}$ 
- On peut trouver la loi d'une VA aussi par identification. 
### Lien entre fonction génératrice l'espérance et la variance
Soit $X$ une VAD ==à valeurs dans== $\mathbb{N}$ .
#### Espérance
$X$ admet une espérance $\Leftrightarrow G _{X}$ est dérivable en $1$.
- $G'_{X}(1) = E(X)$
#### Variance
$X$ admet une variance $\Leftrightarrow G_{X}$ est deux fois dérivable en $1$. 
- $G''_{X}(1) = E(X(X-1))$ 
- $V(X) = G''_{X}(1) -  G'_{X}(1) + G_{X}^{'2} (1)$
### Fonction génératrice de la somme de VA indépendantes
Soit $X$ et $Y$ des VAD à valeurs dans $\mathbb{N}$  et indépendantes.
Alors lorsque $G_{X}(t)$ et $G_{Y}(t)$ sont absolument convergentes, pour $|t|< \min(R_{G_{X}}, R_{G_{Y}})$ 
$G_{X+Y} (t)= G_{X}(t) \cdot  G_{Y}(t)$
- Possible pour $n$ VA indépendantes.

## Inégalités probabilistes et loi faible des grands nombres 
### Inégalité de Markov
Soit $X$ une VAD d'espérance finie et ==$X\geq 0$==.
$\displaystyle \forall a>0, \quad \frac{E(X)}{a} \geq P(X\geq a)$ 
### Inégalité de Bienaymé-Tchevychev 
Soit $X$ une VAD admettant une variance. Alors,
$\forall a > 0 , \quad \frac{V(X)}{a^{2}} \geq  P \Big( |X-E(X)| \geq a \Big)$
### Loi faible des grands nombres
Soit $(X_{n})_{n \in \mathbb{N}}$ une suite de VA indépendantes identiquement distribuées de variance finie.
On note $\displaystyle  S_{n}= \sum_{k=1}^{n} X_{k}$ et $m = E(X_{k})$.
$\forall \epsilon \geq 0, \quad \frac{\sigma ^{2}}{n \epsilon ^{2}} \geq P \left( \left| \frac{S_{n}}{n} - m  \right| \geq \epsilon  \right)$

## Astuces 
$P(X<a) = 1- P(X\geq a)$ 
$(X\geq a) = (X=a)\cup (X>a)$
$\implies P(X>a) \leq P(X\geq a)$ 