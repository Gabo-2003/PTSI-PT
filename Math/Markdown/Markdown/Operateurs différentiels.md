![[image operateurs differentielles cartesiennes.png]]
## Nabla 
$\displaystyle \overrightarrow{\nabla} = \frac{\partial }{\partial x} \overrightarrow{e_{x}}+ \frac{\partial }{\partial y} \overrightarrow{e_{y}}+ \frac{\partial }{\partial z}\overrightarrow{e_{z}}$ 
- Gradient : $\overrightarrow{grad}(S) = \overrightarrow{\nabla}S$
- Divergence : $div(\overrightarrow{S}) = \overrightarrow{\nabla} \cdot \overrightarrow{S}$ 
- Laplacian : $\Delta S = \overrightarrow{\nabla}^{2} S$ 
- Rotationnelle : $\overrightarrow{rot}(\overrightarrow{X}) = \overrightarrow{\nabla} \wedge \overrightarrow{X}$

## Divergence 
On définie la divergence d'un [[champ]] vectoriel comme le flux volumique sortant associé à un vecteur.

## Rotationnel 
### Notion de circulation
Il s'agit de calculer la projection d'un vecteur le long d'une courbe. 
$\displaystyle \int_{A}^{B} x \cdot  d\overrightarrow{OM}$ le longue de $(\mathcal{C})$
### Définition
C'est un vecteur dont les coordonnées sont les circulations surfaciques autour du vecteur unitaire associé. 
- Direction : indique autour de quel axe le vecteur $\overrightarrow{X}$ tourne.
- Sens : Sense de rotation de la circulation positive. 
- norme : valeur absolue de la circulation surfacique. 

## Théorèmes
### Théorème d'Ostrogradski 
On considère une surface fermée $(S)$ qui délimite un volume $(V)$,
$\displaystyle \oint \oint_{(S)}  \overrightarrow{X}\cdot d\overrightarrow{S}_{sortant} = \iiint_{(V)} div(\overrightarrow{X}) \cdot  d \tau$ 
### Théorème de Stokes 
On considère une contour fermée $(C)$ sur lequel s'appui une surface $(S)$ $\displaystyle\oint_{(C)} \overrightarrow{X}(M) \cdot  d \overrightarrow{OM} = \iint _{(S)} \overrightarrow{rot}(\overrightarrow{X}(M)) \cdot d\overrightarrow{S}$

## Différentielle 
Soit $X(x_{1},x_{2},\ldots)$
$\displaystyle dX = \sum_{i} \frac{\partial X}{\partial x_{i}} dx_{i}$ 