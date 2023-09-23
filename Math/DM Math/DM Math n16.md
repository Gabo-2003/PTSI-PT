Soit $f$ la fonction définie pout tout réel $x \neq 1$ par : $f(x)=\frac{e^{x}}{1-x}$
1- 
a- On a :
- $e^{x}$ de classe $C^{\infty}$ sur $\mathbb{R}$
- $\frac{1}{1-x}$ de classe $C^{\infty}$ sur $\mathbb{R} \setminus \{1\}$
Alors $\boxed{f(x)=\frac{e^{x}}{1-x} \text{  de classe  } C^{\infty} \text{  sur  }\mathbb{R}\setminus \{1\}}$ par quotient de fonctions classe $C^{\infty}$ sur $\mathbb{R}$$

b- On commence par calculer quelque derives de $f$
$$\begin{align*} f(x)&=\frac{e^{x}}{1-x} \\ f'(x)&=\frac{e^{x}-xe^{x}+e^{x}}{(1-x)^{2}}=\frac{e^{x}(2-x)}{(1-x)^{2}} \\ f''(x)&=\frac{(e^{x}(2-x)-e^{x})(1-x)^{2}+e^{x}(2-x)2(1-x)}{(1-x)^{4}} =\frac{e^{x}(1-2x+x^{2}+4-2x)}{(1-x)^{3}} = \frac{e^{x}(x^2-4x+5)}{(1-x)^{3}} \end{align*}$$

Alors il semble que $\forall x \in \mathbb{R}\setminus \{1\}, \forall n \in \mathbb{N} \text{  on a : } \boxed{f^{(n)}(x)=\frac{e^{x}P_{n}(x)}{(1-x)^{n+1}}}$
avec $P_{n}(x)$ une polynôme a coefficient constante.

On le démontre par recurrence :
**Initialisation :** 
pour $n=0, \quad f^{(0)}(x)=f(x) =\frac{e^{x}}{1-x}$
on a donc $P_{0}(x)=1$ ce qui est bien une polynome, donc ça marche.

**Hérédité :** On suppose que $f^{(n)}(x)=\frac{e^{x}P_{n}(x)}{(1-x)^{n+1}}$ est vrai.
On veut démontrer que $f^{(n+1)}(x)=\frac{e^{x}P_{n+1}(x)}{(1-x)^{n+2}}$  est vrai aussi.

$$\begin{align*}(f^{(n)}(x))'&= \frac{(e^{x}P_{n}(x)+e^{x}P'_{n}(x))(1-x)^{n+1}-e^{x}P_{n}(x)(-(n+1)(1-x)^{n})}{(1-x)^{^{2n+2}}} \\ &=\frac{e^{x}(P_{n}(x)+P'_{n}(x))(1-x)+(n+1)P_{n}(x))}{(1-x)^{^{n+2}}} \\ &= \frac{e^{x}(P_{n}(x)(2+n-x)+P'_{n}(x)(1-x))}{(1-x)^{^{n+2}}} \end{align*}$$
Avec $P_{n+1}(x)=P_{n}(x)(2+n-1)+P'_{n}(x))$ une polynôme par somme, produits et dérivé de polynômes

