---
tags:
  - electrostatique
---
## Potentiel d'une charge ponctuelle et d'une distribution
### Charge  [[Le champ électrostatique#Champ d'une charge ponctuelle|ponctuelle]]
$\displaystyle \overrightarrow{E} = \frac{1}{4 \pi \epsilon _{0}} \frac{q}{r^{2}} \overrightarrow{e_{r}}$       or   $\overrightarrow{grad}(\frac{1}{r}) = - \frac{1}{r^{2}}\overrightarrow{e_{r}}$ alors : 
$\displaystyle \overrightarrow{E} = -\frac{1}{4 \pi \epsilon _{0}} \overrightarrow{grad}(\frac{1}{r})=- \overrightarrow{grad}\left(\frac{1}{4 \pi \epsilon _{0}r}\right)$
#### Potentiel électrostatique
$\displaystyle V(M) = \frac{q}{4 \pi \epsilon _{0} r }$   donc 
$\displaystyle \overrightarrow{E}(M) = - \overrightarrow{grad}(V(M))$
### Distribution discrète 
On utilise le [[Le champ électrostatique#Principe de superposition|principe de superposition]] pour trouver le potentielle de $N$ charges ponctuelles : 
- $V(M) = \sum_{N} V_{i}(M)$ 
### Calcule de $V$ à partir d'une circulation 
$dV = - \overrightarrow{E} \cdot d \overrightarrow{OM}$ 
$\displaystyle \implies V(M) - V(M_{0}) = - \int_{M_{0}}^{M} \overrightarrow{E}(M) \cdot d \overrightarrow{OM}$
## Application 
### Condensateur plan
![[image condensateur plan.png|200]]
On fait l'hypothèse que le condensateur est fait par deux plaques où on néglige les effets de bord. Il faut vérifier : $e << \sqrt{S}$ 
On utilise l'[[Signaux électiques dans l'ARQS#Condensateurs (récepteur)|expression]]  $\displaystyle Q=CU \Leftrightarrow C = \frac{Q}{U}$
- $Q = \sigma S$
- $\displaystyle U = V\left(\frac{e}{2}\right) - V\left(- \frac{e}{2}\right) = \frac{\sigma }{\epsilon _{0}} e$
Alors on trouve : $\displaystyle C = \frac{S \epsilon _{0}}{e}$
## Cartes de champ
![[Champ#Elements d'un champ]]


## Énergie potentielle électrostatique 
$\overrightarrow{F} = q \overrightarrow{E} = q \overrightarrow{grad}(V) = \overrightarrow{grad}(qV)$, et d'après 
![[Etude énergétique#Forces conservatives]] 
Alors $E_{p} = qV$
## Équations locales  
### Équation de Maxwell-Gauss
$\displaystyle div(\overrightarrow{E}) = \frac{\rho}{\epsilon_{0}}$
- [[Operateurs différentiels#Divergence|Divergence]]
### Équation de Poisson
On combine :
- L'équation de Maxwell-Gauss : $div(\overrightarrow{E}) = \frac{\rho}{\epsilon _{0}}$ 
- La relation entre le champ électrique et son potentiel : $\overrightarrow{E} = - \overrightarrow{grad}(V)$ 
On trouve : $\displaystyle \Delta V = - \frac{\rho}{\epsilon _{0}}$
### Équation de Laplace 
Lorsque l'espace est sans charge on trouve :
$\Delta V = 0$