#chapitre7 #mecanique #cinematique #dynamique
### Mécanique 
Etude du mouvement des corps matériels 
### Cinématique
Etude des mouvements indépendamment de ses causes 
### Dynamique 
Lien entre le mouvement et ses causes

## Repère d'espace et référentiel
### Repère
Système de coordonnées permettant définir la position des points 
### Référentielle
Définie par un repère spatial et un temporelle
### Système cartésienne $(\vec{e_{x}},\vec{e_{y}},\vec{e_{x}})$
$\vec{OM}=x \vec{e_{x}}+ y \vec{e_{y}}+z\vec{e_{z}}$
![[image system cartesienne.png|300]]
### Système polaire 
$r \in \mathbb{R}^{+}$  $\theta \in [0,2\pi]$
$\vec{OM}=\vec{r}=r \vec{e_{r}}$ 
![[image system polaire.png|300]]
#### Passer de repérage polaire à cartésienne
$x=r \cos(\theta)$,  $y=r \sin(\theta)$,   $r =\sqrt{x^{2}+y^{2}}$
$\vec{e_{r}}=\cos(\theta)\vec{e_{x}} + \sin(\theta)\vec{e_{y}}$,  $\vec{e_{\theta}}=-\sin(\theta)\vec{e_{x}} + \cos(\theta)\vec{e_{y}}$
### Système cylindrique $(\vec{e_{r}},\vec{e_{\theta}},\vec{e_{z}})$ 
$\vec{OM}=\vec{r}=r\vec{e_{r}}+z\vec{e_{z}}$
![[image system cylindrique.png|300]]
### Système sphérique $(\vec{e_{r}},\vec{e_{\theta}},\vec{e_{z}})$ 
$r \in \mathbb{R}^{+}$,   $\theta \in [0,\pi]$,  $\varphi \in [0,2\pi]$ 
$\vec{OM}=\vec{r}=r\vec{e_{r}}$ 
![[image system spherique.png|300]] 

## Cinématique du point 
### vecteur position 
$\vec{OM}(t)=x(t)\vec{e_{x}} +y(t)\vec{e_{y}} z(t)\vec{e_{z}}$
#### Trajectoire
Courbe décrit par les positions successive de $M$
### Vecteur vitesse 
$\Delta \vec{OM}=\vec{M(t)M(t+\Delta t)}$ 
#### repère cartésien: $\vec{v}=\dot{x}\vec{e_{x}} +\dot{y}\vec{e_{y}}$ 
#### repère cylindrique: $\vec{v}=\dot{r}\vec{e_{r}} +r\dot{\theta}\vec{e_{\theta}}+z\vec{e_{z}}$
$\displaystyle \dot{\vec{e_{r}}}=\dot{\theta} \vec{e_{\theta}}$  
### Vecteur accélération
$\displaystyle \vec{a}(t)=\frac{d\vec{v}}{dt}$ 
#### repère cartésien: $\vec{a}=\ddot{x}\vec{e_{x}} +\ddot{y}\vec{e_{y}}+\ddot{z}\vec{e_{z}}$ 
#### repère cylindrique: $\vec{a}=(\ddot{r}-r \dot{\theta}^{2})\vec{e_{r}} +(2\dot{r}\dot{\theta}+r\ddot{\theta})\vec{e_{\theta}}+\ddot{z}\vec{e_{z}}$
$\dot{\vec{e_{\theta}}}=-\dot{\theta}\vec{e_{r}}$   
### Mouvement à vecteur accélération constant
$\begin{cases} \overrightarrow{a}= \overrightarrow{g} \\ \overrightarrow{v}(t) = \overrightarrow{g}\,t + \overrightarrow{v_{0}} \\ \overrightarrow{r}(t)=\frac{1}{2} \overrightarrow{g} \, t^{2} + \overrightarrow{v_{0}} \,t + \overrightarrow{r_{0}} \end{cases}$      avec  $\overrightarrow{v_{0}}= \begin{pmatrix} v_{0} \cos(\alpha) \\ v_{0} \sin(\alpha) \end{pmatrix}$ 
#### Trajectoire 
$\displaystyle y= -x^{2} \frac{g}{2 v_{0}^{2} \cos^{2}(\alpha)} + x \tan(\alpha)$ 
### Mouvement circulaire 
$\overrightarrow{v}= R\, \omega \, \overrightarrow{e_{\theta}}$ 
#### Mouvement uniforme 
- $v_{0}=R \, \omega = cst$ 
- $\overrightarrow{a}=-R \, \theta^{2}\overrightarrow{e_{r}}$ 
#### Mouvement non uniforme
$\overrightarrow{a} = \begin{cases} -R \omega^{2} \\ R \dot{\omega} \end{cases}$ 
### Base de Frenet 
- $\overrightarrow{v}=v \overrightarrow{T}$
- $\displaystyle \overrightarrow{a}= \frac{v^{2}}{R}\overrightarrow{N} + \dot{v} \overrightarrow{T}$   