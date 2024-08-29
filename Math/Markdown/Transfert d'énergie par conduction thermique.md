## Les différents échanges 
Ils sont liées à une différence de température entraînant un flux thermique du corps le plus chaud vers le corps le plus froid (deuxième principe). 
### Conduction 
Caractéristique des échanges thermiques dans les solides. Par excitation des atomes voisins, l'énergie se répand de proche en proche dans le matériau sans déplacement de matière. 
### Convection 
Caractéristique des échanges dans les fluides et aux interfaces solide-fluide. Les mélanges liés aux turbulences homogénéisent la température dans les zones éloignées des parois solides alors que près de ces dernières, les fluides auront tendance à adhérer. 
### Rayonnement 
Seul échange possible à travers le vide. C'est le champ électromagnétique qui est le support de ces échanges. 

## Conduction thermique 
### Flux thermique 
C'est la quantité de chaleur qui traverse une surface par unité de temps. 
$\displaystyle \delta \phi = \frac{\delta Q}{ dt}$ en $W$.
Densité du flux :  $\displaystyle \overrightarrow{j}_{th} = \frac{\delta Q}{dS dt} \overrightarrow{e}$  en $W \cdot  m^{-2}$
- $\displaystyle \phi = \iint_{S} \overrightarrow{j}_{th} \cdot d\overrightarrow{S}$
- $\overrightarrow{e}$ est dirigé par la direction de flux surfacique maximal et par le sens de l'échange de $\delta Q$ (chaud vers froid). 
### Loi de Fourier 
Elle exprime la proportionnalité de $\overrightarrow{j}_{th}$ et du gradient de $T$.
$\overrightarrow{j}_{th} = - K \, \overrightarrow{grad}(T)$ 
- Conductivité thermique du matériau : $K$ en $W \cdot m^{-1} \cdot K^{-1}$.
### Équation de diffusion en cartésiennes
Il faut savoir la démontrer en faisant un bilan sur un volume élémentaire. 
$\displaystyle K \frac{\partial ^{2} T}{\partial x^{2}} = \rho c \frac{\partial T}{\partial t} \implies \frac{\partial T}{\partial t} = D \frac{\partial ^{2}T}{\partial x^{2}}$ 
- Coefficient de diffusion thermique : $\displaystyle D = \frac{K}{\rho c}$ en $m^{2} \cdot s^{-1}$.
- Cette équation traduit un phénomène irréversible. 
- $R_{cond} = \frac{e}{KS}$ 
#### Solution stationnaire : cas d'une vitre
Dans cette type de problème on prend pas en compte la convection. La température à l'extérieur et à la surface extérieur du vitre n'est pas la même.
$\displaystyle T(x) = T_{i} + \frac{T_{i}-T_{e}}{e} x$
### Analogie électrique 
![[image analogie elec thermo.png]]
Quand un flux traverse plusieurs milieux, on peut faire une analogie avec des dipôles en série. 
Pour ajouter plusieurs flux, c'est pareils qu'ajouter plusieurs dipôles en parallèle. 
### Cas général 
On peut trouver un ordre de grandeur du problème avec $D = \frac{L^{2}}{\tau}$ avec $L$ la longueur caractéristique du problème et $\tau$ le temps caractéristique du phénomène. 

## Convection 
### Loi de Newton
C'est une loi expérimental. 
$\Phi = h (T_{p}-T_{f})S$
- Surface d'échange : $S$.
- Coefficient de convection : $h$ en  $W \cdot m^{-2} \cdot K^{-1}$.
#### Interprétation physique
Conduction dans la couche limite d'écoulement laminaire du fluide.
D'après la loi de Fourier : 
$\displaystyle  \phi = - K_{f} \frac{\Delta T}{\Delta x} = \frac{K_{f}}{e} (T_{p} - T_{f})S$
- Epaisseur de la couche laminaire : $e$. 
- Conductivité du fluide :  $K_{f}$.
Alors on identifie $\displaystyle h = \frac{K_{f}}{e}$. Plus la couche est petite (plus l'écoulement est turbulent) plus $h$ augmente. 