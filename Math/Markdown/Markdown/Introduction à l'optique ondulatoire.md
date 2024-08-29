## Modélisation de l'onde lumineuse
La lumière peut avoir un comportement corpusculaire comme un comportement ondulatoire.
### La lumière
La lumière est une onde électromagnétique mais elle sera décrite de manière scalaire. Le [[champ]] support de l'onde optique est le champ électrique.
### Expression de l'onde scalaire 
On va se servir des ondes harmoniques.
L'onde sera émise de la source $S$ et arrive le long d'un rayon lumineux jusqu'à au point $M$.
$s(M,t) = S(M)\cos(\omega (t-t_{SM})) = S(M)\cos(\omega t - \omega t_{SM}) = S(M)\cos(\omega t - \varphi_{SM})$ 
#### Durée de transmission du signal $dt$ et $t_{SM}$ 
Élémentaire : $\displaystyle dt = \frac{dl}{v(M)} = \frac{n \, dl}{c}$ 
Macroscopique : $\displaystyle t_{SM} = \int_{S}^{M} dt$ 
#### Retard de phase
$\displaystyle \varphi _{SM} = \omega t_{SM} = k \cdot (SM) = \frac{2\pi}{\lambda _{0}} (SM)$
### Chemin optique
Distance parcouru par la lumière dans le vide pendant $dt$ ou $t_{SM}$ :
Élémentaire : $n \, dl = c \,dt$ 
Macroscopique : $\displaystyle (SM) = \int_{S}^{M} n \: d{l} = \int_{S}^{M} c \: d{t} = c t_{SM}$
#### Propriétés
- En milieu homogène $(M_{1}M_{2}) = n \cdot  \widehat{M_{1}M_{2}}$ 
- Longueur d'onde dans le milieu : $k n = k' = \frac{2\pi}{\lambda }$ alors $\lambda = \frac{\lambda_{0}}{n}$ 
- Différence de marche : différence des chemins optiques parcourus entre $S$ et $M$ le long des deux rayons.
	- $\delta = (SM)_{1} - (SM)_{2}$ 
	- Déphasage entre les deux rayons : $\varphi = k \delta$

## Propagation de l'onde lumineuse
### Surfaces d'onde
On appelle surface d'onde l'ensemble des points de même chemin optique depuis la source.
- Pour une onde monochromatique c'est aussi une surface équiphase.
#### Milieu dispersif 
Dans un milieu dispersif les ondes ne se déplacent pas toutes à la même vitesse.
- Un telle milieu déforme les surfaces d'onde.
### Théorème de Malus
Les rayons lumineux sont orthogonaux aux surfaces d'onde.
### Ondes planes 
Onde dont les surfaces d'onde sont des planes.
- $s(t) = S_{0}\cos(\omega t - k(SM))$
- L'amplitude de l'onde est constante, même surface atteinte par la même énergie.
### Ondes sphériques 
Onde dont les surfaces d'onde sont des sphères. La source  est pontuelle et au centre des surfaces d'onde.
- $s(t) = \frac{S_{0}}{r} \cos(\omega t - k(SM))$
- L'amplitude varie en $\frac{1}{r}$, car la surface d'onde augmente pour la même énergie. 
### Lentilles minces 
![[image lentille mince.png]]
Une lentille permet la transformation d'onde sphérique en onde plane et inversement.
### Notion d'image 
Si $A$ et $A'$ sont conjugués au travers de $(S)$, le chemin optique de $A$ à  $A'$ ne dépend pas du rayon suivi. 
- Pour les rayons ET pour les surfaces d'onde les images virtuelles sont des points de divergence et les images réelles sont des points de convergence. 
- Les variations des propriétés du milieu peuvent provoquer déformations des surfaces d'onde.

## Modèles d'émission des ondes : trains d'onde
Les émissions lumineuses se font, non en continu, mais en bouffées successives à un rythme extrêmement élevé.
### Modèle simple 
Un train d'onde représente une émission cohérente de lumière. On modélise avec une OPPH :
$s_{i} (M,t) = S_{0i}\cos(\omega t -k(SM) + \varphi_{i})$
![[image train donde.png]]
- Durée : $\tau_{c}$
- Extension spatial : $L_{c} = v \tau_{c}= \frac{c}{n} \tau_{c}$ 
- Phase  initial du train : $\varphi _{i}(t)$
	- C'est aléatoire.
