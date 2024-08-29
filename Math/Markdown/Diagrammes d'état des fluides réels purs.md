## Notion de phase
Une phase est une milieu dont les propriétés évoluent continument.
## Changement d'état isotherme d'un corps pur
### Condition d'équilibre 
Pour un corps pur diphasé à l'équilibre à $T$ et $P$ fixés :
$dG = dn_{1} \mu _{1} + dn_{2} \mu _{2}$ or à l'équilibre on a $dG=0$ :
$\mu _{1}(T,P) = \mu _{2} (T,P)$
### Condition d'évolution d'un corps pur diphasé
 C'est l'état physique de moindre potentiel qui est stable.
 Un déséquilibre se traduit par la disparition de la phase de potentiel chimique le plus élevé.
### Nombre de degré de liberté d'un changement d'état 
 On a 2 variables $(T,P)$ et une relation (la précèdent) donc on a 1 dégrée de liberté.
 Alors si on fixe une température, la pression est constante et inversement. 
### Diagramme $(P,T)$
 ![[image diagramme pt.png|400]]
 Point critique : Si $P > P_{c}$, alors on n'as pas de changement d'état.
 Point triple : point unique. 
#### Noms des transformation 
![[image nom transformations.png|400]]

## Enthalpie et entropie de changement d'état 
### Relations générales
On traite les changement d'état isotherme.
On écrit les changement d'état de l'état plus condensé vers le moins condensé.
- Les changement d'état vers un état moins condensé nécessitent un apport d'énergie. 
#### Caractéristique d'un changement d'état isotherme :
L'équilibre donne :
$dG = 0 \implies dH = T dS$
### Enthalpie de changement d'état 
$\Delta h_{vap} \approx 2 \; MJ \cdot  Kg^{-1}$ de l'eau
### Entropie de changement d'état :
D'après la caractéristique d'un changement d'état on en déduit :
$\displaystyle  \Delta s_{c.e} = \frac{\Delta h_{c.e}}{T_{c.e}}$
### Règle des moments 
![[image regle des moments.png|400]]
Il s'applique sous la courbe de changement d'état à toute variable extensive ($s$ et $h$ en particulière) pour une mélange diphasé. 
$m = m_{l}+m_{v}$
Titre en vapeur : $\displaystyle  x_{V} = \frac{m_{v}}{m} =\frac{LM}{LV}$ 
Titre en liquide : $\displaystyle x_{L} = \frac{m_{L}}{m}= \frac{MV}{LV}$
### Énergie récupérable lors de la condensation totale d'un fluide à pression constante
Les liquides permettent de récupérer de l'énergie lorsqu'ils se condensent.
1er principe : $\Delta H = Q = \Delta m \Delta h_{vap}$ 
Donc on à l'énergie récupérée :
$Q_{\text{récupéré}} = \Delta m \Delta h_{vap}$ 

## Les différents diagrammes d'état 
### Elements commun 
Courbe d'ébullition : Premières boules en contact du liquide saturant.
Courbe de rosée : Premières goutes en contact de la vapeur saturant. 
#### Interpolation linéaire
On peut utiliser une espèce de loi des moments pour trouver une valeur entre deux isobares par exemple.
#### Courbes isotitres 
Parfois représentes sous la courbe de changement d'état.
On les trouve avec le théorème des moments. 
### Diagramme de Clapeyron $(P,V)$ 
On peut récupérer le travail donnée à l'extérieur avec l'aire sous la courbe :
$\displaystyle \oint p \; dV = \oint - \delta w = w_{\text{récupérée}}$ 
- Sens horaire : moteur.
- Sens trigo : récepteur.
![[Prepa/PT/Physique/Attachments physique/image clapeyron.png]]
#### Comportement de gaz parfait 
Isothermes : $P = \frac{nRT}{V}$ donc des hyperboles, en $\ln$ des droites.
Isenthalpiques : 2èm loi de joule $dH = C_{p}dT$ donc confondues avec les isothermes : des paraboles.
Isentropiques : Loi de Laplace $P = \frac{cte}{V^{\gamma }}$ idem.
#### Comportement liquide idéal 
Isothermes : Indilatable donc isothermes confondues avec les isochores (verticales). 
Isenthalpiques : $H$ ne dépend que de la température pour un liquide idéal donc des verticales.
Isentropiques : idem
### Diagramme entropique $(T,s)$ 
![[image diagramme entropique.png]]
#### Comportement de gaz parfait 
Isobares : On utilise l'entropie d'un gaz parfait $\displaystyle s(T,P) = S(T_{0}, P_{0}) + \frac{\gamma }{\gamma -1} \frac{R}{M} \ln \left( \frac{T}{T_{0}} \right) - \frac{R}{M} \ln \left( \frac{P}{P_{0}} \right)$. En semi-log on voit des droites.
Isenthalpiques : 2em loi de joules, $dH = C_{p} dT$ donc confondues avec les isothermes (horizontales).
#### Comportement liquide idéal 
Isobares : Indilatable et incompressible donc l'état ne depend que de la temperature, les isobares sont confondues avec la courbe d'ébullition.
Isenthalpiques : $H(T)$ pour un liquide idéal, donc horizontales.  
### Diagramme de Mollier $(h,s)$ 
Le point critique n'est pas dans la position habituelle. 
![[image diagramme mollier.png]]
#### Comportement de gaz parfait 
Isothermes : 2nd loi de joules $dH = C_{p}dT$ donc ils sont confondues avec les isenthalpiques (horizontales).
Isobares : On utilise l'entropie et l'enthalpie du gaz parfait en fonction de $P$ et $T$. C'est des exponentielles. 
#### Comportement liquide idéal 
Isothermes : A une température donnée $s$ et $h$ sont définies d emanière unique, alors les isothermes rejoint la courbe de d'ébullition 
Isobares : $s$ et $h$ ne dépend de $P$, elles décrivent la courbe d'ébullition. 
### Diagramme des frigoristes $(\ln(P), h)$
![[image diagramme des frigoristes.png]]
#### Comportement de gaz parfait 
Isothermes : 2em loi de Joule $dH = C_{p}dT$ confondue avec les isenthalpiques (verticales). 
Isentropiques : on se sert à nouveau de l'entropie du gaz parfait. Difficilement reconnaissable. 
#### Comportement liquide idéal 
Isothermes : $h$ ne depend que de $T$ donc elles sont confondues avec les isenthalpiques (verticales).
Isentropiques : $S = C \ln(T) + cte$ c'est alors vertical.