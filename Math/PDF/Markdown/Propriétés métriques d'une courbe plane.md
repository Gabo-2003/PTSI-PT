## Abscisse curviligne 
### Longueur d'une courbe paramétrée régulière
Soit $f : [t_{1},t_{2}] \longrightarrow \mathbb{R}^{2}$ ou $\mathbb{R}^{3}$, de classe $C^{1}$.
On appelle longueur de la courbe paramétrée $([t_{1},t_{2}], f)$ le réel positif :
$\displaystyle \mathcal{L} = \int_{t_{1}}^{t_{2}} \| \overrightarrow{f'}(t) \|    \: d{t}$
### Abscisse curviligne 
Soit la courbe paramétrée $\Gamma : (I,f)$ de classe $C^{k}$ ($k\geq 2$).
On appelle abscisse curviligne de cette courbe toute application $\sigma$ de classe $C^{1}$ sur $I$ telle que :
$\sigma ' = \| f'(t) \|$
- La longueur de la courbe $([t_{1},t_{2}]\subset I,f)$ est :  $\mathcal{L} = \sigma (t_{2})- \sigma (t_{1})$ 
#### Paramétrage normal 
Appelé aussi paramétrage par l'abscisse curviligne.
Si $\forall t \in I$, $\| f'(t) \|=1$,  alors $s(t)=t$ définie un abscisse curviligne de $\Gamma$. 
### Repère de Frenet
![[image repère frenet.png|400]]
Soit $(I,f)$ une courbe paramétrée $C^{1}$ régulière (la vitesse ne s'annule pas) du plan. 
Le repère orthonormé directe $(M(t), \overrightarrow{T}(t), \overrightarrow{N}(t))$ est appelé repère de Frénet de la courbe $(I,f)$ en $M(t) = f(t) = (x(t),y(t))$.
- $\displaystyle \overrightarrow{T}(t) = \frac{1}{\| \overrightarrow{f'}(t) \|}  \overrightarrow{f'}(t) = \frac{1}{s'(t)} \Big( x'(t), y'(t) \Big)$ 
- $\displaystyle \overrightarrow{N}(t) =  \frac{1}{s'(t)} \Big( -y'(t),x'(t) \Big)$

## Courbure en un point régulier 
### Courbure d'une courbe régulière 
Soit $\Gamma : (I,f)$ avec $f$ de classe $C^{2}$ sur $I$.
Soit $s$ une abscisse curviligne. 
En un point régulier $M(t)$ la courbure de $\Gamma$ est l'unique réel $\gamma (t)$ tel que :
$\displaystyle \frac{d \overrightarrow{T}}{dt} = \frac{ds}{dt} \gamma (t) \overrightarrow{N}(t) \Leftrightarrow \frac{d \overrightarrow{T}}{ds}(t) = \gamma (t) \overrightarrow{N}(t)$
- $\displaystyle  \frac{ds}{dt}(t) = \| \overrightarrow{f'}(t) \|$
La courbure décrit la déviation "normale" du vecteur tangent $\overrightarrow{T}$ :
- $\gamma >0$ : $\overrightarrow{T}$ dévie vers la gauche dans le sens de parcours.
- $\gamma < 0$ : $\overrightarrow{T}$ dévie vers la droite dans le sens de parcours.
#### Formules de Frénet 
- $\displaystyle \frac{d \overrightarrow{N}}{ds} = - \gamma \overrightarrow{T}$ 
- $\displaystyle \frac{d \overrightarrow{T}}{ds} = \gamma  \overrightarrow{N}$
### Théorème de relèvement 
Soit $(I,f)$ une courbe paramétrée régulière de classe $C^{k}$ tel que $(I,f)$ est une *paramétrage par l'abscisse curviligne* : $\| f'(t) \|  =1$.
Il existe une fonction $\alpha$ de classe $C^{k}$ sur $I$ telle que :
$\forall s \in I, \quad \overrightarrow{T}(s) = \cos( \alpha (s)) \overrightarrow{e_{1}} + \sin(\alpha (s))\overrightarrow{e_{2}}$
- Avec $(\overrightarrow{e_{1}} ,\overrightarrow{e_{2}} )$ une BOND fixe.
- $\displaystyle \gamma = \frac{d \alpha }{ds}$
### Rayon et centre de courbure 
#### Rayon de courbure
![[image rayon de courbure.png|400]]
Soit $M(t)$ un *point birégulier* ($\gamma (t) \neq 0$) d'une courbe de classe $C^{2}$.
On appelle rayon de courbure au point $M(t)$ le réel : 
$\displaystyle R(t) = \frac{1}{\gamma (t)} = \frac{ds}{d \alpha }$ 
#### Centre de courbure
Si $\Gamma =(I,f)$ est birégulier de classe $C^{2}$. 
On appelle centre de courbure $C(t)$ de la courbe au point $M(t)$, le point :
$C(t) = M(t) + R(t) \overrightarrow{N}(t)$ 
Alors $t \longmapsto C(t)$ est une courbe de classe $C^{1}$ appelé développée de $\Gamma$.
- Le cercle de courbure est le cercle de centre $C(t)$ et de rayon $R(t)$.

## Enveloppe d'une famille de droites 
### Enveloppe 
Soit $I \subset \mathbb{R}$. Soit $(D_{t})_{t \in I}$ une famille de droites. 
La courbe paramétrée de classe $C^{1}$ $(I,f)$ est une enveloppe de la famille de droites $(D_{t})_{t\in I}$ : 
$\Leftrightarrow \forall t \in I$,   $D_{t}$ est la tangente au support $\Gamma$ de la courbe en $M(t) = f(t)$.
$\Leftrightarrow \forall t \in I$,   $f(t)$ est sur $D_{t}$ et $D_{t}$ est dirigée par $f'(t)$.
Soit le paramétrage $D_{t} : A(t) + \lambda (t) \overrightarrow{u}(t)$ un paramétrage des droites.
$(I,f)$ est l'enveloppe des droites $(D_{t})_{t \in I}$ :
$\Leftrightarrow$ il existe une fonction $K(t)$ de classe $C^{1}$ sur $I$ vérifiant : 
$\forall t \in I, \quad f(t) = A(t) + K(t)\overrightarrow{u}(t)$ et $f'(t)$ est colinéaire à $\overrightarrow{u}$ 
Alors on fait : $[f'(t), \overrightarrow{u}] = 0 \Leftrightarrow \det_{B_{0}}(f'(t), \overrightarrow{u})=0$
### Développée comme enveloppe des normales 
La développée d'une courbe birégulière est l'enveloppe de ses normales.