## Onde dans le conducteur
### Modèle de Drude
Modèle tenant en compte de l'action du réseau cristallin sur les électrons de conduction dans un métal.
On part du PFD : $m_{e} \frac{d \overrightarrow{v}}{dt} = - e \overrightarrow{E} - \frac{m_{e}}{\tau}\overrightarrow{v}$ 
Et la relation : $\underline{\overrightarrow{j}} = n_{e} (-e) \underline{\overrightarrow{v}}$
On trouve : $\displaystyle \underline{\gamma } = \frac{\gamma _{0}}{1+ j \omega \tau}$ avec $\displaystyle \gamma _{0} = \frac{n_{e}e^{2}\tau}{m_{e}}$
On a donc un comportement de filtre passe bas, il faut être en basse fréquence pour que $\underline{\gamma } \approx \gamma _{0}$ et donc avoir un comportement de conducteur ohmique.
Alors il faut que $\omega  << \omega _{0} = \frac{1}{\tau}$
Pour le cuivre il faut que $f < 10^{14} \;Hz$ 
### Équations constitutives 
On veut décrire la propagation d'une onde électromagnétique dans un milieu ohmique et dans l'ARQS magnétique. Pas de charges et pas de variation de $\overrightarrow{E}$. 
- Loi d'Ohm locale (conducteur ohmique) : $\overrightarrow{j} = \gamma _{0} \overrightarrow{E}$ on est en basse fréquence.
- Maxwell-Gauss : $div(\overrightarrow{E}) =0$ et $\rho = 0$
- Flux magnétique : $div(\overrightarrow{B}) =0$ 
- Maxwell-Faraday : $rot(\overrightarrow{E}) = - \frac{\partial \overrightarrow{B}}{\partial t}$ 
- Maxwell-Ampère : $rot(\overrightarrow{B}) = \mu_{0} \overrightarrow{j}$
### Équation de propagation 
Comme avant on utilise la relation  $\overrightarrow{rot} (\overrightarrow{rot} (\overrightarrow{X})) = \overrightarrow{grad}(div(\overrightarrow{x})) - \Delta \overrightarrow{X}$ et on trouve :
$\displaystyle\Delta \overrightarrow{E} = \mu_{0}\gamma_{0} \frac{\partial \overrightarrow{E}}{\partial t}$ 
A différence d'avant, on a ici une équation irréversible, lié à la dissipation de l'énergie par effet Joule.    
### Recherche d'une solution 
$\displaystyle \overrightarrow{E} = E_{1}\exp\left( - \frac{x}{\delta } \right) \exp\left( j \left( \omega t - \frac{x}{\delta }\right)   \right) \overrightarrow{e} + E_{2}\exp\left( \frac{x}{\delta } \right) \exp\left( j \left( \omega t + \frac{x}{\delta }\right)   \right) \overrightarrow{e}$
- $\exp \left( - \frac{x}{\delta } \right)$ : Facteur d'attenuation, penetration de l'onde sur quelque $\delta$ seulement.
- $\omega t - \frac{x}{\delta }$ : aspect propagative, phase de l'onde.
	$\omega t - \frac{x}{\delta } \implies V_{\varphi } = \delta \omega$ propagation dans le sens croissante.
