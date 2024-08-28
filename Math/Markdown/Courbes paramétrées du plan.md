## Fonctions vectorielles à valeurs dans $\mathbb{R}$ 
### Limite et continuité 
Soit $f:I \subset \mathbb{R} \longrightarrow \mathbb{R}^{n} ; \quad \underbrace{t}_{\text{réel}} \longrightarrow \underbrace{f(t)}_{\text{vecteur}}= (\underbrace{f_{1}(t), f_{2}(t), \ldots,f_{n}(t)}_{n \text{  coordonnées}})$

Soit $a \in I$. $f$ admet pour limite le vecteur $l\in   \mathbb{R}^{n}$ en $a$ si :
$\forall \epsilon >0, \exists \eta >0; \quad \forall t \in [a-\eta, a+\eta]\cap I$
$\lVert f(t)-l \rVert \leq \epsilon$. On note $l = \lim_{t \to a} f(t)$ 
- $f$ tend vers $l$ en  $\displaystyle a \Leftrightarrow \forall i \in [[1,n]], \quad \lim_{t \to a} f_{i}(t)= l_{i}$. 
- $f$ continue en  $\displaystyle a \Leftrightarrow \forall i \in [[1,n]], f_{i}$ continue en $a$.  
- $f$ continu en $\displaystyle I \Leftrightarrow \forall i \in [[1,n]], f_{i}$ continue en $I$.
### Vecteur dérivée 
$f$ dérivable en  $a$ si $\displaystyle t \mapsto \frac{1}{t-a}(f(t)-f(a))$ a une limite en $a$.
$f$ dérivable en $a$ si $\forall t \in [  [1,n]], f_{i}$ est dérivable en $a$. 
- Dans ce cas  $f'(a) = (f_{1}'(a), f_{2}'(a) , \ldots, f_{n}'(a))$ 
### Fonctions vectorielles de classe $C^{k}$
- $f$ de classe $C^{k}$ en $\displaystyle I \Leftrightarrow \forall i \in [[1,n]], f_{i}$ est de classe $C^{k}$ sur $I$. 
- Dans ce cas  $f^{(k)}(a) = (f_{1}^{(k)}(a), f^{(k)}_{2}(a) , \ldots, f^{(k)}_{n}(a))$ 
### Opérations sur les dérivées 
Soit $f$ une fonction vectoriel et $\alpha$ une fonction scalaire. Si les deux sont dérivables sur $I$ :
-  $(\alpha f)'(t)=\alpha '(t)f(t)+\alpha (t)f'(t)$
Et si les deux de classe $C^{k}$ : 
- $\displaystyle(\alpha f)^{(n)}(t) = \sum_{k=0}^{n} \begin{pmatrix} n \\ k \end{pmatrix} \alpha ^{(k)}f^{(n-k)}$
Si $f$ et $g$ sont les deux fonctions vectorielles, alors on note  $(x|y)$ le produit scalaire de deux vecteurs de $\mathbb{R}^{n}$.
- $\forall t \in  I, \quad (f(t)|g(t))'=(f'(t)|g(t)) + ( f(t)|g'(t) )$
- $(f(t)\wedge g(t))'=f'(t)g(t)+f(t)g'(t)$
### Formule de Taylor-Young 
Soit $p \in \mathbb{N}^{*}$. $f$ fonction vectoriel de classe $C^{p}$ sur $I \subset \mathbb{R}$, alors $\forall t \in  I, \exists$ une fonction vectoriel $\epsilon : I \longrightarrow \mathbb{R}^{n}$ telle que : 
- $\displaystyle\forall t \in  I, \quad f(t)= \sum_{k=0}^{p} \frac{(t-a)^{k}}{k!} f^{(k)}(a)+(t-a)^{p} \epsilon (t-a)$

## Courbes paramétrées du plan et de l'espace 
### Courbes paramétrées 
On appelle courbe paramétrée de classe $C^{k}$ une couple $(I,f)$ avec $f: I \subset \mathbb{R} \longrightarrow \mathbb{R}^{n}$ une application $C^{k}$ sur $I$. 
- Le point $f(t_{0})$ est dit régulière si $f'(t_{0}) \neq 0$, sinon il est dit singulier.
### Tangentes 
Soit $(f,I)$ une courbe paramétrée de classe $C^{k}$, $k\geq 1$ et $t_{0} \in  I$. Si $\exists$ un vecteur unitaire $\overrightarrow{u(t)} ; \forall t \in  I, \overrightarrow{u(t)}$ dirige la corde $[M(t_{0}), M(t)]$ et si $\displaystyle\lim_{t \to t_{0}} \overrightarrow{u(t)} \neq 0$. Alors la courbe $t\mapsto M(t)$ à une tangente en $M(t_{0})$  dirigée par $\displaystyle\lim_{t \to t_{0}}  \overrightarrow{u(t)}$ 
- Si $M(t_{0})$ est un point régulière, la courbe à une tangente en $M(t_{0})$ dirigée par $f'(t_{0})$. 
- La tangente au point $M(t_{0})$ à la courbe à pour équation : 
$\begin{vmatrix} x-x(t_{0}) & x'(t_{0}) \\ y - y(t_{0})  & y'(t_{0})  \end{vmatrix} =0\Leftrightarrow y'(t_{0}) (x-x(t_{0})) - x'(t_{0})(y-y(t_{0}))=0$ 
### Orientation d'une courbe 
- Avec une vecteur unitaire dirigeant la tangente.
- Pour $t$ croissante ou $t$ décroissante.

## Étude des courbes paramétrées planes 
Soit la courbe paramétrée $(I,f)$ avec $\forall t \in  I$, $f(t) = (x(t), y(t))$ de classe $C^{k}$ sur $I$ et  $k\geq 1$. 
### Réduction du domaine d'étude 
On cherche une transformation du temps et une transformation géométrique 
#### Exemples de transformation du temps 
$t \mapsto t+ T$ : Translation du temps
$t \mapsto -t$ : Symétrie par rapport au temps $t=0$
$t \mapsto b-t$ : Symétrie par rapport à $\frac{b}{2}$ 
$t \mapsto \frac{1}{t}$ : inversion 
#### Exemples de transformations géométriques 
$(x,y)\mapsto(-x,y)$ : Symétrie par rapport à $Oy$
$(x,y) \mapsto (x,-y)$ Symétrie par rapport à $Ox$ 
$(x,y)\mapsto(-x,-y)$ : Rotation de $\pi$ autour de $O$
$(x,y)\mapsto(y,-x)$ : Rotation de $-\frac{\pi}{2}$ autour de $O$
$(x,y)\mapsto(-y,x)$ : Rotation de $\frac{\pi}{2}$ autour de $O$
$(x,y)\mapsto(y,x)$ : Symétrie par rapport à $y=x$
$(x,y)\mapsto(x,y)$ : Translation identité
$(x,y)\mapsto(x+a,y+b)$ : Translation de vecteur $(a,b)$ 
$(x,y)\mapsto(a-x,y)$ : Symétrie par rapport à $x= \frac{a}{2}$ 
### Plan d'étude et tracé du support 
- Déterminer le domaine de définition de $f$ est sa classe.
- Réduire l'intervalle d'étude.
- Dresser le tableau de variations.
- Dessiner la courbe.
### Étude locale de la courbe
1- Si $\displaystyle \lim_{t \to t_{0}}  \frac{y(t)-y(t_{0})}{x(t)-x(t_{0})} = m \in \overline{\mathbb{R}}$ alors $(I,f)$ admet une tangente de pente $m$ en  $M(t_{0})$.
2- Dé même pour $\displaystyle \lim_{ t \to t_{0}}  \frac{y'(t)}{x'(t)} = m \in \overline{\mathbb{R}}$.
3- Si la vitesse est nulle : $(x'(t_{0}), y'(t_{0}))=0$ et l'acceleration est non nulle en $t_{0}$. La courbe admet une tangente dirigée par l'accélération. 
4- Si $f$ est de classe  $C^{k}$, on peut écrire un DL de $f$ au voisinage de $t_{0}$ à l'ordre $q\leq k$ 
	- Avec $p$ le plus petite entière telle que $f^{(p)}(t_{0}) \neq 0$
	- Avec $q$ le plus petite entière telle que $p<q$, $f^{(q)}(t_{0})$ n'est pas colinéaire à $f^{(p)}(t_{0})$
![[image etude point local.png]]
- $p$ paire se mantiene del lado de $p$.
- $q$ paire se mantiene pegadito a $q$.
### Étude des branches infinies
![[image etude des branches infinies.png]]