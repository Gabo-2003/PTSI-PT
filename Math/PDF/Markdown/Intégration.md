- $\displaystyle\int_{a}^{b}f(t)dt = 0$  si $a=0$ 
- $\displaystyle\int_{[a,b]} f \geq 0$ 
- Soit $f(t)\leq g(t)$ alors $\displaystyle \int_{[a,b]}f \leq \int_{[a,b]} g$  si et seulement si les bornes sont dans le bon sens. 
### Valeur moyenne 
$\displaystyle\exists c \in [a,b] ; \quad \frac{1}{b-a}\int_{a}^{b}f(t)dt=f(c)$  

## Approximation d'une intégral
### Sommes de Riemann 
Soit $f$ une fonction continue sur $[a,b]$. On pose :
$\displaystyle G_{n}= \frac{b-a}{n} \sum_{i=0}^{n-1}f(x_{i})$   et   $\displaystyle D_{n}= \frac{b-a}{n} \sum_{i=1}^{n}f(x_{i})$
Ses suites sont convergentes et :
$\displaystyle\lim_{n \to +\infty} G_{n} = \lim_{n \to + \infty} D_{n} = \int_{[a,b]}^{}f$ 
- On a fait $n$ subdivisions de l'intervalle $[a,b]$, alors :
	- $x_{k}=(a+k \frac{b-a}{n})$ 
- Il est possible de trouver la limite des certains suites avec ces sommes. Normalement on a $a=0$  et  $b=1$. 

| Gauche                         | Droite                          |
| ------------------------------ | ------------------------------- |
| ![[image somme de riemann gauche.gif]] | ![[image somme de riemann droite.gif]] |

## Calcule intégral 
### Théorème fondamental de l'analyse
Soit $f$ une fonction continue sur $[a,b]$. 
Soit $\forall x \in[a,b]$, $\displaystyle F(x) = \int_{a}^{x} f(t)dt$.
Alors $F$ est l'unique primitive de $f$ qui s'annule en $a$ :
- $F'(x)=f(x)$
- $\displaystyle \int_{a}^{b} f(t)dt = F(b)- F(a)$ , vrai pour tout primitive de $f$.
### Intégration par partie
Soit $u$ et $v$ deux fonctions de classe $C^{1}$ sur $[a,b]$ : 
$\displaystyle \int_{a}^{b} u'(x)v(x)dx= \Big[ u(x)v(x) \Big]_{b}^{a} - \int_{a }^{b} u(x)v'(x)dx$
### Changement de variable
1. On pose une relation de classe $C^{1}$ entre deux variables.
2. On transforme les bornes de l'intégram.
3. On en déduit l'élément différentielle. 
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