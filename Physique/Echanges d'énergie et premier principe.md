#chapitre22 #thermodynamique 
- $A$ grandeur extensive 
- $a = \frac{A}{m}$ grandeur massique
- $A_{m}=\frac{A}{n}$ grandeur molaire
## Transformation d'un système thermodynamique 
Une transformation thermodynamique est le passage d'un système d'un état d'équilibre initial à un état d'équilibre final.
### Classification des transformations 
#### Isochore 
Volume du système constante : $dV=0$  et  $\Delta V=0$ 
#### Isobare 
Pression du système constante : $dP=0$  et  $\Delta P=0$ 
#### Isotherme 
Température du système constante : $dT=0$  et  $\Delta T=0$ 
#### Monobare 
Pression du système uniforme et constante : $dP \neq 0$  et  $\Delta P=0$ 
#### Monotherme 
Température du système uniforme et constante : $dT \neq 0$  et  $\Delta T=0$ 

## Travail des forces de pression
$\delta W = -P_{ext}dV$ 
- $\delta W > 0 \Leftrightarrow dV < 0$   et inversement. 
- Expression valable si la pression extérieur est uniforme. 
### Transformation mécanique réversible 
Transformation au cours de laquelle $P(t)=P_{ext}(t)$. 
- Travail reçue par le système : aire sous la courbe $P(V)$ dans un [[Description micro et macro d'un système en équilibre#Diagramme de Clapeyron $(P, V)$|diagramme de Clapeyron]]. 
- $W$ positif si le volume final est plus petit que l'initial, négatif dans le cas contraire. 
![[image transformation reversible.png]]
- $W>0$ cycle récepteur
- $W<0$ cycle moteur 
![[image transdormation recepteur et moteur.png]]

## Transfert thermique
C'est l'échange  de l'énergie thermique entre un système et le milieu extérieur sans l'intervention d'une action mécanique mesurable macroscopiquement.  
- $Q$ : Energie thermique échangée par le système. 
### Modes de transfert 
Rayonnement, conduction et convection. 
### Transformation adiabatique 
Transformation au cours laquelle il ne se produit aucune échange thermique entre le système et l'extérieur : $Q=0$
### Thermostat 
Un système est en contact avec un thermostat si les échanges thermiques et mécaniques sont possibles mais la température du thermostat reste constante. 
- C'est le cas si la [[Description micro et macro d'un système en équilibre#Capacité thermique à $V$ constante|capacité thermique]] du système et négligeable devant celle du thermostat. 

## Premier principe de la thermodynamique 
### Conservation de l'énergie d'un système isolé 
$\Delta E_{\Sigma}=- \Delta E_{\overline{\Sigma}}$ 
### Premier principe 
Soit un système fermé, il existe une grandeur $U$ telle que $U$ est une [[Description micro et macro d'un système en équilibre#Variables et équations d'état|fonction d'état]] extensive et :
- $\Delta E_{m}+ \Delta U = W + Q$
- $\Delta U = W + Q$
- $\Delta dU = \delta W + \delta Q$
### Calcule du transfert thermique $Q$
Cas isochore avec la seule travail la pression : $Q=\Delta U$ 

## Enthalpie 
Cas d'une transformation isobare
- $\Delta H = Q$
- $H=U+PV$ 
### Capacité thermique à pression constante 
#### Gaz parfait 
$\Delta H= C_{p}\Delta T$
- $H_{GP}=\frac{5}{2}nRT$ 
- $C_{p}= \frac{\partial H_{GP}}{\partial T}|_{P} = \frac{5}{2}nR$ 
#### Phase condensée incompressible indilatable 
- $H_{m}=H_{m}(T)$
- $C_{p,m} = C_{v,m}$ 
### Enthalpie de changement de phase
- $\Delta_{\alpha \beta}H_{m}=H_{m}(\beta)- H_{m}(\alpha)$  en  $J \cdot mol^{-1}$  