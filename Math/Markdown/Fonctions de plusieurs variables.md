## Limites et continuité des fonctions de $\mathbb{R}^{p}$ dans $\mathbb{R}$
Pour $u \in \mathbb{R}^{p}, \quad \lVert u \rVert = \sqrt{u_{1}^{2} + u_{2}^{2} + \ldots u_{p}^{2}}$
$d(a,u) = \lVert u-a \rVert$
### Ouverts 
![[Prepa/PT/Math/Attachments math/image ouverte.png]]
#### Boule ouverte
Boule ouverte de centre $a$ et de rayon $r >0$ :
$\mathcal{B}(a,r) = \{ u \in \mathbb{R}^{^p} \setminus d(a,u) < r \}$ 
#### Boule fermée
$\mathcal{B}_{f} = \{ u \in \mathbb{R}^{p} \setminus d(a,u) \leq r \}$
#### Partie ouvert
Une partie $U$ de $\mathbb{R}^{p}$ est un ouvert de $\mathbb{R}^{p}$ si :
$\forall a \in U, \; \exists$ un reél $r>0 ; \quad \mathcal{B}(a,r) \subset U$
- L'intersection de deux ouverts et un ouvert.
- La réunion d'un nombre éventuellement infinie de ouverts est un ouvert.
- Une partie $B$ de $\mathbb{R}^{p}$ est un fermée $\Leftrightarrow$ son complémentaire est un ouvert.
#### Point intérieur 
Soit $A$ une partie de $\mathbb{R}^{p}$, $u$ est intérieur à $A$ si :
$\exists r >0 ; \quad \mathcal{B}(u,r) \subset A$
- $A$ est un ouvert de $\mathbb{R}^{p} \Leftrightarrow$ tous ses points sont intérieurs.
#### Point adhérent 
$a \in \mathbb{R}^{p}$ adhérent à $A$ si :
Tout $\mathcal{B}(a,r)$ avec $r>0$ rencontre  $A$.
- Une partie est un fermée s'il contient tous ses points adhérents.
### Applications partielles 
![[image application partielles.png]]
Soit $U$ un ouverte de $\mathbb{R}^{p}$ et $f : U \longrightarrow \mathbb{R}$ une application à deux variables.
Pour chaque point $a= (x_{a}, y_{a})\in U$ on définit les applications partielles de $f$ en $a$.
$\begin{align*}f_{1} : U_{1} &\longrightarrow \mathbb{R}\\ t &\longmapsto f(t,y_{a})\end{align*}$
$\begin{align*} f_{2} : U_{2} &\longrightarrow \mathbb{R} \\ t &\longmapsto f(x_{a},t) \end{align*}$
Avec : $\begin{cases} U_{1} = \{ t \in \mathbb{R} \setminus (t,y_{a}) \in U \} \\ U_{2} = \{ t \in \mathbb{R} \setminus (x_{a},t) \in U \} \end{cases}$
### Limite et continuité en un point
Soit $f: A \subset \mathbb{R}^{2} \longrightarrow \mathbb{R}$, $a$ adhérent à $A$, $l \in \mathbb{R}$.
$f$ tend vers $l$ en $a$ si :
$\forall \epsilon >0, \; \exists \eta > 0 : \quad \forall u \in A, \; d(a,u) \leq \eta \implies |f(u)-l| \leq \epsilon$
- Lorsque $a \in A$ si $f$ admet un limite $l$ en $a$, celle ci est égale à $f(a)$ et on dit que $f$ est continue en $a$.
#### Limite selon un chemin
Soit $f : U \in \mathbb{R}^{p} \longrightarrow \mathbb{R}$.
Soit $a$ adhérent à $U$.
Soit $l \in \mathbb{R}$ et $\varphi : \mathbb{R} \longrightarrow \mathbb{R}^{p}; \; \forall t \in \mathbb{R}, \;  \varphi (t) \in U$. 
Si $f(u) \underset{u \to a} \longrightarrow l$ et si $\varphi (t) \underset{t \to 0} \longrightarrow a$, 
alors $f(\varphi (t)) \underset{t \to 0} \longrightarrow l$ 
### Propriétés des fonctions continues 
Si $f : \mathbb{R}^{p} \longrightarrow \mathbb{R}$ est continue alors :
- $\{ x \in \mathbb{R}^{p} \setminus f(x) > 0 \}$ est un ouverte de $\mathbb{R}^{p}$.
- $\{ x \in \mathbb{R}^{p} \setminus f(x) \geq  0$ et $\{ x \in \mathbb{R}^{p} \setminus f(x)=0\}$ sont des fermés de $\mathbb{R}^{p}$  
#### Théorème des bornes atteint
 Tout fonction réelle continue sur une partie fermée de $\mathbb{R}^{p}$ est bornée et atteint ses bornes.

## Dérivées partielles d'une fonction de $\mathbb{R}^{p}$ dans $\mathbb{R}$
### Dérivées partielles d'ordre 1
Soit $f : A \subset \mathbb{R}^{p} \longrightarrow \mathbb{R}$, $a$ un point intérieur à $A$.
$f$ admet une dérivée partielle par rapport à sa jème variable si sa jème application partielle en $a$ est dérivable en $a_{j}$.
- $\displaystyle \frac{\partial f}{\partial x} (a) = \lim_{x \to x_{a}}  \frac{f(x,y_{a}) - f(x_{a},y_{a})}{x-x_{a}}$
- $\displaystyle  \frac{\partial f}{\partial y} (a) = \lim_{y \to y_{a}}  \frac{f(x_{a},y) - f(x_{a}, y_{a})}{y-y_{a}}$
### Fonctions de classe $C^{1}$ sur un ouvert de $\mathbb{R}^{p}$
Une fonction $f : U \subset \mathbb{R}^{p} \longrightarrow \mathbb{R}$ est $C^{1}$ sur $U$ si elle admet des dérivées partielles d'ordre $1$ en tout point $u$ de $U$, et si ces dérivées partielles sont continues sur  $U$.
- Soit  $f$ de classe $C^{1}$ sur $\mathbb{R}^{2}$. Si $\frac{\partial f}{\partial x} =0$ sur $\mathbb{R}^{2}$ alors il existe $g$ de classe $C^{1}$ sur $\mathbb{R}$ telle que $\forall (x,y) \in \mathbb{R}^{2}$, $f(x,y) = g(y)$. De même pour $y$. Ne s'applique que si les applications partielles sont définies sur un intervalle.
### Formule de Taylor-Young à l'ordre $1$
Soit $f : U \subset \mathbb{R}^{p} \longrightarrow \mathbb{R}$ de classe $C^{1}$. 
Pour $a \in U$, $\forall u \in U$ :
$\displaystyle f(u) = f(a) + \sum_{j=1}^{p} \frac{\partial f}{\partial x_{j}} (a) (u_{j} - a_{j}) + o( \lVert u-a \rVert )$ 
Pour $p=2$ :
 $\displaystyle  f(x,y) = f(x_{a},y_{a}) + \frac{\partial f}{\partial x} (x_{a},y_{a}) (x-x_{a}) + \frac{\partial f}{\partial y} (x_{a},y_{a}) (y-y_{a}) + o(\lVert (x,y) - a \rVert )$ 
 - Le plan d'équation $z = f(x_{a},y_{a}) + \frac{\partial f}{\partial x} (x_{a},y_{a}) (x-x_{a}) + \frac{\partial f}{\partial y} (x_{a},y_{a}) (y-y_{a})$ est le plan tangent à la surface $z = f(x,y)$ en $a$.
### Gradient et point critique d'une fonction $C^{1}$ 
Soit $f : U\subset \mathbb{R}^{p}\longrightarrow \mathbb{R}$, soit $a$ un point de $U$ ou $f$ a des dérivées partielles.
On appelle gradient de $f$ en $a$ le vecteur de $\mathbb{R}^{p}$ :
$\displaystyle \nabla f(a)= \left( \frac{\partial f}{\partial x_{1}} (a), \frac{\partial f}{\partial x_{2}} (a), \ldots, \frac{\partial f}{\partial x_{p}}(a)  \right)$
- On appelle point critique de $f$ les points où le gradient de $f$ s'annule.
Développent limité : pour $\overrightarrow{h}\in \mathbb{R}^{p}$ tel que $a+\overrightarrow{h}\in U$
$f(a+\overrightarrow{h}) = f(x_{a},y_{a}) + \nabla f(a) \cdot  \overrightarrow{h}+ o(\lVert \overrightarrow{h} \rVert )$ 
### Dérivée selon un vecteur 
Soit $f : U\subset \mathbb{R}^{2}\longrightarrow \mathbb{R}$ de classe  $C^{1}$, $f$ admet en tout point $a\in U$ une dérivées selon tout vecteur $\overrightarrow{v}=(v_{1}, v_{2})\in \mathbb{R}^{2}$ et on le note :
$\displaystyle D_{\overrightarrow{v}}f(a) = \nabla f(a) \cdot \overrightarrow{v} = \frac{\partial f}{\partial x} (a)v_{1}+ \frac{\partial f}{\partial y} (a)v_{2}$
### Règle de la chaîne
Soit $U$ et $I$ des ouverts.
Soit $\varphi  : I\subset \mathbb{R} \longrightarrow \mathbb{R}^{p}$ une fonction de classe $C^{1}$. Avec $\varphi (t) = (\varphi _{1}(t), \ldots, \varphi_{p}(t))$
Soit $f : U\subset \mathbb{R}^{p}\longrightarrow \mathbb{R}$ de classe $C^{1}$.
Si $\varphi(I) \subset U$, alors $f \circ \varphi$ est $C^{1}$ et 
$\displaystyle \frac{d}{dt}(f \circ \varphi) (t) = \sum_{j=1}^{p} \varphi'_{j}(t) \frac{\partial f}{\partial x_{j}} (\varphi (t))$
Pour $p=2$, on note $\varphi (t) = (x(t), y(t))$ et $z(t) = f(x(t),y(t))$ alors :
$\displaystyle \frac{dz}{dt} = \frac{\partial z}{\partial x} \cdot \frac{d x}{d t} + \frac{\partial z}{\partial y} \cdot \frac{dy }{dt }$ 
#### Dérivée le long d'une courbe paramètre
Soit  $f : U\subset \mathbb{R}^{2}\longrightarrow \mathbb{R}$ de classe  $C^{1}$.
Soit $\gamma :I \subset \mathbb{R} \longrightarrow U$ de classe $C^{1}$ et  $(\gamma ,I)$ une courbe paramètre.
$\forall t \in I, \quad (f\circ \gamma )'(t) = \nabla f(\gamma (t))\cdot \gamma '(t) = D_{\gamma '(t)}f(\gamma (t))$ 
#### Lignes de niveau
![[image lignes de niveau.png]]
Soit $f : U\subset \mathbb{R}^{2}\longrightarrow \mathbb{R}$ de classe  $C^{1}$. On appelle lignes de niveau de $f$ les courbes :
$\Gamma_{k} = \{  (x,y) \in  U \subset f(x,y)=k\}$ 
- Les lignes de niveau sont orthogonales au gradient en tout point ou le gradient est non nul. 
### Changement de variable et dérivation 
Soit $f : U\subset \mathbb{R}^{2}\longrightarrow \mathbb{R}$ de classe  $C^{1}$.
Soit $\varphi_{1},\varphi _{2} : V \subset \mathbb{R}^{2} \longrightarrow \mathbb{R}$ de classe $C^{1}$ telle que $\forall (u,v)\in V, \quad (\varphi _{1}(u,v), \varphi _{2}(u,v))\in U$.
Alors $H : (u,v) \longmapsto f(\varphi _{1}(u,v), \varphi _{2}(u,v))$ est $C^{1}$ sur $V$ et $\forall (u,v) \in V$ :

$\displaystyle  \frac{\partial H}{\partial u} = \frac{\partial f}{\partial x} \frac{\partial \varphi _{1}}{\partial u} + \frac{\partial f}{\partial y} \frac{\partial \varphi _{2}}{\partial u}$   et   $\displaystyle \frac{\partial H}{\partial v} = \frac{\partial f}{\partial x} \frac{\partial \varphi _{1}}{\partial v} + \frac{\partial f}{\partial y} \frac{\partial \varphi _{2}}{\partial v}$
### Dérivées partielles d'ordre 2
Soit $f : U\subset \mathbb{R}^{2}\longrightarrow \mathbb{R}$. Soit $a$ un point intérieur à $U$, si $f$ admet de dérivées partielles en $a$ et si ses dérivées ont des dérivées partielles, on dit que $f$ a des dérivées partielles secondes.
- $f$ est de classe $C^{2}$ si toutes ses dérivées partielles sont de classe $C^{1}$.
#### Théorème de Schwarz 
$\displaystyle \frac{\partial ^{2}f}{\partial x \partial y} = \frac{\partial ^{2}f}{\partial  y \partial x}$ 
### Formule de Taylor à l'ordre 2
Soit $f : U\subset \mathbb{R}^{2}\longrightarrow \mathbb{R}$ de classe  $C^{2}$. Soit $a = (x_{a},y_{a}) \in U$.
$\displaystyle f(x,y)= f(a) + \frac{\partial f}{\partial x} (a) (x-x_{a}) + \frac{\partial f}{\partial y} (y-y_{a}) + \frac{1}{2} \left( \frac{\partial ^{2}f}{\partial x^{2}} (x-x_{a})^{2} + \frac{\partial ^{2}f}{\partial x \partial y} 2(x-x_{a})(y-y_{a}) + \frac{\partial ^{2}f}{\partial y^{2}} (y-y_{a})^{2} \right) + o(\lVert(x,y)-a \rVert^{2} )$

## Fonctions de $\mathbb{R}^{p}$ dans $\mathbb{R}^{n}$
### Applications coordonnées
Soit $U$ un ouvert.
Soit  $\varphi : U \subset \mathbb{R}^{p} \longrightarrow \mathbb{R}^{n}$.
On note pour $u \in U$ : $\varphi (u) = \varphi _{1}(u), \ldots, \varphi_{n}(u)$
### Limites et continuité 
Soit $\varphi : A \subset \mathbb{R}^{p} \longrightarrow \mathbb{R}^{n}$, $A$ une partie de $\mathbb{R}^{p}$.
- Lorsque $a \in A \subset \mathbb{R}^{p}$, si $\varphi$ admet un limite $l$ en $a$, celle ci est égal à $\varphi (a)$ et on dit que $\varphi$ est continue en $a$.
- Si $a$ intérieur à $A$. $\varphi$ a ine limite en $a$ si et seulement si ses $n$ fonctions ont une limite en $a$.
### Dérivées partielles d'ordre 1 et 2
- $\varphi$ admet des dérivées partielles en un point si toutes les applications coordonnées $\varphi _{i}$ admettent des dérivées partielles en ce point.
- $\varphi$ est $C^{1}$ sur $U$ si ses applications coordonnées sont tous $C^{1}$ sur $U$.
### Formules de dérivation composée
Soit $U$ et $V$ ouverts de $\mathbb{R}^{2}$. 
Soit $\varphi :U \longrightarrow \mathbb{R}^{2} ; (u,v) \longmapsto (\varphi _{1}(u,v), \varphi _{2}(u,v))$.
Soit $f : V \longrightarrow \mathbb{R}$.
Si $f$ est $C^{1}$ sur $V$, $\varphi$ est $C^{1}$ sur $U$ et $\varphi (U) \subset V$.
On pose $g = f \circ \varphi = f(\varphi (u,v)) = f (\varphi _{1}(u,v), \varphi _{2}(u,v)) = (x(u,v), y(u,v))$.
$\displaystyle \frac{\partial g}{\partial u} = \frac{\partial x}{\partial u} \frac{\partial f}{\partial x} + \frac{\partial y}{\partial u} \frac{\partial f}{\partial y}$
$\displaystyle \frac{\partial g}{\partial v} = \frac{\partial x}{\partial v} \frac{\partial f}{\partial x} + \frac{\partial y}{\partial v} \frac{\partial f}{\partial y}$ 

## Extremum d'une fonction de 2 variables 
### Extremum local ou global
Si $f$ possède un extremum local en $a$, alors tout arc paramètre passant par ce point possède un extremum local.
### Condition suffisante d'extremum global 
Théorème des bornes atteints : 
Soit $K$ une partie fermée bornée de $\mathbb{R}^{p}$. 
Soit $f : K \longrightarrow \mathbb{R}$ continue.
Alors $f$ est bornée et atteint ses bornes, donc $f$ a un minimum global et un maximum global sur $K$.
### Condition nécessaire d'extremum 
Soit $f : U \subset \mathbb{R}^{2} \longrightarrow \mathbb{R}$ de classe $C^{1}$.
Si $f$ possède un extremum local en $a\in U$ (ou $a$ intérieur a une partie $A \subset \mathbb{R}^{2}$), alors $a$ est un point critique de $f$.
### Matrice Hessienne
Soit $f : U \subset \mathbb{R}^{2} \longrightarrow \mathbb{R}$ de classe $C^{2}$. 
Pour $a \in U$ on appelle matrice Hessienne de $f$ en $a$ la matrice :
$H_{f}(a) = \begin{pmatrix} \frac{\partial ^{2}f}{\partial x^{2}} (a) & \frac{\partial ^{2}f}{\partial y \partial x}(a)  \\ \frac{\partial ^{2}f}{\partial x \partial y}(a) & \frac{\partial^{2}f }{\partial y^{2}}(a)  \end{pmatrix}$
- $H_{f}$ est symétrique donc diagonalisable dans une base orthonormé. 
#### Nature d'un point critique
On note $\lambda$ et $\mu$ les valeurs propres de $H_{f}$.
- Si $\det(H_{f})(a) >0$ et $tr(H_{f}(a)) >0$ c'est à dire $\lambda >0$ et $\mu >0$, alors $f$ a un minimum local en $a$. 
- Si $\det(H_{f})(a) >0$ et $tr(H_{f}(a)) <0$ c'est à dire $\lambda <0$ et $\mu <0$, alors $f$ a un maximum local en $a$.
- Si $\det(H_{f})(a) <0$  c'est à dire $\lambda\cdot \mu  <0$,  alors $f$ a un point selle en $a$.
- Si $\det(H_{f}(a))=0$ on ne peut pas conclure. 

## Résolution d'équations aux dérivées partielles
Si $f : \mathbb{R}^{2} \longrightarrow \mathbb{R}$ est classe $C^{1}$ et vérifie $\forall a \in \mathbb{R}^{2}$, $\displaystyle \frac{\partial f}{\partial x} (a)=0$.
Alors il existe une fonction $A : \mathbb{R} \longrightarrow \mathbb{R}$ de classe $C^{1}$ telle que $\forall (x,y) \in \mathbb{R}^{2}$, $f(x,y) = A(y)$.