Distance caractéristique : $\displaystyle \delta = \sqrt{\frac{2}{\mu_{0}\gamma _{0}\omega }}$
- Appelée aussi profondeur de peau. Plus l'onde est basse fréquence, plus elle rentre profondément dans le métal.
- Pour un conducteur parfait a $\gamma_{0} = + \infty \implies \delta = 0$
### Expression des champs
On considère un milieu metalique limité à $x>0$. Il resout une OPPH polarisé en  $y$. On a donc :
$\displaystyle \overrightarrow{E} = E_{0}\exp\left( -\frac{x}{\delta } \right) \cos\left( \omega t - \frac{x}{\delta} \right) \overrightarrow{e_{y}}$ 
On trouve le [[champ]] magnétique en utilisant Maxwell-Faraday :
$\displaystyle  \overrightarrow{B} = \frac{\sqrt{2}E_{0}}{\delta \omega } \exp\left( -\frac{x}{\delta } \right) \cos\left( \omega t - \frac{x}{\delta} - \frac{\pi}{4} \right) \overrightarrow{e_{z}}$
- Les deux champs sont déphases de $\frac{\pi}{4}$.
- Ils ne pénètrent que sur une oscillation environ.
### Aspect énergétique
Vecteur de Poynting :
$\displaystyle  \overrightarrow{\Pi}= E_{0}^{2} \sqrt{\frac{\gamma_{0}}{\mu_{0}\omega }}e^{- 2 \frac{x}{\delta }} \frac{1}{2}\left( \cos \left(\omega t - \frac{x}{\delta }- \frac{\pi}{4}\right)+\cos\left(\frac{\pi}{4}\right)\right)\overrightarrow{e_{x}}$ 
$\displaystyle  <\overrightarrow{\Pi}> = E_{0}^{2}\sqrt{\frac{\gamma_{0}}{\mu_{0}\omega }}e^{- \frac{x}{\delta }} \frac{\sqrt{2}}{4} \overrightarrow{e_{x}}$ 
Calcul de $e_{EB}$ :
$\displaystyle  e_{EB} = \frac{1}{2} E_{0} e^{-2 \frac{x}{\delta }} \left( \epsilon_{0}\cos^{2}\left( \omega t - \frac{x}{\delta }\right) + \frac{\gamma_{0}}{\omega } \cos^{2}\left( \omega t - \frac{x}{\delta }- \frac{\pi}{4} \right)  \right)$
$<e_{EB}> = \frac{1}{4} E_{0} e^{-2 \frac{x}{\delta }} \left(\epsilon_{0}+ \frac{\gamma_{0}}{\omega }  \right)$
- Pour les deux moyennes on observe une rapide décroissance lors de la pénétration dans le conducteur. C'est à cause de $e^{- 2\frac{x}{\delta }}$ avec une distance caractéristique $\frac{\delta }{2}$ 
Calcul de $P_{v}$ :
$\displaystyle P_{v} = \overrightarrow{E} \cdot  \overrightarrow{j} = \overrightarrow{E}^{2}\gamma_{0} = \gamma_{0}E_{0}^{2}e^{-2 \frac{x}{\delta }}\cos^{2}\left( \omega t - \frac{x}{\delta } \right)$ 
$\displaystyle <P_{v}> = \frac{\gamma_{0}E_{0}^{2}}{2}e^{-2 \frac{x}{\delta }}$

## Réflexion sur un conducteur parfait
### Le conducteur parfait
Il est définie par $\gamma = + \infty$. Dans lui on a :
- $\overrightarrow{E} = 0$
- $\overrightarrow{B} = 0$
- $\overrightarrow{j} = 0$ 
- $\rho = 0$
#### Conditions au limites 
Si le conducteur est dans $x>0$ :
- $\displaystyle \overrightarrow{B}(M^{+},t) - \overrightarrow{B}(M^{-},t) = \mu_{0}\overrightarrow{j_{S}}(M,t) \wedge \overrightarrow{u_{trav}}(M)$
- $\displaystyle \overrightarrow{E}(M^{+},t) - \overrightarrow{E}(M^{-},t) = \frac{\sigma (M,t)}{\epsilon_{0}} \cdot  \overrightarrow{u_{trav}}(M)$
Il y a continuité du champ électrique $\overrightarrow{E_{T}}$ et du champ magnétique $\overrightarrow{B_{N}}$ à travers d'une interface quelconque.
### OPPH incident 
On pose la plaque métallique en $x=0$ et le milieu de propagation en  $x<0$.
On considère une OPPH polarisé selon $Oy$ qui se déplace selon $x$ croissant :
$\displaystyle \overrightarrow{E}_{i} = E_{0}\cos(\omega t-kx)\overrightarrow{e_{y}}$ 
$\displaystyle \overrightarrow{B}_{i} = \frac{E_{0}}{c}\cos(\omega t-kx)\overrightarrow{e_{z}}$ 
On prend $\overrightarrow{u_{trav}}= - \overrightarrow{e_{x}}$ en prenant la variation du champ de l'intérieur vers l'extérieur.
### Onde réfléchi
L'absence d'onde transmise et d'effet Joule rend nécessaire l'existence d'une onde réfléchie. 
- Par linéarité des équations mise en jeu, l'onde réfléchi est de même frequence et de vecteur d'onde de même norme.
$\overrightarrow{E_{r}} = - E_{0}\cos(\omega t+kx) \overrightarrow{e_{y}}$ 
$\overrightarrow{B_{r}} = \frac{E_{0}}{c} \cos(\omega t+kx)\overrightarrow{e_{z}}$ 
### Onde totale
$\displaystyle \overrightarrow{E} = \overrightarrow{E_{r}}+ \overrightarrow{E_{i}} = 2E_{0} \sin(\omega t)\sin(kx) \overrightarrow{e_{y}}$ 
$\displaystyle \overrightarrow{B} = \overrightarrow{B_{r}}+ \overrightarrow{B_{i}} = \frac{2E_{0}}{C} \cos(\omega t) \cos(kx)\overrightarrow{e_{z}}$
Ce sont des ondes stationnaires 
Noeuds : points de vibration nulles. 
Ventres : points de vibration maximales.
### État de la surface 
Avec les conditions aux limites on trouve que l'onde incident ne crée pas d'accumulation de charges mais un déplacement suivant $\overrightarrow{E}$.
Les courants surfaciques produits sont la source du champ réfléchi.
### Pression de radiation

