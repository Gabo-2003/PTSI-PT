## Bilan sur les fluides écoulement stationnaire traversant un dispositif 
### Système à une entrée et une sortie : bilan d'enthalpie 
On considère un écoulement stationnaire, alors le débit volumique $D_{v}$ d'entrée n'est pas forcement le même que en sortie. Par contre, par conservation de la masse et stationnarité, le débit massique $D_{m}$ se conserve. 
$\displaystyle q = \frac{Q}{\Delta m}$   et   $\displaystyle \dot{Q} = \frac{Q}{\Delta t}$ 
Puissance thermique : $\implies  \dot{Q} = q \cdot D_{m}$ 
De la même manière on trouve la puissance mécanique : $\dot{W} = w \cdot D_{m}$
#### Bilan d'enthalpie
Premier principe sur le système $\Sigma$ entre $t$ et $t+dt$ :
$dU + dE_{M} = P_{1} \delta V_{1} - P_{2}\delta V_{2} + w \delta m + q \delta m$
Maintenant on utilise l'expression : 
$dU = U(t+ dt) - U(t) = (U_{0} + u_{2} \delta m) - (U_{0} + u_{1} \delta m) = (u_{2} -u_{1})\delta m$
Avec le même raisonnement on trouve :
$dE_{M} = (e_{M2} - e_{M1})\delta m$ 
On injecte dans la premier expression :
$(u_{2} -u_{1})\delta m + (e_{M2} - e_{M1})\delta m = P_{1} \delta V_{1} - P_{2}\delta V_{2} + w \delta m$
$\implies (u_{2}+P_{2}v_{2} + e_{M2}) - (u_{1}+P_{1}v_{1} + e_{M2}) = q + w$
$\implies \boxed{\Delta h + \Delta e_{M} = w + q}$
Et si on multiplie par $D_{m}$ :
$\implies \boxed{D_{M}(\Delta h + \Delta e_{M}) = \dot{W} + \dot{Q}}$ 
#### Bilan d'entropie
Avec le même raisonnement on trouve :
$\boxed{\Delta s = \frac{q}{T_{source}} + s_{c}}$ 
Et si on multiplie par $D_{m}$ :
$\implies \boxed{D_{m} \Delta s = \frac{\dot{Q}}{T_{source}} + \dot{S_{c}}}$
### Systèmes à plusieurs entrées et sorties 
Par conservation du débit massique :
$\displaystyle \sum D_{me,i} = \sum D_{ms,j}$ 
$\implies \boxed{ \sum_{\text{sorties}} D_{mi} (h_{i}+e_{Mi}) - \sum _{\text{entrées}} D_{mj}(h_{j}+e_{Mj}) = \dot{W} + \dot{Q}}$

## Description de dispositifs élémentaires industrielles 
### Compresseur et turbine calorifugés
#### Compresseur 
Il s'agit dans ce dispositif de mettre un fluide sous pression en faisant appel à un travail extérieur.
- Travail extérieur : $P_{m}<0$
- Fluide pas chauffée : $P_{th}=0$
- Injecté et récupérée sans vitesse notable :  $\Delta e_{c} = 0$
- Même altitude : $\Delta e_{p} = 0$
$D_{m}\Delta h = P_{m} > 0$
#### Turbine
Il s'agit de mettre en mouvement de rotation un arbre en faisant passer un fluide sous pression sur les pales. 
- Fluide pas chauffée : $P_{th}=0$
- Injecté et récupérée sans vitesse notable :  $\Delta e_{c} = 0$
- Même altitude : $\Delta e_{p} = 0$
$D_{m} \Delta h = P_{m} < 0$
### Mélangeur et séparateur isobare calorifugés
#### Mélangeur 
$D_{m1} + D_{m2} = D_{m3}$ 
$D_{m3}h_{3} - (D_{m1}h_{1} + D_{m2}h_{2}) = 0$ 
#### Séparateur 
$D_{m1} = D_{m2} + D_{m3}$
$(D_{m2}h_{2}+D_{m3}h_{3}) - D_{m1}h_{1} =0$
### Échangeur thermique calorifugé
$D_{1}\Delta h_{1} + D_{m2}\Delta h_{2} = 0$
Avec $\Delta h_{1}=q_{1}>0$ réchauffage pour un des fluides.
Et $\Delta h_{2}=q_{2}<0$ refroidissement pour l'autre.
### Détendeur calorifugé
Dispositif qui abaisse la pression d'un fluide par passage dans des parois poreuses rigides
- Pas de pièces mobiles donc pas de travail apporté : $P_{m} = 0$
- Fluide pas chauffée : $P_{th}=0$
- Pas d'apport de vitesse : $\Delta e_{c} = 0$
- Pas de variation d'altitude $\Delta e_{p} = 0$
$D_{m} \Delta h = 0$
### Tuyère calorifugée 
- Pas de travail : $P_{m} = 0$
- Réaction rapide : $P_{th} = 0$
- Pas de variation d'auteur : $\Delta e_{p} = 0$
$D_{m} (\Delta h + \Delta e_{c}) = 0$
### Chaudières 
$D_{m} \Delta h=P_{th}>0$