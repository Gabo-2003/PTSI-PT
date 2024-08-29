#chapitre25 #thermodynamique 
## Second principe et entropie
### Transformation réversible 
Il est possible de ramener le système et son environnement exactement dans l'état initial.
- Les contraintes extérieures varient continument et lentement, on considère que le système est toujours à l'équilibre (quasi-statique).
- Un changement infinitésimal suffit à inverser le sens de la transformation. 
### Entropie 
Correspond à une mesure du désordre de ce système à l'échelle microscopique. Mesure l'évolution irreversible des phénomènes naturels. 
- L'entropie d'un système isolé est créable et indestructible.
### Second principe 
Pour un système fermé, il existe une fonction d'état $S$ extensible tel que :
$S = S_{ech}+S_{crée}$ 
- $S_{crée}=0$ : Transformation réversible. 
- $S_{crée}>0$ Transformation irréversible. 
- $\displaystyle S_{éch} = \sum_{i}^{} \frac{Q_{i}}{T_{source,i}}$  Avec $Q_{i}$ la transfert depuis un thermostat à $T_{source,i}$.
#### Pour une transformation infinitésimal
Pour un système fermée: 
$S(t+dt) - S(t) = \boxed{dS = \delta S_{ech} + \delta S_{cree}}$
- $\displaystyle \delta S_{éch} = \sum_{i}^{} \frac{\delta Q_{i}}{T_{source,i}}$
#### Transformation quasi-statique
Dans ce cas $T_{\Sigma}= T_{S}$
- $\displaystyle S_{éch}= \frac{1}{T_{s}} \sum_{i}^{}Q_{i}$
#### Transformation monotherme 
En contact avec un thermostat : $T_{\Sigma}= T_{0}$
- $\displaystyle S_{éch}= \frac{Q}{T_{0}}$ 
### Transformation adiabatique réversible
Dit isentropique 
- Transformation adiabatique : $Q_{i}=0 \Rightarrow S_{éch}=0$ 
- Transformation réversible : $S_{crée}=0$ 
- Application du 2èm principe : $\Delta S = 0$
- La réciproque de tout le précèdent est fausse.

## Entropie d'un corps pur
### Gaz parfait 
#### Coefficient adiabatique 
$\displaystyle \gamma = \frac{C_{p}}{C_{v}}$ 
#### Formule de Mayer 
$C_{p}-C_{v}=nR$
- On en déduit : $\displaystyle C_{v}= \frac{nR}{\gamma -1}$ 
#### Loi de Laplace
Valable pour un gaz parfait et une transformation adiabatique réversible.
- $PV^{\gamma}=cst$        $P^{1-\gamma}\,T^{\gamma}=cst$      $T\,V^{\gamma-1}=cst$ 
### Phase condensée indilatable et incompressible
- $S(T)=nS_{m}(T)=ms(t)$ 
- $\Delta S_{m}=C_{m} \ln(\frac{T}{T_{0}})$ 
### Entropie de changement de phase 
$\displaystyle \Delta_{\alpha \beta}S_{m}= \frac{\Delta_{\alpha \beta}H_{m}}{T}$