## Onde électromagnétique dans une cavité unidimensionnelle 
### Position du problème 
On étudie la possibilité d'existence d'une onde électromagnétique entre deux parois métalliques idéales. 
On cherche les solutions de la forme :
Onde stationnaire $\overrightarrow{E} = f(x)g(t)\overrightarrow{e_{y}}$ suivant $g(t) = e^{i \omega t}$. 
- C'est une onde plane et transverse
### Solutions 
#### Solution pour le champ électrique 
On injecte la solution proposé dans l'équation de d'Alembert :
$\displaystyle\nabla \overrightarrow{E} = \frac{1}{c^{2}} \frac{\partial^{2} \overrightarrow{E} }{\partial t^{2}}$ 
On trouve avec $A$ une constante :
$\begin{cases} f''(x) -A f(x) = 0 \\ g''(t) - A g(t) =0 \end{cases}$
##### Si $A>0$ :
$f(x) = \alpha \,ch(\sqrt{A}x) + \beta \,sh(\sqrt{A}x)$
On trouve avec les conditions limites : $f(x) = 0$. Donc ce n'est pas une solution.
##### Si $A<0$
On pose  $-A = k^{2}$
- Pour $f$ :
$f(x) = \alpha \cos(k x) + \beta \sin(k x)$ 
On trouve avec les conditions limites $\displaystyle  k_{n} = \frac{n \pi}{a}$
$f(x) = \sin\left( \frac{n \pi}{a} x \right)$
- Pour $g$ : $g''(t) +k^{2}c^{2}g(t) = 0$
On pose $\omega ^{2} = k^{2} c^{2}$ 
$g(t) = E_{0}\cos(\omega t - \varphi )$ 
Finalement on a :
$\overrightarrow{E} = E_{0}  \sin\left( \frac{n \pi}{a} x \right)\cos(\omega t - \varphi )$
#### Relations 
$\displaystyle k_{n} = \frac{2 \pi}{\lambda _{n}} = \frac{n \pi}{a} \implies \lambda _{n} = \frac{2a}{n}$ 
$\displaystyle k_{n} = \frac{\omega_{n}}{c} = \frac{n \pi}{a} \implies \omega _{n} = \frac{c n \pi}{a}$ 
#### Solution pour le champ magnétique 
On utilise l'équation de Maxwell-Faraday et on trouve :
$\displaystyle \overrightarrow{B} = - \frac{E_{0}}{c} \cos\left( \frac{n \pi}{a} x  \right) \sin(\omega t + \varphi ) \overrightarrow{e_{z}}$
### Analyse des solutions 
Seule les ondes stationnaires peuvent se développer dans ces cavités. La superposition de telles ondes, qui peut ne pas être une onde stationnaire, est aussi solution. 