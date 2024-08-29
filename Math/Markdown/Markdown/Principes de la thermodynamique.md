## Premier principe de la thermodynamique 
### Energie interne 
$\displaystyle U= \sum_{\text{tout particule}} E_{c,micro} + E_{p,micro}$ 
### Conservation de l'énergie d'un système isolé 
$\Delta E_{\Sigma}=- \Delta E_{\overline{\Sigma}}$ 
### Premier principe 
Soit un système fermé, [[Description d'un système en équilibre et échanges d'énergie#Energie interne|l'énergie interne]] $U$ est une [[Description d'un système en équilibre et échanges d'énergie#Variables et équations d'état|fonction d'état]] extensive.
#### Macroscopique
- Si on distingue le travail des forces conservatives :
$\Delta E_{m}+ \Delta U = W_{nc} + Q$
- Pour un système au repos :
$\Delta U = W_{nc} + Q$
- Transformation isochore ($V= cte$):
$dU = \delta Q$ 
#### Infinitésimale 
$dU +dE_{c}= \delta W + \delta Q$
- A énergie mécanique constante :
- $dU= \delta W + \delta Q$
### Capacité thermique à volume constante
$\displaystyle C_{V}= \left. \frac{\partial U}{\partial T} \right|_{V}$ 
### Première identité thermodynamique 
$U (V,S): \quad dU = -P \cdot dV + T \cdot dS$
- $\displaystyle  T = \left. \frac{\partial U}{\partial S} \right|_{V}$  et   $\displaystyle  P = \left. \frac{\partial U}{\partial V} \right|_{S}$

## Enthalpie 
C'est une changement de variable de l'énergie interne dans le cas de transformation isobares. On passe de la variable $V$ à $P$.
$H=U+PV$ 
- $dH = \delta Q$
### Capacité thermique à pression constante
$\displaystyle C_{p}= \left. \frac{\partial H}{\partial T} \right|_{P}$
### Deuxième identité thermodynamique 
$H(S,P) : \quad dH = T \cdot  dS +  V \cdot  dP$
### Phase condensée incompressible indilatable 
- $H_{m}=H_{m}(T)$
- $C_{p,m} = C_{v,m}$ 
### Enthalpie de changement de phase
- $\Delta_{\alpha \beta}H_{m}=H_{m}(\beta)- H_{m}(\alpha)$  en  $J \cdot mol^{-1}$  

## Enthalpie libre 
C'est une changement de variable pour avoir une fonction de état en fonction de $P$ et $T$. Valable pour un corps pur. Utile à $T$ et $P$ constante.
- $G(T,P) = H- TS = U + PV - TS$
- $dG = V \cdot  dP - S \cdot  dT$
Pour une mélange :
- $\displaystyle dG = - S \cdot  dT + V \cdot  dP + \sum \left. \frac{\partial G}{\partial n_{i}} \right|_{T,P,n_{i}} dn_{j \neq i}$ 
### Potentiel chimique 
$\displaystyle \mu _{i} = \left. \frac{\partial G}{\partial n_{i}}  \right|_{T,P,n_{j\neq i}} = \left. \frac{\partial H}{\partial n_{i}}  \right|_{P,S,n_{j\neq i}} = \left. \frac{\partial U}{\partial n_{i}}  \right|_{V,S,n_{j\neq i}}$
On a donc (admis) :
$\displaystyle G(T,P,n_{i}) = \sum _{\text{constituantes}}\mu _{i}n_{i}$
#### Pour un Gaz parfait
En fonction de l'[[Description d'un système et évolution vers un état final#Activité d'une espèce chimique|activité]] du constituant :
$\mu _{i} = \mu _{i}^{0}(T) + RT\ln(a_{i})$
### Expression de l'enthalpie libre
 A partir de la $dG$ on peut trouver $dH$ et $dU$ :
 - $dH = T\cdot dS + V \cdot  dP + \sum \mu _{i} dn_{i}$ 
 - $dU = T \cdot  dS - P \cdot  dV + \sum \mu _{i} dn_{i}$
### $G$ et entropie crée
Pour un système au repos à $T$ et $P$ constantes, on trouve a partir de $dG$ :
$dG = - T \delta S_{c}$ 
### Potentiel thermodynamique
Pour une transformation isobare, isotherme et spontanée, $G$ joue le rôle de potentiel thermodynamique : elle est minimale à l'équilibre, comme l'énergie potentielle l'est en mécanique en une position d'équilibre stable. 

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
Dit aussi isentropique.
- Transformation adiabatique : $Q_{i}=0 \Rightarrow S_{éch}=0$ 
- Transformation réversible : $S_{crée}=0$ 
- Application du 2èm principe : $\Delta S = 0$
- La réciproque de tout le précèdent est fausse.
### Entropie d'un corps pur
#### Phase condensée indilatable et incompressible
- $S(T)=nS_{m}(T)=ms(t)$ 
- $\Delta S_{m}=C_{m} \ln(\frac{T}{T_{0}})$ 
#### Entropie de changement de phase 
$\displaystyle \Delta_{\alpha \beta}S_{m}= \frac{\Delta_{\alpha \beta}H_{m}}{T}$

## Utilisation des identités thermodynamiques pour le gaz parfait (corps pur)
### Nature et équation d'état
Molécules ponctuelles sans interactions autre que les chocs.
- $PV = nRT$
### Première loi de Joules
 $\displaystyle U_{GP} = U(T) \longrightarrow dU = \frac{\partial U}{\partial T} dT = C_{V} dT$
 GP monoatomique : $C_{V} = \frac{3}{2} n R$  (3 est le degré de liberté du gaz)
 GP diatomique dans certains conditions : $C_{v} = \frac{5}{2}nR$
### Deuxième loi de Joules 
 $\displaystyle H_{GP} = H(T) \longrightarrow dH = \frac{\partial H}{\partial T} dT = C_{P}dT$
 Coefficient adiabatique : $\displaystyle \gamma = \frac{C_{P}}{C_{V}}$ 
### Loi de Mayer
 $dH = dU + d(PV) \longrightarrow C_{P} dT = C_{V} dT + nR dT$
- $C_{p} - C_{V} = nR$
- On en déduit : $\displaystyle C_{v}= \frac{nR}{\gamma -1}$ 
### Entropie du gaz parfait
A partir de la première identité thermodynamique, la premier loi de joule et l'équation d'état d'un gaz parfait on trouve :
$S(T,V) = C_{v} \ln(T) + nR \ln(V)+cte$
- Avec l'équation d'un gaz parfait on trouve aussi $S(T,P)$ et $S(P,V)$.
### Loi de Laplace
Pour une transformation isentropique d'un gaz parfait de  $\gamma = cte$ /° $T$ :  
- $PV^{\gamma}=cst$        $P^{1-\gamma}\,T^{\gamma}=cst$      $T\,V^{\gamma-1}=cst$ 
### Cas des corps condensés 
Pour un corps indilatable et incompressible ($V=cte$) : $U(T) \approx H(T)$.
- $dH=C dT \approx dU$. 
Et on trouve pour l'entropie a partir de la 1er identité : 
$S =C \ln(T)+cte$. 