#calcul
- $\displaystyle\int_{a}^{b}f(t)dt = 0$  si $a=0$ 
- $\displaystyle\int_{[a,b]} f \geq 0$ 
- Soit $f(t)\leq g(t)$ alors $\displaystyle \int_{[a,b]}f \leq \int_{[a,b]} g$  si et seulement si les bornes sont dans le bon sens. 
### Valeur moyenne 
$\displaystyle\exists c \in [a,b] ; \quad \frac{1}{b-a}\int_{a}^{b}f(t)dt=f(c)$  

## Approximation d'une intégral
### Sommes de Riemann 
- $\displaystyle G_{n}= \frac{b-a}{n} \sum_{i=0}^{n-1}f(x_{i})$ 
- $\displaystyle D_{n}= \frac{b-a}{n} \sum_{i=1}^{n}f(x_{i})$
- $x_{i}=(a+i \frac{b-a}{n})$ 
- normalement $a=0$  et  $b=1$ 

## Calcule intégral 
$\displaystyle\phi : x \longmapsto \int_{a}^{x}f(t)dt$ unique primitive de $f$ qui s'annule en $a$.
$\phi'(x)=f(x)$
### Intégration par partie
$\displaystyle \int_{a}^{b} u'(x)v(x)dx= \Big[ u(x)v(x) \Big]_{b}^{a} - \int_{a }^{b} u(x)v'(x)dx$
### Changement de variable
On pose le changement, bornes, élément différentielle. 
### Périodicité et symétrie 
Si $f$ est paire :  $\displaystyle\int_{-a}^{a}f(t)dt = 2 \int_{0}^{a}f(t)dt$ 
Si $f$ est impaire : $\displaystyle\int_{-a}^{a}f(t)dt=0$ 
Si $f$ de période $T$ : $\begin{cases} \displaystyle\int_{a}^{b} f(t)dt= \int_{a+T}^{b+T}f(t)dt \\  \text{et} \\ \displaystyle \int_{a}^{a+T} f(t) dt = \int_{0}^{T} f(t) dt \end{cases}$ 	
### Inégalité de Taylor-Lagrange 
Soit $P \in \mathbb{N}$, $f$ de classe $C^{p+1}$ sur $I$, $\forall (x,a) \in I^{2}$ 
$M_{p+1}=\sup|f^{(p+1)}(t)|$ 
- $\displaystyle|f(x)- \sum_{k=0}^{p} \frac{(x-a)^{k}}{k!}f^{(k)}(a) | \leq \frac{M_{p+1}|x-a|^{p+1}}{(p+1)!}$ 

## Extension au valeurs complexes
$\displaystyle \int_{[a,b]} f =\int_{[a,b]} Re(f)+ i \int_{[a,b]} Im(f)$ 