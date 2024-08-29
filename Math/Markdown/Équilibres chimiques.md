## G, potentiel thermodynamique à $p$ et $T$ constantes 
On cherche a établir un équilibre chimique à $T$ et $P$ constantes. Alors la variation de $G$ est obtenu par la transposition entre les potentiel chimique des réactifs et des produits. D'après la  [[Principes de la thermodynamique#$G$ et entropie crée|relation]]  entre $G$ et $S$ : 
- Condition d'évolution $dG <0$ : Un système ne peut pas évoluer que dans le sens qui diminue $G$.
- Condition d'équilibre $dG = 0$.
### Condition d'équilibre et d'évolution d'une réaction chimique
$\displaystyle dG = \sum \nu _{i} \mu _{i} \cdot  d\xi  = \Delta _{r}G \cdot  d \xi \leq 0$
- Sens direct : $\Delta _{r}G <0$ et $d\xi >0$.
- Sens indirect : $\Delta _{r}G >0$ et $d\xi <0$.
- Équilibre : $\Delta _{r}G =0$.
### Expressions de $\Delta _{r}G$
$\Delta_{r} G = \Delta_{r} G^{\circ} +RT \ln(Q_{r})$
### Loi d'action de masses
$\displaystyle Q_{r,eq} = K^{\circ} (T) = \exp\left( - \frac{\Delta_{r} G^{\circ} }{RT} \right)$
$\displaystyle \Delta_{r}G = RT \ln\left(\frac{Q_{r}}{K^{\circ}}\right)$ 
### Relation de Van't Hoff
Dans le cadre de l'approximation d'Ellingham, cette relation donne l'évolution de la constante d'équilibre avec la température.
$\displaystyle \frac{d \ln(K^{\circ} )}{dT} = \frac{\Delta_{r} H^{\circ} }{RT^{2}}$
### Combinaison de réaction et constantes d'équilibre 
D'après la loi de Hess :
$\displaystyle K^{\circ} = \prod (K_{i}^{\circ}) ^{\nu_{i}}$
### Grandeurs de réaction à partir de $\Delta_{r} G^{\circ} (T)$ ou $K^{\circ} (T)$ 
On cherche l'enthalpie ou l'entropie de réaction standard à partir des expressions présidents. 
#### $\Delta_{r} G^{\circ}$ en fonction de $T$  
$\Delta_{r} G^{\circ} = \Delta_{r} H^{\circ}  -T \Delta_{r} S^{\circ}$
- Ordonnée à l'origine : $\Delta_{r} H^{\circ}$ 
- Pente : $- \Delta_{r} S^{\circ}$
#### $\ln(K^{\circ} (T))$ en fonction de $1/T$
$\displaystyle \ln(K^{\circ} (T))= - \frac{\Delta_{r} H^{\circ} }{RT} + \frac{\Delta_{r} S^{\circ} }{R}$ 
- Ordonnée à l'origine : $\displaystyle \frac{\Delta_{r}S^{\circ} }{R}$.
- Pente : $\displaystyle - \frac{\Delta_{r} H^{\circ} }{R}$
### Dégrée d'avancement d'une réaction 
#### Réaction peu avancée
$K^{\circ} << 1$  et  $\xi_{f} << n_{limitant}$ 
#### Réaction équilibrée
$K^{\circ}  \approx 1$  et  $\displaystyle \xi_{f} \approx \frac{n_{lim}}{2}$
#### Réactions totales ou quantitatives 
$K^{\circ} >> 1$  et  $\xi_{f} \approx n_{max}$ 
#### Température  d'inversion
$K^{\circ} (T_{i}) = 1 \implies \Delta_{r} G^{\circ} =0$

## Influencer le sens de réaction 
On considère que le système est au départ à l'équilibre.
### Principe de modération 
Un système qui est dans un équilibre stable réagit à une perturbation en s'y opposant. L'élévation de température extérieur est contrée par un déplacement de la réaction dans le sens qui refroidit le système. 
### Température 
On commence avec une réaction à l'équilibre $\Delta_{r} G=0$.
On raisonne en considérant une élévation de température
#### Raisonnement 
Pour une réaction endothermique : $\Delta_{r} H^{\circ} >0$.
D'après la [[relation de  Van't Hoff]], $\ln(K^{\circ} )$ est croissante avec $T$.
Comme on a la relation [[ entre Q et K ]] alors $\Delta_{r} G$ diminue.
Or on a commence à l'équilibre, $\Delta_{r} G$ dévient négatif.
Alors la réaction se fait dans le sens direct. 
#### Conclusion 
Une augmentation de température provoque une déplacement de l'équilibre dans le sens endothermique. De même, une diminution de $T$ provoque un déplacement de l'équilibre dans le sens exothermique. 
### Pression 
Or $K^{\circ}$ ne dépend pas de $P$. Alors on aura influence que si on a de gaz  présents. Dans ce cas  $Q_{r}$ dépend de la pression. 
#### Raisonnement 
On commence avec un système à l'équilibre.
Si $\displaystyle \sum _{gaz} \nu_{i}>0$ alors on crée du gaz.
Alors on a $Q_{r}$ qui augmente avec $P$.
Alors d'après [[ entre Q et K ]] $\Delta_{r} G$ augmente.
Or on a commence à $\Delta_{r} G=0$ alors $\Delta_{r} G>0$.
Donc la réaction se fait dans le sens indirecte, c'est à dire le sens qui détruit du gaz. 
#### Conclusion 
Une augmentation de pression déplace un équilibre dans le sens d'une diminution des quantités de gaz. De même, une diminution de pression le déplace dans le sens qui augmente la quantité de gaz dans le milieu.
### Composition 
En ajoutant un produit ou un actif on modifié $Q_{r}$. Si on l'augmente la réaction se fait dans le sens indirecte, et si on l'augmente dans le sens direct. 