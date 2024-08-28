## Surfaces paramétrées 
### Définition 
Soit $\Omega$ un ouvert de $\mathbb{R}^{2}$.
Soit $f: \Omega \longrightarrow \mathbb{R}^{3} : (u,v) \longmapsto \Big(x(u,v),y(u,v),z(u,v) \Big)$ une application de classe $C^{1}$.
Une surface paramétrée de classe $C^{1}$ est le couple $(\Omega ,f)$. 
- Le point $f(u_{0}, v_{0})$ est régulière si :
La famille $\displaystyle \left( \frac{\partial f}{\partial u} (u_{0},v_{_0}), \frac{\partial f}{\partial v} (u_{0},v_{0}) \right)$ est libre $\displaystyle \Leftrightarrow  \frac{\partial f}{\partial u} (u_{0},v_{_0}) \wedge  \frac{\partial f}{\partial v} (u_{0},v_{0})  = \overrightarrow{n} \neq \overrightarrow{0}$. 
### Plan tangent en un point régulière 
Soit $\Omega \subset \mathbb{R}^{2}$ un ouvert et $f : \Omega \longrightarrow \mathbb{R}^{3}$ de classe $C^{1}$. 
Le plan tangente de $(\Omega ,f)$ au point régulière $f(u_{0},v_{0})$ est dirigé par les vecteurs : $\displaystyle  \frac{\partial f}{\partial u} (u_{0},v_{_0})$ et $\displaystyle \frac{\partial f}{\partial v} (u_{0},v_{0})$.
- $\overrightarrow{n}$ est un vecteur normal à ce plan.
### Cas des surfaces paramétrées cartésiennes
Soit $\Omega \subset \mathbb{R}^{2}$ un ouvert et $\varphi  : \Omega \longrightarrow \mathbb{R}$ de classe $C^{1}$. 
La surface $(\Omega ,f)$ définie par $f : (x,y) \longmapsto (x,y, \varphi (x,y))$ est dite cartésienne. 
On trouve $\displaystyle \frac{\partial f}{\partial x}  \wedge \frac{\partial f}{\partial y}  = \left( - \frac{\partial \varphi }{\partial x} , - \frac{\partial \varphi }{\partial y} ,1 \right)$, donc toute surface cartésienne est régulière.
### Courbes tracées sur une surface paramétrée 
Soit $\Sigma = (U,f)$ une surface paramétrée de classe $C^{1}$ avec $U$ ouvert de $\mathbb{R}^{2}$.
Soit la courbe $\Gamma :t \longmapsto \gamma(  u(t), v(t))$ de classe $C^{1}$ sur $I\subset U$. 
$\Gamma$ est tracée sur $\Sigma$ s'il admet une paramétrage de la forme $\Gamma : f(u(t),v(t))$. 
- Soit $M$ un point régulières appartenant à $\Gamma \cap \Sigma$. La tangent en $M$ de $\Gamma$ est incluse dans le plan tangent en $M$ de $\Sigma$. 
#### Courbes coordonnées 
Au point $M_{0}=f(u_{0},v_{0})$ sont les courbes de l'espace :
$t \longmapsto f(t,v_{0})$ et $t \longmapsto f(u_{0},t)$ 
#### Sections planes 
Obtenues en coupant une surface $\Sigma$ par des plans. 

