#suites
## Suites réelles ou complexes 
### Suites arithmétique géométriques
$(u_{n})_{\mathbb{N}} :  \begin{cases} u_{0} \in \mathbb{R} \text{  ou  } \mathbb{C}  \\ u_{n+1}=a u_{n}+b \quad (1) \end{cases}$
#### Méthode du point fixe :
- On pose $l=al+b \quad (2)$ 
- On fait $(1)-(2) \Leftrightarrow u_{n+1}-l = a(u_{n}-l)$ 
- On pose une suite auxiliaire $v_{n}= u_{n}-l$ 
### Suites récurrentes linéaires d'ordre 2
- $(u_{n})_{\mathbb{N}} : u_{n+2}=a u_{n+1} +b u_{n}$ 
- Equation caractéristique : $\begin{equation*} \tag{K} r^{2}-ar-b=0 \end{equation*}$
- Si $\Delta>0$ : $u_{n} = \lambda r_{1}^{n}+\mu r_{2}^{n}$ 
$\begin{cases} \lambda + \mu = u_{0}  \\ \lambda r_{1} + \mu r_{2} = u_{1} \end{cases}$
- Si $\Delta = 0$ : $u_{n} = (\lambda n + \mu) r_{1}^{n}$ 
$\begin{cases} \mu = u_{0}  \\ (\lambda + \mu) r_{1} = u_{1} \end{cases}$
- Si $\Delta < 0$, $r_{1}= \overline{r_{2}} = \rho e^{i \theta}$ : $u_{n} = \rho^{n}(\lambda \cos(n \theta)+ \mu \sin(n \theta))$   
$\begin{cases} \lambda = u_{0}  \\ \rho(\lambda \cos(\theta)+ \mu \sin(\theta)) = u_{1} \end{cases}$

## Convergence d'une suite 
$(u_{n})_{\mathbb{N}}$ converge vers $l$ si:
$\forall \varepsilon > 0, \exists n_{0} \in \mathbb{N} ; \forall n \geq n_{0},  |u_{n}-l| \leq \varepsilon$ 
### Suites extraites 
Tout suite de la forme $(u_{\varphi(n)})_{\mathbb{N}}$ ($\varphi$ une application croissante).
- Tout suite extraite d'une suite convergente est convergente de même limite. 
- Si une suite possède deux suites extraites qui ne convergent pas vers un même limite, la suite est divergente. 
- Si les suites $u_{2n}$ et $u_{2n+1}$ convergent vers $l$, alors $u_{n}$ convergent vers $l$.

## Limites infinies des suites réelles 
$u_{n}$ tend vers $\pm \infty$ si $\forall A >0, \exists n_{0} \in \mathbb{N}; \forall n \geq n_{0}, u_{n} \leq A$ 
### Méthode pour lever F.I
- $\infty - \infty$ : factoriser par le terme qui croit le plus vite.
- $\frac{\infty}{\infty}$ : factoriser dans le numérateur et dans le dénominateur le terme qui croit le plus vite.
- Différences de $\sqrt{\quad}$ : quantité conjugué.
- $1^{\infty}$ : on utilise $x=e^{\ln(x)}$ 

## Suites réelles et relation d'ordre
### Passage à la limite dans les inégalités :
Soit $u_{n}$ et $v_{n}$ avec $\lim u_{n}=l$ et $\lim v_{n}=l'$, si après un rang $n_{0}$ $u_{n} \leq v_{n}$ alors $l \leq l'$. 
### Théorème de encadrement 
Soit $\lim u_{n} = \lim w_{n}=l$ et après un rang $n_{0}$ on a $u_{n}\leq v_{n}\leq w_{n}$ alors $\lim v_{n} = l$
### Divergence par minoration ou majoration 
Si $\lim u_{n}=+\infty$ et après un rang $n_{0}$ $u_{n} \leq v_{n}$ alors $\lim v_{n}=+\infty$

## Théorèmes de convergences 
### Théorème de limite monotone
- Tout suite croissante majorée converge et $\lim u_{n}=\sup(u_{n})$
- Si $u_{n}$ est croissante et non majorée, $\lim u_{n}= + \infty$ 
### Suites adjacentes 
$u_{n}\leq l \leq v_{n}$
- $u_{n}$ croissante.
- $v_{n}$ décroissante.
- $\lim (v_{n}-u_{n})=0$
- Si $u_{n}$ et $v_{n}$ adjacentes alors ils ont un même limite.

## Etude du suite de la forme $u_{n+1}=f(u_{n})$
- On dit que un intervalle $I$ est stable par $f$ si $\forall x \in I, f(x)\in I$.
- Signe de $u_{n+1}-u_{n}=f(u_{n})-u_{n}$ on pose $g: x \longmapsto f(x)-x$. Alors on a $u_{n+1}-u_{n}=g(u_{n})$ : on étude le signe
- Si $f$ est croissante sur $I$, et si $\forall n \in \mathbb{N}, u_{n} \in I$. Alors $(u_{n})_\mathbb{N}$ est monotone. 
- Soit $u_{n}$ du type $u_{n+1}=f(u_{n})$ où $f$ est continue, si $(u_{n})$ converge, alors sa limite est solution de l'équation $f(x)=x$.