#### Contraintes d'interfèrence 
Si la différence de marche entre rayons est trop grande : $\delta > L_{c}$ les rayons ne se croissent pas, donc l'interférence est impossible.
- Deux points sources émettent des trains d'onde avec des phases initiales différent donc pas de interférence.
### Modèles plus élaborés 
Le train d'onde a une naissance et une extinction progressive.
#### Spectre rectangulaire
On voit la relation : $\displaystyle  \Delta t \Delta f \approx 1$.
- Ordre de grandeur de la durée d'émission : $\Delta t$ (semblable à $\tau_{c}$).
- Ordre de grandeur de la largeur spectrale : $\Delta f$.
#### Spectre Gaussien 
On constate encore que $\Delta t \Delta f \approx 1$ 
- Plus une source spectrale est à spectre étroite, plus le train d'onde est long en durée et en longueur.
#### Ordres de grandeur 
![[image ordres train donde.png]]
En différentient $\displaystyle f = \frac{c}{\lambda }$ on trouve :
$\displaystyle\Delta f = \frac{c \cdot \Delta \lambda }{\lambda ^{2}}$ 

## Intensité lumineuse et détecteurs 
### Différents capteurs, rapidité 
Un capteur optique quadratique fournit un signal proportionnel à l'énergie lumineuse reçue pendant le temps d'intégration. 
### Éclairement
Elle rend compte de l'énergie lumineuse par unité de temps et de surface qui illumine un endroit, elle correspond au vecteur de Poynting.
$\mathcal{E} = <s^{2}>$,       $\mathcal{E} = \frac{S_{0}^{2}}{2}$ 
- On prend la moyenne car les variations sont trop rapides pour les capteurs quadratiques.

## Interférences lumineuse 
### Superposition de 2 ondes incohérentes entre elles 
Soit $\mathcal{E}$ l'éclairement de la composition de deux ondes $s = s_{1} + s_{2}$ issues du même point :
$\mathcal{E} = \left< s^{2} \right> = \left< s_{1}^{2}\right> + \left< s_{2}^{2} \right> + \left<2 s_{1}s_{2} \right>$
$\mathcal{E}= \mathcal{E}_{1} + \mathcal{E}_{2} + 4 \sqrt{\mathcal{E}_{1}\mathcal{E}_{2}} \left<\cos(\omega _{1}(t-t_{1}) + \varphi _{1})\cos(\omega _{2} (t-t_{2}) + \varphi _{2})  \right>$
On analyse le terme d'interférence : 
- Si les sources sont trop différents, si $t_{1}$ et $t_{2}$ sont trop différents ou si les pulsations sont différentes : la rélation de phase et quelconque et donc les ondes sont incohérentes et la moyenne est nulle. Alors :
$\mathcal{E} = \mathcal{E}_{1} + \mathcal{E}_{2}$ 
### Interférences à 2 ondes 
Deux rayons lumineux peuvent interférer si :
- Ils sont issus du même point source. 
- Ils ont la même fréquence : $\omega _{1} = \omega _{2}$.
- Ils ont été émis dans le même train d'onde : $\delta < L_{c}$.
#### Formule de Fresnel 
$\mathcal{E} = \mathcal{E}_{1} + \mathcal{E}_{2} + 2 \sqrt{\mathcal{E}_{1} \mathcal{E}_{2}}\cos(\varphi)$ 
Et si $\mathcal{E}_{1} = \mathcal{E}_{2} = \mathcal{E}_{0}$ on a la formule réduit : 
$\mathcal{E} = 2\mathcal{E}_{0}(1+\cos(\varphi))$
### Franges, ordre d'interférence et contraste 
#### Franges
Franges brillantes : Interférences constructives si $\varphi = p\cdot 2\pi$.
- $p$ un entier.
Franges sombres : Interférences destructives si $\varphi= p \cdot 2 \pi$.
- $p$ un multiple de $\frac{1}{2}$.
Pour trouver le nombre de franges on utilise :
- $N = 1+2\lfloor p_{max} \rfloor$  
#### Ordre d'interférence 
$\displaystyle p = \frac{\varphi }{2\pi} = \frac{\delta }{\lambda _{0}}$
#### Contraste 
$\displaystyle C = \frac{\mathcal{E}_{max} - \mathcal{E}_{min}}{\mathcal{E}_{max} + \mathcal{E}_{min}}$ 
- $C \in [0,1]$
- L'éclairement est parfait ($C=1$) si $\mathcal{E}_{min} = 0$.