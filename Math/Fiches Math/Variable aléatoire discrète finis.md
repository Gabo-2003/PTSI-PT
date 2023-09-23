
#probabilite 
- Une variable aléatoire est une application qui, à une  résultat $\omega$, associe une nombre $X(\omega)$   $\begin{align*} X : &\Omega \longrightarrow E \\ &\omega \longmapsto X(\omega) \end{align*}$ 
- $X(\omega)$ ensemble de valeurs prises par $X$. 

## Loi de probabilité d'une variable aléatoire
- $P_{x} : P(X(\Omega)) \longrightarrow [0,1]; A \longmapsto P(X \in A)$ 
### Méthode
Trouver $X(\Omega)$ et après trouver $P(X=x_{i})$ 
### Image par une fonction 
$Y=g(x)$ est l'application  $Y: \Omega \longrightarrow \mathbb{R}; \omega \longmapsto g(X(\omega))$ 
#### Trouver la distribution de $Y$
- Déterminer $Y(\Omega)= \{ y_{j} \} = \{ g(x_{i}) \}$. 
- Déterminer $\displaystyle P(Y=y_{j})= \sum_{i \text{  tq  }g(x_{i})=y_{j}} P(X=x_{i})$ 
### Indépendance des variables 
$X \text{  indépendant de  } Y \Leftrightarrow P(X=x_{i}, Y=y_{j})=P(X=x_{i})P(Y=y_{j})$ 
## Esperance 
$\displaystyle E(X)= \sum_{x \in X(\Omega)} x P(X=x)$ 
### Théorème de transfert 
$\displaystyle E(f(X))= \sum_{x \in X(\Omega)}f(x)P(X=x)$ 
- $E(aX+b)=a E(X)+b$  (linéaire)
- Si $X \leq Y$, alors $E(X) \leq E(Y)$  (croissante)
- $X \leq Y$ veut dire  $\forall \omega \in \Omega,  X(\omega) \leq Y(\omega)$ 

## Variance et écart-type
$V(X)=E((X-E(X))^{2})$ 
- $V(X)=E(X^2)-(E(X))^{2}$
- $V(aX+b)=a^{2}V(X)$ 

## Lois discrètes usuelles 
### Variables uniformes 
$X \: \text{  VAR  } ; \begin{cases} X(\Omega)=E=\{ x_{i} \}_{1\leq  i\leq n} \\ \text{et} \\ P(X=x_{i})=\frac{1}{n}  \end{cases}$ 
- On le note $X \sim u(E)$ 
### Loi de Bernoulli 
$X \: \text{  VAR  } ; \begin{cases} X(\Omega)= \{ 0,1\} \\ P(X=1)=p \in ]0,1[ \\P(X=0)=q=1-p \end{cases}$
- $E(X)=p$              $V(X)=pq$ 
- $X \sim B(p)$
### Loi binomiale 
Si on a $n$ expériences indépendantes à 2 issues (Soit "succès " avec $P(\text{"succès"})=p \in]0,1[$, soit "échec"). Si $X$ est la VAR qui compte le nombre de succès, On a alors :
$\displaystyle \begin{cases} X(\Omega)= [[0,n]] \\ \displaystyle P(X=k)= \binom{n}{k}p^{k}q^{n-k} \end{cases}$ 
- $E(X)=np$         $V(X)=npq$ 
- $X \sim \mathcal{B}(n,p)$ 

## Inégalités probabilistes 
### inégalité de Markov
Soit $X$ une VAR positive et $a>0$ 
- $\displaystyle P(X \geq a) \leq \frac{E(X)}{a}$
### Inégalité de Bienaymé-Tchebychev 
$\forall \varepsilon > 0$ 
- $\displaystyle P(|X-E(X)|\geq \varepsilon) \leq \frac{V(X)}{\varepsilon^{2}}$  