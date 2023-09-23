On définie sur $\mathbb{R}^{*+}$ les fonctions $\begin{align*} f(t)=\frac{\ln(t)}{1+t^{2}} \end{align*}$ et $\begin{align*} F(t)=\int_{1}^{x}f(t)dt \end{align*}$

1-
a- On cherche a déterminer le signe de $F$ sur  $\mathbb{R}^{*+}$
On commence par étudier $f$
$$f(t)=\frac{\ln(t)}{1+t^{2}}$$
- $\forall t \in \mathbb{R}^{*+}$  $1+t^{2} >0$
- $0\leq ln(t) \Leftrightarrow t\geq1$
- $ln(t)<0 \Leftrightarrow t<1$

Alors   $\begin{align*} &f \text{  positive sur  }  [1,+\infty[ \Rightarrow F \text{  positive sur  } [1,+\infty[ \\ &f \text{  négative sur  }  ]0,1[ \Rightarrow F \text{  négative sur  } ]0,1[ \end{align*}$

b- $f$ continue par quotient de fonctions continues sur $\mathbb{R}^{*+}$. Alors d'après le théorème de Darborauk-Riemann, $f$ admet une primitive sur $\mathbb{R}^{*+}$ qu'on note $\phi$
Alors $\forall x>0$
$$F(x)=\int_{1}^{x}f(t)dt=\phi(x)-\phi(1)$$
$$\Rightarrow F'(x)=\phi'(x)=f(x)$$
$$\Rightarrow \boxed{F'(x)=\frac{\ln(t)}{1+t^{2}}}$$

2- $\begin{align*} F(t)=\int_{1}^{x}f(t)dt \end{align*}$  On cherche a faire une changement de variable
- $s=\frac{1}{t} \Leftrightarrow t=\frac{1}{s}$
- Bornes: $\begin{cases} t=x  \\t=1 \end{cases} \Leftrightarrow \begin{cases} s=\frac{1}{x}  \\s=1 \end{cases}$
- Element différentielle: $\begin{align*} t(s)=\frac{1}{s} \Rightarrow t'(s)=-\frac{1}{s^{2}}=\frac{dt}{ds} \Leftrightarrow dt=- \frac{1}{s^{2}}ds \end{align*}$

$$\begin{align*} F(x)=& \int_{1}^{\frac{1}{x}} \frac{\ln(\frac{1}{s})}{1+(\frac{1}{s})^{2}} ds = \int_{1}^{\frac{1}{x}} -\frac{\ln(1)-\ln(s)}{s^{2}+1}ds \\ =&\int_{1}^{\frac{1}{x}} - \frac{-\ln(s)}{s^{2}+1} = \int_{1}^{\frac{1}{x}} \frac{\ln(s)}{s^{2}+1}\end{align*}$$
$$\boxed{F(x)=F(\frac{1}{x})}$$

3- 
a- $\forall x>0 \quad \varphi(x)= \frac{\arctan(x)}{x}$ On veut montrer que $\varphi$ prolongeable par continuité

$$\begin{align*} \varphi(x) \underset{0}= \frac{x- \frac{x^{3}}{3}+ x^{3}\varepsilon(x)}{x}=1-x^{2}+x^{2}\varepsilon(x) \end{align*}$$
Donc $\boxed{\lim_{x \to 0}\varphi(x)=1}$
Alors on peut faire une prolongement par continuité
$$\boxed{\tilde{\varphi}: \mathbb{R}^{+} {\longrightarrow}\mathbb{R} ; t\longmapsto \begin{cases} \varphi(t) \text{  si  } t\neq 0  \\ 1 \text{ si  } t=0 \end{cases}}$$

b- $\begin{align*} F(x)=\int_{1}^{x}\ln(t) \times \frac{1}{1+t^{2}} dt \end{align*}$
$\forall x>0$ on va faire une Intégrale par Parties
$\begin{align*} u(t)&=\ln(t) \hspace{3cm} u'(t)=\frac{1}{t} \\ v(t) &= \arctan(t) \hspace{2cm} v'(t)= \frac{1}{1+t^{2}} \end{align*}$
avec $v$ et $u$ continue pour $x>0$

$$\begin{align*} F(x)=[\arctan(t)\ln(t)]^{x}_{1}-\int_{1}^{x} \arctan\frac{t}{t}dt \end{align*}$$
$$\boxed{F(x)=\arctan(x)- \int_{1}^{x} \arctan\frac{t}{t}dt}$$

c- Or $\varphi(t)$ continue en 0. Alors $\boxed{\int_{1}^{x} \varphi(t)dt \text{  continue en  } 0}$ .
Soit $g(x)=\arctan(x) \ln(x)$
On a $g(x)=(x- \frac{x^{3}}{3}+x^{3}\varepsilon(x))(x- \frac{x^{2}}{2}+ \frac{x^{3}}{3}+x^{3}\varepsilon(x))=x^{2}- \frac{x^{3}}{2} + x^{3}\varepsilon(x)$
Donc $\boxed{\lim_{t \to 0} \arctan(t) \ln(t)=0}$
Donc $F(x)$ prolongeable par continuité en $0$

4- 
a- $\forall k \in \mathbb{N}$ et $x>0$ On a 
$$I_{k}(x)=\int_{1}^{x}t^{k}\ln(t)dt$$
On fait une IPP
$\begin{align*} u(t)&=\ln(t) \hspace{3cm} u'(t)=\frac{1}{t} \\ v(t)&= \frac{1}{k+1}t^{k+1} \hspace{2cm} v'(t)= t^{k} \end{align*}$
$u$ et $v$ continue
$$\begin{align*} I_{k}(x)=[\frac{\ln(t)}{k+1} t^{k+1}]^{x}_{1}- \int_{1}^{x} \frac{t^{k+1}}{(k+1)t}dt =\frac{\ln(x)}{k+1} x^{k+1}- \frac{1}{k+1}(\frac{x^{k+1}}{k+1} - \frac{1}{k+1}) \end{align*}$$
$$\Leftrightarrow \boxed{I_{k}(x)= \frac{\ln(x)}{k+1} x^{k+1} + \frac{1-x^{k+1}}{(k+1)^{2}} }$$

b- On veut démontrer par recurrence que $\forall n \in \mathbb{N}$ et $\forall x>0$ on a 
$$\begin{align*} \frac{1}{1+x^{2}} = \sum_{k=0}^{n}(-1)^{k}x^{2k} \: +(-1)^{n+1} \frac{x^{2n+2}}{1+x^{2}} \end{align*}$$
**Initialisation :** pour $n=0$
$\begin{align*} \frac{1}{1+x^{2}}=1-\frac{x^{2}}{1+x^{2}} = \frac{1+x^{2}-x^{2}}{1+x^{2}} \end{align*}$ ça marche

**Hérédité :** On suppose que $\begin{align*} \frac{1}{1+x^{2}} = \sum_{k=0}^{n}(-1)^{k}x^{2k} \: +(-1)^{n+1} \frac{x^{2n+2}}{1+x^{2}} \end{align*}$ est vrai
On veut démontrer que $\begin{align*} \frac{1}{1+x^{2}} = \sum_{k=0}^{n+1}(-1)^{k}x^{2k} \: +(-1)^{n+2} \frac{x^{2n+4}}{1+x^{2}} \end{align*}$ est vrai aussi.

$$\begin{align*} \frac{1}{1+x^{2}} &= \sum_{k=0}^{n}(-1)^{k}x^{2k} \: +(-1)^{n+1} \frac{x^{2n+2}}{1+x^{2}} = \sum_{k=0}^{n+1}(-1)^{k}x^{2k} \:-(-1)^{n+1} x^{2n+2} +(-1)^{n+1} \frac{x^{2n+2}}{1+x^{2}} \\ &= \sum_{k=0}^{n+1}(-1)^{k}x^{2k} -(-1)^{n+1} \left(x^{2n+2} - \frac{x^{2n+2}}{1+x^{2}}\right)\end{align*}$$
$$\boxed{\frac{1}{1+x^{2}} = \sum_{k=0}^{n+1}(-1)^{k}x^{2k} \: +(-1)^{n+2} \frac{x^{2n+4}}{1+x^{2}} \text{  CQFD}}$$

**Conclusion :** $\forall n \in \mathbb{N}$ et $\forall x>0$ On a 
$$\boxed{\frac{1}{1+x^{2}} = \sum_{k=0}^{n}(-1)^{k}x^{2k} \: +(-1)^{n+1} \frac{x^{2n+2}}{1+x^{2}}}$$