## Surfaces définies par une équation cartésienne 
### Définition 
Soit $U\subset \mathbb{R}^{3}$ un ouvert. Soit $F : U \longrightarrow \mathbb{R}$ de classe $C^{1}$. 
$\Sigma = \{  (x,y,z) \in U |  F(x,y,z) = 0\}$ est la surface définie par l'équation cartésienne $F(x,y,z) = 0$.
- Surface de niveau $0$ de la fonction $F : (x,y,z) \longmapsto F(x,y,z)$. 
- On ne trouve pas toujours une surface. 
### Plan tangente
Une équation cartésienne $F(x,y,z) = 0$ avec $F$ de classe $C^{1}$ admet une paramétrage local de classe $C^{1}$.
Soit $U$ un ouvert de $\mathbb{R}^{3}$.
Soit $F : U \longrightarrow	\mathbb{R}$ de classe $C^{1}$.
Soit $\Sigma$ la surface d'équation  $F(x,y,z) = 0$.
On dit que le point $m_{0} = (x_{0},y_{0},z_{0})$ est régulier si $\nabla F(m_{0}) \neq	\overrightarrow{0}$.
- Si $m_{0}$ régulier, le plan tangent à $\Sigma$ passant par $m_{0}$ est $\perp$ à $\nabla F(m_{0})$.
### Surfaces de niveau 
Les surfaces $\Sigma_{k}$ d'équation $F(x,y,z) = k$, $k \in \mathbb{R}$ s'appellent surfaces de niveau de $F$. 
### Courbes tracées sur une surface définie par une équation cartésienne 
Soit $\Gamma$ une courbe de $\mathbb{R}^{3}$ paramétrée par $t \longmapsto (x(t),y(t),z(t))$ sur une intervalle $I\subset \mathbb{R}$.
On dit que cette courbe est tracée sur $\Sigma$ lorsque $\forall t \in I, F \Big( x(t),y(t),z(t) \Big)=0$. 
- Si $M$ est un point régulier à la fois de $\Gamma$ et de $\Sigma$ alors la tangente en $M$ à $\Gamma$ est incluse dans le plan tangent en $M$ à $\Sigma$.  
#### Droites tracées sur une surface 
Pour trouver les droites tracées sur une surface, on cherche un paramétrage :
$t \longmapsto \Big( x_{0}+at, y_{0}+bt,z_{0}+ct \Big)$ avec tous ces variables des inconnues, qui vérifient : 
 $\forall t \in I, F( x_{0}+at, y_{0}+bt,z_{0}+ct )=0$

## Surfaces réglées 
### Définition
Une surface réglées est une surface qui est une réunion de droites. 
- Ces droites sont appelées génératrices de la surface. 
La famille $(D_{u})_{I}$ doit être $C^{1}$ : 
Soit $\varphi  : I\subset I \longrightarrow \mathbb{R}^{3}$ de classe $C^{1}$.
Soit $\overrightarrow{K} : I \longrightarrow \mathbb{R}^{*3}$ de classe $C^{1}$.
$\forall u \in I, (D_{u})_{I}$ passe par $\varphi (u)$ et est dirigée par $\overrightarrow{K}(u)$. 
- La courbe de l'espace $u \longmapsto \varphi (u)$ est appelée directrice de la surface réglée. 
### Plan tangent à une surface réglée
Soit $\Sigma$ une surface reglée de classe $C^{1}$ paramétrée par $f : (u,v) \longmapsto \varphi (u) + v \overrightarrow{K}(u)$. 
Le plan tangent en un point régulière d'une surface réglée $\Sigma$ contient la génératrice passant par ce point. 