**Conclusion :** $\forall x \in \mathbb{R}\setminus \{1\}, \forall n \in \mathbb{N}$
$$\text{On a :  }\boxed{f^{(n+1)}(x)=\frac{e^{x}P_{n+1}(x)}{(1-x)^{^{n+2}}}}$$
$$\text{avec  } \boxed{P_{n+1}(x)=P_{n}(x)(2+n-x)+P'_{n}(x)(1-x))}$$

c- d'après les questions précédents 
$$\begin{align*} P_{0}(x)&=1 \\ P_{1}(x)&=-x+2 \\ P_{2}(x)&=x^2-4x+5  \end{align*}$$
Le degré le plus haut semble être $\infty$
Le coefficient dominant semble être $1$ et $-1$  

d- On cherche a calculer $P_{n}(1)$
$$\begin{align*}&P_{n+1}(1)=P_{n}(1)(1+n)+P'_{n}(1)(0))\\ \Leftrightarrow& P_{n+1}(1)=(n+1)P_{n}(1) \end{align*}$$$$ \Leftrightarrow \boxed{P_{n}(1)=\frac{P_{n+1}(1)}{n+1}}$$

2- 
a- $\forall x \neq 1$
$$\begin{align*} (x-1)f'(x)-(x-2)f(x)&= (x-1)\frac{e^{x}(2-x)}{(1-x)^{2}} -(x-2)\frac{e^{x}}{1-x} \\ &= \frac{e^{x}(2-x)}{-(1-x)} +\frac{(2-x)e^{x}}{1-x} =0 \end{align*}$$

$$\Leftrightarrow \boxed{(x-1)f'(x)-(x-2)f(x)=0}$$

b- **Formule de Leibniz**
Soit $n$ un entier naturel et soit $f$ et $g$ deux fonctions de classe $C^{n}$ Sur $I$. Alors $f \times g$ es de classe $C^{n}$ sur $I$ et :
$$(fg)^{n}=\sum_{k=0}^{n}\binom{n}{k}f^{(k)}g^{(n-k)} =\sum_{k=0}^{n}\binom{n}{k}f^{(n-k)}g^{(k)}$$

c- On veut montrer que $\forall x \in \mathbb{R}, \forall n \in \mathbb{N}^{*}$ 
$P_{n+1}(x)=(n+2-x)P_{n}(x)+n(x-1)P_{n-1}(x)$
On le fera par recurrence
**Initialisation :**
pour $n=1$ : 
$\begin{align*}P_{2}(x)&=(3-x)P_{1}(x)+(x-1)P_{0}(x)=(3-x)(2-x)+(x-1)\\ &= x^{2}-4x+5 \text{  ça marche}\end{align*}$ 

**Hérédité :** On suppose que $P_{n+1}(x)=(n+2-x)P_{n}(x)+n(x-1)P_{n-1}(x)$ est vrai
On veut démontrer que $P_{n+2}(x)=(n+3-x)P_{n+1}(x)+(n+1)(x-1)P_{n}(x)$ est vrai aussi

$$\begin{align*} &P_{n+1}(x)=(n+2-x)P_{n}(x)+n(x-1)P_{n-1}(x) \\ \Leftrightarrow& P_{n+1}(x)(n+3-x)=(n+3-x)((n+2-x)P_{n}(x)+n(x-1)P_{n-1}(x)) \\ \Leftrightarrow& P_{n+2}(x)=(n+3-x)((n+2-x)P_{n}(x)+n(x-1)P_{n-1}(x))+(n+1)(x-1)P_{n}(x) \\ \Leftrightarrow& P_{n+2}(x)=(n+3-x)P_{n+1}(x)+(n+1)(x-1)P_{n}(x) \end{align*}$$

**Conclusion :** On a prouve que $\forall x \in \mathbb{R}, \forall n \in \mathbb{N}^{*}$ 
$\boxed{P_{n+1}(x)=(n+2-x)P_{n}(x)+n(x-1)P_{n-1}(x)}$

d- On  a $P_{n+1}(x)=P_{n}(x)(2+n-1)+P'_{n}(x))$
          et $P_{n+1}(x)=P_{n}(x)(2+n-1)+n(x-1)P_{n-1}(x))$
Alors
$$\begin{align*} &P_{n}(x)(2+n-1)+n(x-1)P_{n-1}(x))=P_{n}(x)(2+n-1)+P'_{n}(x)) \\ \Leftrightarrow& (1-x)P'_{n}(x) = n(x-1)P_{n-1}(x)=-n(1-x)P_{n-1}(x) \\ \Leftrightarrow& \boxed{P'_{n}(x)= -nP_{n-1}(x)} \end{align*}$$

3- On commence par calculer $f^{(n)}$ sur $\mathbb{R}\setminus \{1\}$ avec la formule de Leibniz
Soit $f(x)=u(x)\times v(x)$

$\begin{align*} \text{  avec :  }u(x)&=e^{x} \\ u'(x)&=e^{x}\\ u^{(n)}(x)&= e^{x} \end{align*}$ 

$\begin{align*} \text{  et  } v(x)&=\frac{1}{1-x}=(1-x)^{-1} \\ v'(x)&=-1 \times -1 (1-x)^{-2}=(1-x)^{-2} \\ v''(x)&=2(1-x)^{-3} \\ v'''(x)&=2\times 3(1-x)^{-4}, \text{alors} \\ v^{(n)}(x)&=n!(1-x)^{-n-1} \text{  par recurrence} \end{align*}$

Or $v$ et $u$ deux fonctions de classe $C^{n}$ sur $\mathbb{R} \setminus 1$
On a :
$$\begin{align*} f^{(n)}&=(uv)^{(n)}=\sum_{k=0}^{n}\binom{n}{k}v^{(k)}u^{(n-k)}=\sum_{k=0}^{n}\binom{n}{k}k!(1-x)^{-k-1}e^{x} \\ &=e^{x}\sum_{k=0}^{n}\binom{n}{k} \frac{k!}{(1-x)^{k+1}} \end{align*}$$

D'apres $f^{(n)}(x)=\frac{e^{x}P_{n}(x)}{(1-x)^{n+1}}$, on a :

$$\begin{align*} \Leftrightarrow& \; e^{x}\sum_{k=0}^{n}\binom{n}{k} \frac{k!}{(1-x)^{k+1}}=\frac{e^{x}P_{n}(x)}{(1-x)^{n+1}} \\ \Leftrightarrow& P_{n}(x)= \sum_{k=0}^{n} \frac{n!}{k!(n-k)!} \frac{k!}{(1-x)^{k+1}} (1-x)^{n+1} = n!\sum_{k=0}^{n}  \frac{(1-x)^{n-k}}{(n-k)!} \end{align*}$$
$$\boxed{\Leftrightarrow P_{n}(x)=n!\sum_{k=0}^{n}  \frac{(1-x)^{k}}{k!}, \forall x \in \mathbb{R}, \forall n \in \mathbb{N}}$$





