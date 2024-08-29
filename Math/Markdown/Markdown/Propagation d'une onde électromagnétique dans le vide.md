---
tags:
  - electromagnetique
---
## Propagation du champ électromagnétique dans le vide
### Equations de Maxwell dans le vide
Les équations dans le vide s'écrivent en absence de charge et de courant.
### Equations de propagation des champs  
On utilise la relation  $\overrightarrow{rot} (\overrightarrow{rot} (\overrightarrow{X})) = \overrightarrow{grad}(div(\overrightarrow{x})) - \Delta \overrightarrow{X}$ (pas a connaître) et les [[Équations de Maxwell#Les équations de Maxwell|équations de Maxwell]] dans le vide pour trouver les équations de propagation des champs :
Equations de D'Alembert :
- $\displaystyle \Delta \overrightarrow{E} = \mu_{0} \epsilon_{0} \frac{\partial ^{2} \overrightarrow{E}}{\partial t^{2}}$ 
- $\displaystyle \Delta \overrightarrow{B} = \mu_{0} \epsilon_{0} \frac{\partial ^{2} \overrightarrow{B}}{\partial t^{2}}$
On pose $\displaystyle \mu_{0} \epsilon_{0} = \frac{1}{c^{2}}$ avec $c$ qui est la vitesse de propagation de $(\overrightarrow{E}, \overrightarrow{B})$.

## Onde plane progressive (OPP)
![[image OPP.png|300]]

### Définitions 
On suppose que la propagation de l'onde est selon $Ox$
#### Onde plan
Onde dont les surfaces d'onde sont des plans orthogonaux à une direction $\overrightarrow{u}$ fixe.
Dans le plan $x = cste$, les champs électrique et magnétique sont identiques. 
Alors ces champs ne dépendent que d'une variable de espace et de temps.
#### Onde progressive
Onde de la forme $\displaystyle \overrightarrow{G}(t- \frac{x}{c})$.
Soit $\overrightarrow{F}$ et $\overrightarrow{G}$ deux ondes progressives : 
$\displaystyle \overrightarrow{E} = \underbrace{\overrightarrow{F}(t+ \frac{x}{c})}_{\text{Sens décroissante}} + \underbrace{\overrightarrow{G}(t - \frac{x}{c})}_{\text{Sens croissante}}$
Alors $\overrightarrow{E}$ et $\overrightarrow{B}$ sont les superpositions de deux ondes progressives se déplaçant en sens inverse.
### Propriétés  
#### L'onde plane est transverse
Le champ électromagnétique $(\overrightarrow{E},\overrightarrow{B})$ d'une onde plane est transverse : les deux champs sont inscrites dans le plan d'onde
#### Structure de l'onde plane progressive 
- $\displaystyle \overrightarrow{E} = c \overrightarrow{B} \wedge \overrightarrow{u_{prop}}$
- $\displaystyle \overrightarrow{B} = \frac{\overrightarrow{u_{prop}}\wedge\overrightarrow{E}}{c}$
- Le trièdre $(\overrightarrow{E}, \overrightarrow{B}, \overrightarrow{u_{prop}})$ est direct.

En notation complexe : $\displaystyle \overrightarrow{\underline{B}} = \frac{\overrightarrow{k} \wedge \overrightarrow{\underline{E}}}{\omega}$ 
## Onde plane progressive harmonique $(OPPH)$
![[image OPPH.png|400]]
### Forme générale 
Le principe de superposition nous permet d'étudier les signaux réels à partir des signaux harmoniques plus simples à manipuler.
On a la forme générale :
$\overrightarrow{E} = E_{0} \cos\left( \omega t - \omega \frac{x}{c} \right) \overrightarrow{u}$
Vecteur d'onde : $\overrightarrow{k} = \frac{\omega }{c} \overrightarrow{u_{prop}}$
Amplitude du champ magnétique : $B_{0} = \frac{E_{0}}{c}$ 
### Notations complexes 
- $\displaystyle \underline{\overrightarrow{E}} = E_{0} \exp(i (wt -kx))\overrightarrow{u_{E}}$ 
- $\displaystyle \underline{\overrightarrow{B}}  = \frac{E_{0}}{c} \exp(i (\omega t -kx)) \overrightarrow{u_{B}}$ 
Avec $\overrightarrow{E} = Re(\underline{\overrightarrow{E}} )$ et $\overrightarrow{B} = Re(\underline{\overrightarrow{B}} )$
Le vecteur $\overrightarrow{\nabla }$ devient $-i \overrightarrow{k}$. 
On peut réécrire les équations de Maxwell avec cette vecteur.
On peut aussi retrouver les propriétés de la structure d'une onde plane (trièdre, relations avec le vecteur propagation). 
### Relation de dispersion
En injectant l'expression d'un champ harmonique dans l'équation d'onde on trouve la relation de dispersion : 
$\displaystyle  k^{2} = \frac{\omega ^{2}}{c^{2}}$
- Elle est valable même si l'onde n'est pas une OPPH.
### Longueur d'onde
Période spatial de l'onde. 
Nombre d'onde : $\displaystyle  \sigma = \frac{1}{\lambda }$
On a pour le vecteur d'onde : $\displaystyle k =\frac{2\pi}{\lambda } = 2\pi \sigma  \quad \propto \quad \omega  = \frac{2\pi}{T} = 2\pi f$
### Vecteur de Poynting et flux d'énergie
$\displaystyle \overrightarrow{v_{e}} = \frac{\langle \overrightarrow{\Pi} \rangle}{\langle e \rangle}= c \; \overrightarrow{u_{prop}}$  
Alors $c$, la vitesse de propagation de la phase, est aussi dans le vide la vitesse de propagation de l'énergie portée par l'onde électromagnétique. 
### Les différentes gammes d'ondes électromagnétiques 
![[image gamme ondes.png]]

## État de polarisation d'une onde
On parle d'onde polarisé lorsque l'extrémité du vecteur $\overrightarrow{E}$ dessine une courbe stable dans le temps. 
### Cas générale
La lumière naturelle n'est pas polarisée, ce sont des paquets d'onde. Elle peut se polariser totalement ou partiellement par réflexion, diffusion, transmission...
### Polarisation elliptique 
Le cas le plus génerale.
### Polarisation rectiligne
Si les deux composantes du champ $\overrightarrow{E}$ ont un déphasage de $\varphi = 0 [\pi]$.
La différence d'amplitude entre les composantes fait varier l'inclination de la droite.
### Polarisation circulaire
Si les deux composantes du champ $\overrightarrow{E}$ ont la même amplitude et un déphasage de $\varphi = \frac{\pi}{2} [\pi]$
### Polariseur par absorption 
Fait par des lames dichroïques. C'est une polarisation par absorption qui permet de ne conserver qu'une composante du champ électrique selon une direction: en sortie, l'onde est polarisée rectilignement. 
### Loi de Malus
Soit une onde polarisé rectilignement de intensité lumineuse $I_{0}$ entrant dans le polariseur et d'intensité sortant $I$. 
Soit $\theta$ l'angle entre la polarisation de l'onde incident et l'axe du polariseur. 
Alors on a la relation : $I = I_{0}\cos^{2}(\theta)$ 
