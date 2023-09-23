
## L'espace $\mathbb{R}^{2}$ 
$\forall u =(x,y), \quad \forall u'=(x',y')$ 
### Produit scalaire 
$u \cdot v =xx'+yy'$ 
### Norme : 
$\| u \|=\sqrt{x^{2}+y^{2}}$ 
### Distance 
$d(u,v)= \| v-u \|=\sqrt{(x'-x)^{2}+(y'-y)^{2}}$ 
### Boule ouverte
Soit $u$ un  vecteur et $r$ un réel positif.
Boule ouverte de centre $u$ et rayon $r$ : $\mathcal{B}(u,r)= \{ v \in \mathbb{R}^{2} \frac{}{ d(u,v)}< r \}$ 
![[image boule ouverte.png]]
### Ouverte 
Une partie de $A$ est un ouverte de $\mathbb{R}^{2}$ si $\exists \varepsilon >0 \; ; \; \mathcal{B}(u, \varepsilon)<A$ 
![[image ouverte.png]]

## Fonctions définies sur une partie de $\mathbb{R}^{2}$, limite, continuité
### Applications partielles 
Fonction $f$ de $\mathbb{R}^{2}, A \subset \mathbb{R}^{2}, a=(x_{0},y_{0})$ 
Soit $f:A \longrightarrow \mathbb{R}$
- $\varphi_{1,a} : x \longmapsto f(x,y_{0})$ 
- $\varphi_{2,a} : x \longmapsto f(x_{0},y)$ 
- Les courbes de $\varphi_{1,a}$ et $\varphi_{2,a}$ sont les sections de la surface  $z=f(x,y)$ par les plans $y=y_{0}$ et $x=x_{0}$. 
![[image application partielles.png]]
### Continuité 
$f$ [[Limites et continuité#Continuité et prolongement par continuité|continue]] en $a$ si : $\forall \varepsilon>0, \exists \alpha >0 \; ; \; \forall u \in A, \; \| u-a \| \leq \alpha \Rightarrow (f(u)-f(a))\leq \varepsilon$
- $f$ continue en $A$ si $f$ continue en tout point de $A$.
- La somme, produit quotient, composé de deux fonctions continues est continue.
- $f$ continue en $a=(x_{0}, y_{0}) \Rightarrow \begin{cases} \varphi_{1,a} \text{  continue en  } x_{0}  \\ \varphi_{2,a} \text{  continue en  } y_{0}  \end{cases}$ 
	- La réciproque est fausse.

## Calcul différentiel 
Applications définies sur un ouverte $U$ de $\mathbb{R}^{2} \longrightarrow \mathbb{R}$  
### Dérivées partielles premières 
(sous réserve d'existence)
- $\displaystyle \frac{\partial f}{\partial x}(x_{0},y_{0})= \lim_{t \to 0} \frac{f(x_{0}+t,y_0)-f(x_{0},y_{0})}{t}$ 
- $\displaystyle \frac{\partial f}{\partial y}(x_{0},y_{0})=\lim_{t \to 0} \frac{f(x_{0},y_{0}+t)-f(x_{0},y_{0})}{t}$ 
- L'existence des dérivées partielles 1èrs n'implique continuité en ce point.
### Fonctions de Clase $C^{1}$ 
$f$ de classe $C^{1}$ en $a$, si $\frac{\partial f}{\partial x}$ et $\frac{\partial f}{\partial y}$ existent et sont continues en $a$. 
- La somme, produit, quotient des fonctions de classe $C^{1}$ est une fonction de classe $C^{1}$.
- Soit $f$ de classe $C^1$ sur $U$ et $a=(x_{0},y_{0}) \in U$. $f$ admet [[Analyse asymptotique#Développement limité|un]] $DL_{1}(a)$ :  $\displaystyle f(x_{0}+h,y_{0}+k)= \underbrace{f(x_{0},y_{0})}_{\text{Partie constante}} + \underbrace{\frac{\partial f}{\partial x}(x_{0},y_{0})h+\frac{\partial f}{\partial y}(x_{0},y_{0})k}_{\text{Partie linéaire}} + \underbrace{o(\| (h,k) \|)}_{\text{reste}}$ 
#### Approximation linéaire - différentielle
L'application $(h,k)\longmapsto f(x_{0}+h,y_{0}+k)-f(x_{0},y_{0})$ peut être approximée par l'application linéaire : $\displaystyle (h,k) \longmapsto \frac{\partial f}{\partial x}(x_{0},y_{0})h+\frac{\partial f}{\partial y}(x_{0},y_{0})k$ . C'est la différentielle de $f$ au point $a$.
#### Interprétation géométrique 
Plan tangente : $\displaystyle z=f(x_{0},y_{0})+(x-x_{0})\frac{\partial f}{\partial x}(x_{0},y_{0})+(y-y_{0})\frac{\partial f}{\partial y}(x_{0},y_{0})$ 
![[image plan tangente.png|300]]
#### Gradient 
Le gradient de $f$ (classe $C^{1}$) en $a$ est le vecteur : $\displaystyle \nabla f(x_{0},y_{0}) = (\frac{\partial f}{\partial x}(a), \frac{\partial f}{\partial y}(a))$   
- Définie la direction dans laquelle $f$ croît le plus vite.
### Dérivées partielles et composée
Soit $\overrightarrow{u}$ un vecteur, on appelle dérivé de $f$ en $a$ (s'il existe) : $\displaystyle \lim_{t \to 0} \frac{f(a+t \cdot \overrightarrow{u})-f(a)}{t}$ 
- Si $f$ de classe $C^1$ sa dérivée en $a$ selon $\overrightarrow{u}$ est : $\displaystyle \lim_{t \to 0} \frac{f(a+t \cdot \overrightarrow{u})-f(a)}{t} = \boxed{\nabla f(a) \cdot \overrightarrow{u}}$ 
#### Règle de la chaîne 
Soit $U$ un ouverte de $\mathbb{R}^{2}$ et $I \subset \mathbb{R}$ 
$f: U \longrightarrow \mathbb{R} \; ; \; (x,y)\longmapsto f(x,y)$ de classe $C^1$ 
$\gamma : I \longrightarrow U \; ; \; t \longmapsto (x(t),y(t))$ 
![[image regle chaine.png|400]] 
$\displaystyle F'(t)=(f(x(t),y(t)))'=x'(t) \frac{\partial f}{\partial x}(x(t),y(t))+y't\frac{\partial f}{\partial y}(x(t),y(t))$ 

Soit $U$ et $V$ deux ouvertes de $\mathbb{R}^{2}$
$f: U \longrightarrow \mathbb{R} \; ; \; (x,y)\longmapsto f(x,y)$ de classe $C^{1}$ 
$g: V \longrightarrow U \; ; \; (u,v) \longmapsto (\varphi(u,v), \psi(u,v))$ classe $C^{1}$ 
![[image chaine 2.png]]
Alors $F=f \circ g$ de classe $C^{1}$ 
En posant $(\varphi(u,v), \psi(u,v))=(x(u,v),y(u,v))$ 
$F(u,v)=f(x(u,v),y(u,v))$ 
$\begin{cases}\displaystyle \frac{\partial F}{\partial u} = \frac{\partial f}{\partial x} \frac{\partial x}{\partial u} + \frac{\partial f}{\partial y} \frac{\partial y}{\partial u}  \\ \displaystyle \frac{\partial F}{\partial v} = \frac{\partial f}{\partial x} \frac{\partial x}{\partial v} + \frac{\partial f}{\partial y} \frac{\partial y}{\partial v} \end{cases}$ 
## Extremum local
### Point critique
Soit $f$ de classe $C^{1}$ sur $U$
Un point $a \in U$ tel que $\begin{cases} \displaystyle \frac{\partial f }{ \partial x}(a)=0 \\ \displaystyle \frac{\partial f }{ \partial y}(a)=0 \end{cases}$  s'appelle point critique de $f$.
### Présence de extremum
Si $f$ présente un extremum local en $a \Rightarrow \begin{cases} \displaystyle \frac{\partial f }{ \partial x}(a)=0 \\ \displaystyle \frac{\partial f }{ \partial y}(a)=0 \end{cases}$ 
- La réciproque est fausse 