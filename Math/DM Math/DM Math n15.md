**Exercice 1 : Méthode des tangentes de Newton-Raphson**
Soit $f:[a,b] \longrightarrow \mathbb{R}$ une fonction de classe $C^{2}$ sur $[a,b]$ telles que: 
$$f(a)<0 \text{  et  } f(b)>0 , \forall x \in [a,b], \; f'(x)>0 \text{  et  } f''(x)\geq 0.$$

1- 
- $f$ continue sur $[a,b]$
- $f'(x)>0$ sur $[a,b]$ alors $f$ croissante sur cet intervalle
- $f(a)<0 \text{  et  } f(b)>0$ alors $0 \in [f(a), f(b)]$
Donc, d'après le Corollaire du TVI
$\boxed{\exists! \;c \in [a,b] ; \; f(c)=0}$

2-  
Or $f''(x) \geq 0, \; \forall x \in [a,b]$
Par propriété, $\boxed{f \text{  est convexe sur  } [a,b]}$

3- Soit $u \in [c,b]$

a- Soit $\Delta$ la tangente a la courbe $\Gamma$ de $f$ au point $U =(u, f(u))$
On a l'équation de la tangente 
$\begin{align*}\Delta &=f'(u)(x-u) + f(u) \\ &=f'(u)x -uf'(u) +f(u) \end{align*}$

Soit $v$ l'intersection entre $\Delta \text{  et  } Ox$
on a
$\begin{align*}\Delta (v) =0 &\Leftrightarrow f'(u)v -uf'(u) +f(u)= 0 \\ &\Leftrightarrow v=\frac{uf'(u)-f(u)}{f'(u)} \end{align*}$
$\boxed{v=u - \frac{f(u)}{f'(u)}}$

b- On a 
$\begin{align*} v &\leq u \\ \Leftrightarrow \frac{uf'(u)-f(u)}{f'(u)} &\leq u \\ \Leftrightarrow -f(u) &\leq 0 \\ \Leftrightarrow f(u) &\geq 0 \quad \text{C'est qui est toujours vrai}\end{align*}$
Alors $\boxed{v \leq u}$ est vrai

c- On a $\Delta =f'(u)x -uf'(u) +f(u)$

Or $v=\frac{uf'(u)-f(u)}{f'(u)} \Leftrightarrow f'(u)v =uf'(u)-f(u)$
On a 
$\begin{align*}\Delta &=xf'(u) - f'(u)v \\ &= f'(u)(x-v) \end{align*}$

Or $f$ est convexe sur $[a,b]$. Par définition, tous les tangentes a la courbe $\Gamma$ de f entre $[a,b]$ sont en dessous de la courbe. 
Alors 
   $f(x) \geq \Delta$
$\Rightarrow \boxed{f(x) \geq f'(u)(x-v)}$

d- On a $u \in [c,b]$ or $f$ strictement croissante sur cette intervalle
$\Leftrightarrow c \leq u \leq b$
Or $f(v) \geq f'(u)(v-v)$
$\Leftrightarrow f(v) \geq 0$
$\Rightarrow v \geq c$ et $v \leq u$
Alors $c \leq v \leq u \leq b$
$\Rightarrow \boxed{v \in [c, u]}$

4- 
a- On a  
$\begin{align*}f(x) &\geq f'(u)(x-v) \\ \Leftrightarrow v&\geq x -\frac{f(x)}{f'(x)} \end{align*}$
Alors On peut poser la suite 
$\forall n \in \mathbb{N}, \quad x_{n+1}=x_{n} -\frac{f(x_n)}{f'(x_n)}$
Ici $x_{n+1}$ est un valeur possible de $v$, calculé en utilisant le dernier $v$ trouvé. On commence avec $x_{0}=b$ 

b- On étude la monotonie de $x_n$
$x_{n+1}-x_{n}=x_{n} -\frac{f(x_n)}{f'(x_n)} -x_{n}=-\frac{f(x_n)}{f'(x_n)}$
Or $f'(x)>0 \text{  et  } x_{n}$ est une valeur de $v$, alors
$\begin{align*} c &\leq x_{n} \leq u \\ \Rightarrow f(c) &\leq f(x_{n)} \text{  (f croissante)  } \\ \Rightarrow 0 &\leq f(x_{n}) \end{align*}$

Alors $x_{n+1} = -\frac{f(x_n)}{f'(x_{n})}$ est négative, 
donc $\boxed{(x_{n}) \text{  est décroissante}}$ 

5- Or $f$ de classe $C^{2}$ sur $[a,b]$, $f'$ et $f''$ Sont continues sur cette intervalle.
Alors, d'après le théorème des bornes atteintes:
$f'[a,b]=[m1,m2]$ où $\boxed{m1= \underset{[a,b]}\inf(f') \text{  et  } m2= \underset{[a,b]}\sup(f')}$  
De la même manière:
$f''[a,b]=[M1,M2]$ où $\boxed{M1= \underset{[a,b]}\inf(f'') \text{  et  } M2= \underset{[a,b]}\sup(f'')}$  

6- $\forall x \in[a,b], \quad g(x)=(x-c)f'(x)-f(x)$
a- $g$ est dérivable en $[a,b]$ par produit et somme de fonctions dérivable en $[a,b]$.
et $g'(x) = f'(x)+(x-c)f''(x)-f'(x)$
$\boxed{g'(x)=(x-c)f''(x))}$

b- $\forall t \in [c,x_n]$
On a :
$\begin{align*} t &\leq x_{n}\\ \Leftrightarrow t-c &\leq x_{n}-c  \end{align*}$
et aussi: $f''(t) \leq M2$

Alors $f''(t)(t-c) \leq M2 \times(x_{n}-c)$
$\Leftrightarrow \boxed{|g'(t)| \leq M2(x_{n}- c)}$

c- On a :
$\begin{align*}  f''(x_{n}) &\leq M2 \\ f''(x_{n})(x-c) &\leq M2(x-c) \\ g(x_{n}) &\leq M2(x-c)-f(x_{n}) \end{align*}$
Donc d'après le théorème de l'inégalité des accroissements finis :
$\begin{align*} |g(x_{n})-g(c)| &\leq |M2(x-c)-f(x_n)|(x_{n}-c) \\ \Leftrightarrow g(x_{n}) &\leq M2(x-c)^{2}-f(x_{n}) \quad (\text{or  } g(c)=0) \\  \end{align*}$
$\boxed{|g(x_{n})| \leq M2(x-c)^{2}}$

d- 
$x_{n+1} -c = x_{n}-\frac{f(x_n)}{f'(x_{n})} -c =x_{n} \frac{g(x_{n})-(x_{n}-c)f'(x_{n})}{f'(x_{n})}-c$
$x_{n+1} -c = \frac{g(x_{n})}{f'(x_{n})}$
