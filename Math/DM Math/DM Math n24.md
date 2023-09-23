**Exercice 1 :** Soit $E=\mathbb{R}_{2}[X]$, On considère 
$$G= \{ P \in E / P(1) \}$$
$$\Phi(P)(X)=2P(X+1)-(X-1)P'(X)$$

1- On veut vérifier aue $G$ est un sous-espace vectoriel de $E$
Soit $D= \alpha X^{2}+ \beta X+\gamma$ avec $(\alpha,\beta, \gamma)\in \mathbb{R}^{3}$

$$\begin{align*} D \in P \Leftrightarrow& D(1)=0 \\ \Leftrightarrow& \alpha + \beta + \gamma =0 \\ \Leftrightarrow& \gamma = -\beta - \alpha \end{align*}$$

Alors $D = \alpha X^{2}+ \beta X - \beta -\alpha = \alpha(X^{2}-1)+ \beta(X-1)$
Donc $\boxed{G = Vect(X^{2}-1,X-1)}$
Alors $G$ est un $s.e.v$ engendré par $u=X^{2}-1$ et $v=X-1$

2- On veut montrer que $\Phi$ est une application linéaire
Soit $(u_{1},u_{2})\in \mathbb{R}^{2}[X]$
$\begin{align*} u_{1}=a_{1}X^{2}+b_{1}X + c_{1} \\ u_{2}=a_{2}X^{2}+b_{2}X + c_{2} \end{align*}$                   et $\lambda \in \mathbb{R}$

$$\begin{align*} \Phi(u_{1}+u_{2}) &= \Phi(X^{2}(a_{1}+a_{2})+X(b_{1}+b_{2})+c_{1}+c_{2}) \\ &= 2((X+1)^{2}(a_{1}+a_{2})+(X+1)(b_{1}+b_{2})+c_{1}+c_{2})-(X-1)(2X(a_{1}+a_{2})+b_{1}+b_{2}) \\ &= 2((X+1)^{2}a_{1}+(X+1)b_{1}+c_{1})-(X-1)(2Xa_{1}+b_{1})\\ &+2((X+1)^{2}a_{2}+(X+1)b_{2}+c_{2})-(X-1)(2Xa_{2}+b_{2}) \\ &= \Phi(u_1)+\Phi(u_{2})  \end{align*}$$

$$\begin{align*} \Phi(\lambda u_{1})&= \Phi(\lambda(a_{1}X^{2}+b_{1}X + c_{1})) \\ &= 2((X+1)^{2}\lambda a_{1}+(X+1)\lambda b_{1}+\lambda c_{1})-(X-1)(2X\lambda a_{1}+\lambda b_{1}) \\ &= \lambda(2((X+1)^{2}a_{1}+(X+1)b_{1}+c_{1})-(X-1)(2Xa_{1}+b_{1})) \\ \lambda \Phi(u_{1}) \end{align*}$$
Donc $\Phi$ est linéaire 
De plus, Soit $P \in E$ tel que 
$$\begin{align*} P(X) &= \alpha X^{2} +\beta X + \gamma \\ P'(X) &= 2\alpha X +\beta \end{align*}$$

Alors  
$$\begin{align*} \Phi(P)(X)&= 2(\alpha(X+1)^{2}+\beta(X+1)+\gamma)-(X-1)(2\alpha X+\beta) \\ &= X(6\alpha+\beta)+2\alpha+2\gamma+3\beta \end{align*}$$
$\Rightarrow deg(\Phi(P)(X))\leq 1$
Alors $\Phi(P)(X) \in E$
Donc $\Phi$ est un endomorphisme de $E$

3- On cherche $ker(\Phi)=F$ sur $E$
$\forall \text{  polynome  } u$ telle que $u = \alpha X^{2}+\beta X+ \gamma$
$u\in ker(\Phi) \Leftrightarrow \Phi(u)=0$
On a $\Phi(u)(x)=X(6\alpha+\beta)+2\alpha+2\gamma+3\beta$
Un polynôme est nul $\Leftrightarrow$ tous ses coefficients sont nulles.
$$\Phi(u)=0 \Leftrightarrow \begin{cases} 6\alpha+\beta=0 \\ 2\alpha+2\gamma+3\beta=0 \end{cases} \Leftrightarrow \begin{cases} \beta=-6\alpha  \\ \gamma=8\alpha \end{cases}$$
Si remplace, alors
$u \in F \Leftrightarrow \exists \lambda \in \mathbb{R} ; u =\lambda(X^{2}-6X+8)$  
Donc $\boxed{F = ker(\Phi)=Vect(X^{2}-6X+8)}$

4- Par propriété, $\Phi$ injective $\Leftrightarrow ker(\Phi)=0$ C'est qui n'est pas le cas. Alors $\Phi$ n'est pas ni injective ni bijective.
Donc $\Phi$ n'est pas une automorphisme 

