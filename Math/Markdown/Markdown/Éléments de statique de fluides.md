---
tags:
  - meca_fluides
---
Les variables [extensives] : $\delta$ 
Les variables [intensives] : $d$
## Forces surfaciques, volumiques, [[champ]] de pression
### Force volumiques
Ils s'exercent dans l'ensemble du volume d'un système. Ils peuvent donc être définis avec une densité volumique de force $\overrightarrow{f_{v}}$ et un volume élémentaire $\delta V$.
- $\delta \overrightarrow{F} = \overrightarrow{f_{v}} \cdot \delta  V$
### Force surfacique et champ de pression
- $Pa \sim N \cdot m^{-2}$ 
Force élémentaire qui s'exerce sur une surface élémentaire :
- $\delta  \overrightarrow{F_{p}}(M) = P \cdot \overrightarrow{dS}$
La surface $\overrightarrow{dS}$ est définie comme un vecteur :
- Norme : mesure la surface (exemple $dxdy$)
- Direction : $\perp$ à la surface qui est localement plane
- Sens : Peut être entrant ou sortant 

## Statique dans le [[champ]] de pesanteur uniforme
### Théorème fondamental de la statique de fluides
A l'équilibre mécanique, on a le théorème fondamentale de la statique des fluides appliquée à la atmosphère isotherme :
- $\displaystyle \frac{dP}{dz} = -\mu  g$      qui est aussi    $\overrightarrow{grad} P = \overrightarrow{f_{v}}$
### Atmosphère [[Echanges d'énergie#Isotherme|isotherme]] 
On part de la relation fondamentale de la statique de fluides et l'équation d'état d'un gaz parfait et on trouve : 
$\displaystyle P(z) = P_{0} \exp\left(-\frac{Mg}{RT} z\right) \implies \mu (z) = \mu _{0} \exp\left(-\frac{Mg}{RT} z\right)$
#### Interprétation 
On pose $\displaystyle H = \frac{RT}{Mg}$ hauteur d'échelle
- $\displaystyle P(z) = P_{0} \exp(- \frac{z}{H})$ au bout de $z = \text{quelque  } H$ l'atmosphère est nulle.
### Fluide incompressible 
Si on considère un [[Fluide en écoulement stationnaire dans une conduite#Fluide incompressible|fluide incompressible]] alors :
- $\displaystyle \mu = \text{cst} / \text{espace} \implies \frac{d P}{dz} = - \mu  g = \text{cte}$
Alors en intégrant on trouve :
- $P(z) = P_{0} - \mu g z$
#### Propriétés et applications 
##### Théorème de Pascal
![[image theoreme de pascal.png]]

Les fluides homogènes transmettent les pressions à altitude constante :  $P(z)= \text{cte}$
##### Presse hydraulique 
(photo)
$F' = \Delta P \cdot S = F \cdot \frac{S}{s}$ 

## Résultant des forces de pression 
D'après le [[Champ magnétique#Principe de Curie|Principe de Curie]] : la force résultante des actions de pression est incluse dans tout plan de symétrie. 
Pour la calculer, on choisie un système de coordonnées adapté et on fait un découpage infinitésimal de la surface. On somme (en intégrant) toutes les forces infinitésimal.
### [[Dynamique Newtonienne#Poussée d'Archimède|Poussée d'Archimède]] 
Il devrait être considère que en statique.
Le centre de gravité de l'objet (Point d'application du poids) et le centre de gravité du volume déplacé (point d'application de la pousse d'Archimède) ne sont pas forcement le même. 
$\overrightarrow{\Pi} = m_{déplacé} \cdot g \overrightarrow{e_{z}}$
