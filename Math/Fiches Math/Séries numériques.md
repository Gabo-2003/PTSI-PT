#suites 
![[Graph Séries numériques.canvas|Graph Séries numériques]] 
## Séries à termes réels ou complexes
### Définition
- Série de terme général $u_{n}$ :   $(\sum u_{n})$ 
- Somme partielle d'ordre $n$  de la série : $\displaystyle S_{n}= \sum_{k=0}^{n}u_{k}$ 
### Repasser de $S_{n}$ à $u_{n}$
$\begin{cases} u_{0} = S_{0} \\ \forall n \in \mathbb{N}, S_{n} - S_{n-1}=u_{n} \end{cases}$ 
### Convergence 
- $(\sum_{}^{}u_{n})$ convergente si $(S_{n})$ converge. 
- $\displaystyle \forall z \in \mathbb{C}\quad \left(\sum_{}^{} \frac{z^{n}}{n!}\right)$ converge et : $\displaystyle e^{z}=\sum_{n=0}^{+ \infty} \frac{z^{n}}{n!}$ 
#### Somme de la série 
$\displaystyle l= \lim_{n \to + \infty} S_{n} = \lim_{n \to + \infty} \sum_{k=0}^{n} u_{k}= \sum_{k=0}^{+ \infty} u_{k}$ 
### Propriétés 
- $\forall \lambda, \quad (\sum_{}^{}u_{n})$ et $(\sum_{}^{}\lambda u_{n})$ sont de la même nature (convergent ou divergent).
- Si convergentes : 
	- $\displaystyle \sum_{n=0}^{+ \infty} \lambda u_{n}=\lambda \sum_{n=0}^{+ \infty} u_{n}$ 
	- $\displaystyle \sum_{n=0 }^{+ \infty} u_{n} + v_{n}=\sum_{n=0 }^{+ \infty} u_{n} + \sum_{n=0 }^{+ \infty} v_{n}$ 
- Si $(\sum_{}^{}u_{n})$ converge alors $\displaystyle \lim_{n \to + \infty} u_{n} =0$   (réciproque fausse)
- Si $\displaystyle \lim_{n \to + \infty} u_{n} \neq 0$ alors $(\sum_{}^{}u_{n})$ est grossièrement divergente.  
- $(u_{n})$  converge $\Leftrightarrow \sum_{}^{}(u_{n+1}-u_{n})$ converge. 
### Théorème des séries alternes
Soit $( u_{n} )$ une suite réelle, décroissante, convergente vers 0. 
- Alors la série $\sum (-1)^{n} u_{n}$ converge.
## Séries à termes positifs $(\forall n \in \mathbb{N}, u_{n} \geq 0)$ 
- Soit $(\sum_{}^{}u_{n})$ une série à termes positifs, il converge $\Leftrightarrow (S_{n})$ est majorée. 
### Théorème de comparaison des séries à terme positifs
- Si $u_{n} \sim v_{n}$, les deux positives : la convergence de $(\sum_{}^{}v_{n})$ est de même nature que la de $(\sum_{}^{} u_{n})$. 
- Si a partir d'un rang $n_{0}$  $u_{n} \leq  v_{n}$ et si $(\sum_{}^{} v_{n})$ converge alors $(\sum_{}^{} u_{n})$ converge.
- Si $u_{n} \underset{+ \infty } = O(v_{n})$ ou $u_{n} \underset{+ \infty } = o(v_{n})$ et si $\sum v_{n}$ converge, alors $\sum u_{n}$ converge. 
### Comparaison série-intégral 
Soit $f$ continue, positive et décroissante : 
- $\displaystyle \int_{n_{0}}^{n+1} f(t) dt \leq \sum_{k=n_{0}}^{n}f(k) \leq f(n_{0})+ \int_{n_{0}}^{n}f(t)dt$ 
- Majoration pour convergence :
![[image majoration.png|200]]
- Minoration pour divergence :
![[image minoration.png|200]]
### Série de Riemann 
$\displaystyle\left(\sum_{}^{} \frac{1}{n^{\alpha}}\right)$ converge $\Leftrightarrow \alpha >1$ 

## Séries absolument convergentes 
$(\sum_{}^{} u_{n})$ est absolument convergente (est donc convergente) si $(\sum_{}^{}|u_{n}|)$ converge. 
- $(\sum_{}^{}|u_{n}|)$ est une série a terme positive. 
- Si $(\sum_{}^{} u_{n})$ est une série absolument convergente alors $\displaystyle \left| \sum_{n=0}^{+ \infty } u_{n} \right| \leq  \sum_{n=0}^{+ \infty } | u_{n} |$
### Théorème de comparaison 
- Si $u_{n} \underset{+ \infty } = O(v_{n})$ alors la converge absolue de $\sum v_{n}$ implique celle de $\sum u_{n}$. 
- Si a partir d'un rang $n_{0}$  $|u_{n}| \leq  |v_{n}|$ et si $(\sum_{}^{} v_{n})$ converge absolument alors $(\sum_{}^{} u_{n})$ converge absolument.
- Si $u_{n} \sim v_{n}$  la convergence absolue de $(\sum_{}^{}v_{n})$ implique celle de $(\sum_{}^{} u_{n})$. 
### Règle de d'Alembert 
Soit $(u_{n})_{n \in \mathbb{N}}$ une suite réelle ou complexe qui ne s'annule pas. On suppose que la suite $\displaystyle \left| \frac{u_{n+1}}{u_{n}} \right|$ tend vers $l \in \mathbb{R} \cup {+ \infty}$
- Si $l<1$  alors $\sum_{}^{} u_{n}$ converge absolument.
- Si $l>1$  alors $\sum_{}^{} u_{n}$ diverge grossièrement.
### Produit de Cauchy de deux séries absolument convergentes
#### Produit de Cauchy 
Le produit de Cauchy des séries $\sum_{}^{} u_{n}$ et $\sum_{ }^{} v_{n}$ est la série $\sum w_{n}$ où $\forall n \in \mathbb{N}$ 
- $\displaystyle w_{n} = \sum_{n \geq 2}^{} u_{p}v_{p}=\sum_{k=0}^{n}u_{k}v_{n-k}$ 
#### Théorème 
Si les séries à termes réels ou complexes $\sum_{}^{} u_{n}$ et $\sum_{ }^{} v_{n}$ convergent absolument, alors la série produit de Cauchy $\sum w_{n}$ converge absolument et : 
- $\displaystyle \sum_{n=0}^{+ \infty}w_{n}= \left(\sum_{n=0}^{+ \infty}u_{n}\right) \left(\sum_{n=0}^{+ \infty}v_{n}\right)$    