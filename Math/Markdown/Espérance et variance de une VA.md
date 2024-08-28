## Espérance d'une VA discrète réelle 
$E(X)$ est un indicateur de de position de la VA $X$
### Variable aléatoire d'espérance finie
Soit $X$ une VA discrète sur $(\Omega, \mathcal{A} )$.
On a l'énumération $X(\Omega ) = \{ x_{n} \setminus n \in \mathbb{N} \}$.
On dit que $X$ admet une espérance lorsque $\displaystyle \sum _{n \in \mathbb{N}} x_{n} P(X=x_{n})$ converge ==absolument==.
Alors l'espérance de $X$ est : $\displaystyle E(x) = \sum_{n=0}^{+\infty } x_{n}P(X= x_{n})$. 
- La convergence absolue est nécessaire pourque l'espérance ne dépende pas de l'énumération de $X(\Omega )$`
### Formule de transfert 
Soit la VA $f(X)$, elle a une espérance si la série $\displaystyle  \sum _{n \in \mathbb{N}} f(x_{n}) P(X=x_{n})$ est absolument convergente. Dans ce cas :
- $\displaystyle E(f(X)) = \sum_{n=0}^{+\infty } f(x_{n})P(X=x_{n})$
#### Pour un couple 
Soit la VA $g(X,Y)$, on énumère $X(\Omega ) \times  Y(\Omega ) = \{ (u_{n}, v_{n}) \setminus n \in \mathbb{N} \}$. Alors :
- $\displaystyle  E(g(X,Y)) = \sum_{n=0}^{+\infty } g(u_{n}, v_{n})P(X=u_{n}, Y = v_{n})$
### Propriétés 
- L'espérance est linéaire : $E(aX+bY) = aE(X) + b E(Y)$.
- Si $E(x) = 0$, alors $X$ est centrée.
- Si $X$ est à valeurs positifs, $E(X)\geq 0$.
- L'espérance est croissante. 
- Si $X$ et $Y$ sont indépendantes et admettent des espérances, alors : $E(XY) = E(X) E(Y)$

## Variance d'une VADR
Soit $X$ une VA discrète réelle telle que $X^{2}$ est d'espérance finie, alors $X$ admet une variance.  
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
$\sigma (X) = \sqrt{V(X)}$
- VA réduit : $\displaystyle Y = \frac{X}{\sigma (X)} \implies \sigma (Y) = 1$.
- VA centrée :  $Y = X-E(X) \implies E(Y) = 0$. 
- VA centrée et réduit : $\displaystyle Y = \frac{X-E(X)}{\sigma (X)}$.
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
$V(X+Y) = V(X)+V(Y) + 2 cov(X,Y)$ 
Pour $n$ VAD on a : 
$\displaystyle  V(X_{1} + X_{2} + \ldots + X_{n}) = \sum _{1\leq i, j\leq n} cov(X_{i}, X_{j}) = \sum_{i=1}^{n} V(X_{i}) +2 \sum_{1\leq i<j\leq n} cov(X_{i}, X_{j})$ 