## Surfaces de révolution 
### Définition et caractérisation 
On dit que la surface $\Sigma$ est une surface de révolution si il existe une droite $\Delta$ telle que $\Sigma$ soit invariante par toute rotation autour de $\Delta$. 
On appelle plan méridien de $\Sigma$ tout plan contenant son axe de révolution. Les méridiens sont les sections de $\Sigma$ coupés. 
Une surface $\Sigma$ est une surface de révolution autour de la droite $\Delta$ si et seulement si l'intersection de $\Sigma$ avec tout plan orthogonal à $\Delta$ est un cercle ou une réunion de cercles d'axe $\Delta$. 
### Paramétrage d'une surface de révolution d'axe $Oz$. 
![[image surface de revolution.png|400]]
Soit la courbe $\Gamma : t \longmapsto \Big( x_{1}(t), y_{1}(t), z_{1}(t) \Big)$ Alors, $M(x,y,z) \in \Sigma$ :
$\Leftrightarrow \exists P \in \Gamma$ tel que $M$ est l'image de $P$ par une rotation d'axe $Oz$. 
$\Leftrightarrow \exists (t,\theta) \in I \times \mathbb{R}; \quad \begin{pmatrix} x \\ y \\ z \end{pmatrix} = \begin{pmatrix} \cos(\theta) & - \sin(\theta) & 0 \\ \sin(\theta) & \cos(\theta) & 0 \\  0 & 0 & 1 \end{pmatrix} \begin{pmatrix} x_{1}(t) \\ y_{1}(t) \\ z_{1}(t) \end{pmatrix}$ 
Soit $t = \sqrt{x^{2} + y^{2}}$.
Si $u \longmapsto (r(u), z(u))$ est la courbe méridienne d'une surface de révolution. 
Alors $(u,\theta) \longmapsto \Big( r(u)\cos(\theta), r(u)\sin(\theta), z(u) \Big)$ est une paramétrage de cette surface. 
### Obtention d'une équation cartésienne d'une surface de révolution 
#### Méthode 1 
On utilise un paramétrage et on enlève les paramètres. 
#### Méthode 2 
Soit $\Delta : G + Vect(\overrightarrow{u})$ la droite de révolution de $\Sigma$.
Soit $\Gamma : t \longmapsto P(t)$ une courbe (c'est une méridienne de $\Sigma$). 
Le point de l'espace $M(x,y,z) \in \Sigma$ $\Leftrightarrow \exists P \in \Gamma ; \begin{cases} \overrightarrow{GP} \cdot \overrightarrow{u} = \overrightarrow{GM} \cdot  \overrightarrow{u} \\ OP = OM \end{cases}$
### Plan tangent à une surface de révolution 

## Courbe définie par l'intersection de deux surfaces 
On peut définir une courbe $\Gamma$ (pas tout le temps) comme l'intersection de deux surfaces définies par une équation cartésienne : 
$\Gamma : \begin{cases} f(x,y,z) = 0 \\g(x,y,z) = 0 \end{cases}$ avec $f$ et $g$ de classe $C^{1}$ sur $\mathbb{R}^{3}$. 
### Point régulier sur une courbe 
Un point de la courbe définie par le système précèdent est régulier si les gradients de $f$ et de $g$ sont linéairement indépendantes.
### Tangente en un point régulier 
Soit $M_{0} \in \Sigma_{1} \cap \Sigma_{2}$.
La tangente de $\Gamma$ au point $M_{0}$ est l'intersection des plans tangentes de $\Sigma_{1}$ et de $\Sigma_{2}$ en $M_{0}$. 
- Elle est dirigé par $\nabla f(M_{0}) \wedge \nabla g(M_{0})$. 
## Bilan
### Surfaces
$f(x,y,z) = 0$ équation cartésienne d'une surface. $\nabla f \perp$ au plan tangent. 
$f :(u,v) \longmapsto \Big( x(u,v), y(u,v), z(u,v) \Big)$ surface paramétrée : $\displaystyle \frac{\partial f}{\partial u} \wedge \frac{\partial f}{\partial v} \perp$ au plan tangent. 
$f: (x,y) \longmapsto \Big(x,y, \varphi (x,y) \Big)$ surface paramétrée cartésienne : tout le temps régulière. 
- $\varphi :(x,y) \longmapsto  \varphi (x,y)$ : fonction à 2 variables pour étudier $z = \varphi (x,y)$ et $\nabla \varphi \perp$ aux courbes de niveaux.
### Courbes
$f : t \longmapsto \Big( x(t), y(t) \Big)$ : paramétrage d'une courbe, $f'(t)$ dirige la tangente. 
$F(x,y) = 0$ équation cartésienne de courbe dans le plan, $\nabla F \perp$ à la courbe. 