5- On a $F=Vect(X^{2}-6X+8)$ et $G=Vect(X^{2}-1,X-1)$. On veut montrer $F$ et $G$ sont supplémentaires dans $E$.
Alors $\forall P \in E$, on doit montrer que $\exists P_{F}\in F$ et $\exists P_{G}\in G$ telle que 
$P =P_{F}+P_{G}$  avec $P =\alpha X^{2}+\beta X+ \gamma$
$$P=a(X^{2}-6X+8)+b(X^{2}-1) +c(X-1)$$
$$\begin{align*} \Leftrightarrow  \begin{cases} a+b=\alpha \\ -6a+ c=\beta \\8a-b-c=\gamma \end{cases} \overset{l_{2}\leftarrow l_{2}+ l_{1}}\Leftrightarrow \begin{cases} a+b=\alpha \\2a-b=\beta+\gamma \\8a-b-c=\gamma \end{cases} \overset{l_{2} \leftarrow l_{2}-2l_{1}}\Leftrightarrow \begin{cases}a+b=\alpha \\-3b=\beta+\gamma-2\alpha \\8a-b-c=\gamma  \end{cases}\end{align*}$$
On a trois pivots et trois équations, donc le système admet une unique solution.
Donc, on a bien $\boxed{E=F\oplus G}$

**Exercice 2 :** Soit $E$ l'espace vectoriel des applications de classe $\mathcal{C}^{2}$ sur $\mathbb{R}$ et $F=\{ \Phi \in E\: / \:\forall x \in \mathbb{R}, \: \Phi''(x)=(1+X^{2})\Phi(x)  \}$

1- On veut montrer que $F$ est un sous-espace vectoriel de $E$
- $\Phi \subset E$
- Soit $0_{E}$ l'application nulle on a $0''_{E}(x)=0=(1+X^{2})0_{E}(X)$
Alors $0_{E} \in F \Rightarrow F \neq \emptyset$
- Stabilité de $F$ par combinaison linéaire 
$\forall(u,v)\in F^{2}, \forall(\lambda, \mu)\in \mathbb{R}^{2}$ On a 
$$\begin{cases} u''(x)=(1+x^{2})u(x) \\ v''(x)=(1+x^{2})v(x) \end{cases}$$
$$\begin{align*} \Rightarrow(\lambda u''+\mu v'')&=\lambda u''(x)+\mu v''(x)=\lambda(1+x^{2})u(x)+\mu(1+x^{2})v(x) \\ &= (1+x^{2})(\lambda u(x)+ \mu v(x)) =(1+x^2)(\lambda u + \mu v)(x) \end{align*}$$
Donc $\lambda u''+ \mu v'' \in F$ 

Alors, par définition $F$ est un $s.e.v$ de $E$

2- On pose $\forall x \in \mathbb{R}, \quad f(x)=e^{\frac{x^{2}}{2}} \text{  et  } g(x)=e^{\frac{x^{2}}{2}}\int_{0}^{x}e^{-t^{2}}dt$

a- On veut montrer que $f$ et $g$ appartient à $F$
$f(x)=e^{\frac{x^{2}}{2}}$
$f'(x)=xe^{\frac{x^{2}}{2}}$
$f''(x)=e^{\frac{x^{2}}{2}}+x(xe^{\frac{x^{2}}{2}})=e^{\frac{x^{2}}{2}}(1+x^{2})$
ça marche

$\begin{align*} g(x)=f(x)\int_{0}^{x}e^{-t^{2}}dt \end{align*}$
Or $e^{-t^{2}}$ continue par composé de fonctions continues sur $\mathbb{R}$, D'apres le théorème de Darboraux-Riemman, $e^{-t^{2}}$ admet une primitive sur $\mathbb{R}$ qu'on note $\varphi$
Alors 
$\begin{align*} g(x)=f(x)\int_{0}^{x}\varphi(t) dt=f(x)(\varphi(x)-\varphi(0)) \end{align*}$
$g'(x)=f'(x)(\varphi(x)-\varphi(0))+f(x)\varphi(x)$
$\begin{align*} g''(x)&= f''(x)(\varphi(x)-\varphi(0))+2f'(x)\varphi(x)+f(x)\varphi''(x) \\ &= f(x)(1+x^{2})(\varphi(x)-\varphi(0))+2xe^{\frac{x^{2}}{2}}e^{-2x^{2}}+e^{\frac{x^{2}}{2}}(-2xe^{-x^{2}}) \\ &= (1+x^{2})g(x) \end{align*}$
ça marche
 $f$ et $g$ appartient à $F$
 
b- Montrer que si $u$ et $v$ appartient a $F$, $u'v-v'u$ est constante
$\Leftrightarrow (u'v-v'u)'=0$
On a $(u'v-v'u)'=u''v+u'v'-v''u+v'u'=u''v-uv''=(1+x^{2})u(x)v(x)-u(x)(1+x^{2})v(x)=0$
Donc $u'v-v'u$ est constante $\forall(u,v)\in F^{2}$