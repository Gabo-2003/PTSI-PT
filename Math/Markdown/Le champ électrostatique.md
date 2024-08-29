---
tags:
  - electrostatique
---
## Le [[Champ]] électrostatique 
### [[Champ]] d'une charge ponctuelle 
$\displaystyle \overrightarrow{E_{1}}(M) = \frac{1}{4 \pi \epsilon_{0}} \frac{q_{1}}{M_{1}M^{3}} \cdot \overrightarrow{M_{1}M}$  en $V \cdot m^{-1} = N \cdot C^{-1}$ 
- $\displaystyle \frac{1}{4 \pi \epsilon _{0}} = 9,0 \cdot 10^{9} \; F^{-1}$ 
- $\epsilon _{0}$ en $F \cdot m ^{-1}$ 
### Force coulombienne 
$\displaystyle \overrightarrow{F_{1\to2}} = \frac{1}{4 \pi \epsilon _{0}} \frac{q_{1}q_{2}}{M_{1}M_{2}^{3}}\cdot \overrightarrow{M_{1}M_{2}} = q_{2}\cdot \overrightarrow{E}_{1}(M_{2})$
### Principe de superposition 
$\displaystyle \overrightarrow{E}_{tot}(M) = \sum_{p} \overrightarrow{E_{i}}(M)$
 
## Description continue d'une distribution de charges 
### Différentes descriptions continues 
#### Densités linéiques 
Charge par unité de longueur porté par un fil. 
$\displaystyle \lambda (M) = \frac{\delta q}{dl}$ en $C \cdot m^{-1}$ 
#### Densité surfacique 
Charge par unité de surface portée par la nappe. 
$\displaystyle \sigma (M) = \frac{\delta q}{dS}$ en $C \cdot m^{-2}$ 
#### Densité volumique 
Charge par unité de volume considéré. 
$\displaystyle \rho(M) = \frac{\delta  q}{d\tau}$ 
==Le champ électrique est continue pour une distribution volumique.==
### Passage d'une description à une autre 
Exemple pour un cylindre :
- Linéique : $\displaystyle \lambda  = \frac{Q}{l}$ 
- Surface  $\displaystyle \sigma  = \frac{Q}{2 \pi R l} = \frac{\lambda }{2 \pi R}$
- Volumique : $\displaystyle \rho = \frac{Q}{\pi R^{2}l} = \frac{2 \sigma }{R} = \frac{\lambda }{\pi R^{2}}$

## Raisonnements de symétrie et d'invariance 
### Symétrie 
![[image symetrie elec.png|200]]
Pour tout point $M \in \pi_{s}$, le champ électrostatique global n'a que des composantes dans le plan.
$sym_{\pi_{s}}(\overrightarrow{E}(M)) = \overrightarrow{E}(sym_{\pi_{s}}(M))$
### Antisymétrie 
![[image antisymetrie elec.png|200]]
Pour tout point $M \in \pi_{a}$, le champ électrostatique totale est orthogonal au plan.  
$sym_{\pi_{a}}(\overrightarrow{E}(M)) = -\overrightarrow{E}(sym_{\pi_{a}}(M))$
### Les invariances 
Si la distribution est invariante par translation ou rotation suivant un axe. $\lVert \overrightarrow{E} \rVert$ ne dépend pas de la variable linéaire ou rotationnelle respective.

## Théorème de Gauss 
### Flux du champ électrostatique 
$\displaystyle \phi = \int \int_{(S)} d \phi = \int \int_{(S)} \overrightarrow{E} \cdot \overrightarrow{dS}$
### Théorème de Gauss
Le flux du champ électrostatique sortant d'une surface fermée est égal à la charge contenu dans cette surface divisée par la permittivité du vide $\epsilon _{0}$ 
- $\displaystyle \phi = \oint \oint \overrightarrow{E} \cdot \overrightarrow{dS} = \frac{Q_{int}}{\epsilon _{0}}$ 
- La surface de Gausse doit respecter les plan de symétrie.
#### Surface fermée 
Elle a un intérieur et un extérieur : on passe de l'un à l'autre en traversant la surface. 

## Méthode pour les problèmes de symétrie haute 
1- Les symétries déterminent la direction du champ $\overrightarrow{E}$. 
2- Les invariances déterminent les dépendances de la norme $\lVert \overrightarrow{E} \rVert$.
3- On choisie une surface de Gauss $(S)$ qui respecte les symétries. 
4- On calcule le flux $E$ au travers de $(S)$. 
5- On calcule $Q_{int}$ dans les différents cas. 
6- On applique le théorème de Gausse
Pour les problèmes de symétrie plus basse, on utilise le théorème de superposition. 

## Champ des surfaces classiques 
### Plan
si $z>0$ : $\displaystyle \overrightarrow{E} = \frac{\sigma}{2 \epsilon_{0}}$ 
si $z<0$ : $\displaystyle \overrightarrow{E} = -\frac{\sigma}{2 \epsilon_{0}}$ 


