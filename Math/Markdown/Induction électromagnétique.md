## Lois de l'induction
La variation du [[Magnétostatique|champ magnétique]] au travers du circuit fait apparaître un [[Le champ électrostatique|champ électrique]] mettant en mouvement les charges du conducteur. 
### Induit
Portion de circuit dans laquelle un courante électrique est généré.
### Inducteur 
Système créant le [[champ]] magnétique à l'origine du phénomène d'induction
### Induction statique ou motionnelle 
#### Statique 
Induit supposé rigide et fixe. $\vec{B}$ varie avec le temps due à un mouvement de l'inducteur ou variation de la courante
#### Motionnelle 
Champ stationnaire. Variation de $\vec{B}$ due au mouvement ou déformation de l'induit 
### Lois de base de l'induction
#### Loi de Faraday
Relie le courant induit dans un circuit fermé à la variation de flux magnétique via la notion de force électromotrice (f.é.m.) induit. 
- $\displaystyle \boxed{e(t)=- \frac{d\Phi}{dt}} = \oint_{Circuit} \overrightarrow{E}(M) \cdot d \overrightarrow{OM}$   
- Avec $\Phi$ le flux sur la surface qui s'appui sur le circuit.
- C'est possible grâce à la [[Magnétostatique#Flux conservatif|conservation du flux]] du champ magnétique.
##### Forme locale [[Equation de Maxwell-Faraday]]
$\displaystyle\overrightarrow{\text{rot}}(\overrightarrow{E}) = - \frac{\partial \overrightarrow{B}}{\partial t}$ 
Cet loi donne les sources axiales du champ électrique, c'est-à-dire, les variations temporelles de champ magnétique.
#### Loi de Lenz
Les effets des phénomènes d'induction s'opposent aux causes qui leur ont donnée naissance.

## Induction statique 
### Auto-induction 
#### Inductance propre 
##### Flux propre $\phi_{p}$
Le circuit génère un flux magnétique à travers lui-même.
##### Flux appliqué $\phi_{a}$
Flux de un champ extérieur $\vec{B_{ext}}$  
##### Flux total $\phi$
$\phi= \phi_{p}+\phi_{a}$  
- C'est le flux qui intervienne dans la Loi de Faraday. 
- Alors le phénomène d'induction peut se produire sans recourir à un inducteur "extérieur".
##### Coefficient d'auto-induction $L$
$\boxed{\phi_{p}= L \times i(t)}$ 
- $L$ ne dépend que de la géométrie du circuit. Alors constante si la géométrie ne varie pas.  
- Unité usuelle : henry ($H$) avec $1H = 1Wb/A$. 
- $L>0$ toujours 
#### Cas du solénoïde long  
$L= \mu_{0} \frac{N^{2}}{l}S$ 
- avec $S$ la surface de d'une spire
#### Force électromotrice auto-induite
Déduit de la [[Actions d'un champ magnétique#Loi de Faraday|Loi de Faraday]] 
- Convention générateur : $\boxed{e_{p}(t)=-L \frac{di}{dt}}$
- Convention récepteur : $u(t)=L \frac{di}{dt}$ 
#### Etude énergétique 
$E_{m}(t)=\frac{1}{2}Li^{2}$
### Induction mutuelle
On a deux circuits $\mathcal{C}_{1}$ et $\mathcal{C}_{2}$ d'inductances propres $L_{1}$ et $L_{2}$ et parcourus par des courantes $i_{1}(t)$ et $i_{2}(t)$
#### Coefficient d'induction mutuelle $M$
$\begin{align*}   \Phi_{1\rightarrow2} = M \times i_{1}(t)  \\ \Phi_{2\rightarrow 1} = M \times i_{2}(t) \end{align*}$    $M$ exprimé en Henry
- Dépend de la géométrie des deux circuits et de la position et orientation relative entre eux.
- Positif si le flux appliqué s'ajoute au flux propre, négative sinon.
- $M^{2} \leq L_{1}L_{2}$ 
#### Influence totale entre deux bobines longues 
Deux circuits sont en influence totale lorsque chacun capte l'integralité du flux magnétique envoyé par l'autre.
- $M=L_{1}L_{2}$ 
- $|M|=\mu_{0} \frac{N_{1}N_{2}}{\sqrt{l_{1}l_{2}}}S$
- Dans le cas où il n'y a pas d'influence totale : $|M|=k \sqrt{L_{1}L_{2}} ; \quad  0 \leq k \leq 1$ 
#### Circuits couplés
##### Etablissement du système d'équations couplées
$\begin{cases} \displaystyle e_{1}(t)=-L_{1} \frac{di_{1}}{dt} -M\frac{di_{2}}{dt} \\ \displaystyle e_{2}(t)=-L_{2} \frac{di_{2}}{dt} -M\frac{di_{1}}{dt} \end{cases}$
##### Régime sinusoïdal forcé 
$\underline{E_{g}} = \underline{Z} \times \underline{I_{1}}$ 
$\displaystyle \underline{Z}=R_{1}+j \omega L_{1} + \frac{(\omega M)^{2}}{R_{2}+j \omega L_{2}}$ 
- Donc du POV du circuit n°1, la bobine se comporte comme un dipôle dont l'impédance complexe dépend des caractéristiques de deux circuits et leur positions relatives.
##### Etude énergétique 
$\displaystyle E_{m}(t)=\frac{1}{2}L_{1}i_{1}^{2}+\frac{1}{2}L_{2}i_{2}^{2} + M i^{1} i^{2}$ 
#### Transformateur électrique 
Système électrique utilisé pour modifier un signal électrique alternatif en un signal de même forme et même fréquence mais d'amplitudes de tensions et de courants différents.
##### Loi de tensions 
$\displaystyle m = \frac{v_{2}(t)}{v_{1}(t)}=\frac{N_{2}}{N_{1}}$ 

## Induction motionnelle
### Conversion de puissance mécanique en puissance électrique
#### Méthode de résolution du système électromécanique
- Choix du repérage spatial et des conventions.
- Analyse qualitative.
- Etablissement de l'équation électrique : [[Signaux électiques dans l'ARQS#Loi des Mailles|loi de mailles]] et Loi de Faraday  
- Etablissement de l'équation mécanique : [[Dynamique Newtonienne#2èm Loi Principe fondamental de la dynamique|PFD]] et [[Mouvement d'un solide#Théorème scalaire du moment cinétique|TMC]].
- Résolution du système d'équations.
#### Rails de Laplace (générateurs)
##### Choix du repérage spatial et des conventions
![[image rails generateurs.png|300]]
##### Analyse qualitative
Une force $\vec{F}$ est appliquée sur la tige 
$\hookrightarrow$ cette force conduit à une déplacement
$\hookrightarrow$ Alors il y a une variation du [[Actions d'un champ magnétique#Flux magnétique|flux magnétique]] $\phi$ (car $S$ varie)
$\hookrightarrow$ Apparition d'une courant induit et des [[Actions d'un champ magnétique#Forces de Laplace|forces de Laplace]] $\vec{F_{L}}$ 
- D'après la [[Actions d'un champ magnétique#Loi de Lenz|loi de Lenz]], $\vec{F_{L}}$ s'oppose à $\vec{F}$ 
##### Etablissement de l'équation électrique
$-Blv = Ri$ 
##### Etablissement de l'équation mécanique
$m \frac{dv}{dt}=ilB+F$ 
##### Résolution du système d'équations
$\displaystyle v(t) = v_{\infty} (1-e^{- \frac{t}{\tau}})$ 
avec $\begin{cases} \tau = \frac{mR}{ (Bl)^{2}}  \\ v_{\infty} = \frac{FR}{(Bl)^{2}} \end{cases}$ 
##### Etude énergétique
$\displaystyle \mathcal{P}_{\text{méca}} = \frac{dE_{c}}{dt} + \mathcal{P}_{J}$ 
- Une fois le [[Circuits linéaires du 1èr ordre#Régime transitoires et permanents|régime permanent]] est établie, la conversion d'énergie est totale : $\mathcal{P}(\vec{F})=\mathcal{P}_{J}$ 
#### Freinage par induction
##### Courants de Foucault 
Courants électriques crées dans une masse conductrice par induction 
##### Freinage 
Grace à la loi de Lenz, il est possible d'utiliser l'induction dans un volume conducteur afin de générer plus de mouvement des charges par induction et donc obtenir une force de freinage plus important.
- Il n'y a pas de contact entre les pièces.
- Le couple de freinage est proportionnelle à la vitesse, donc pas d'arrête totale.
### Conversion de puissance électrique en puissance mécanique 
#### Moteur à courante continue à entrefer plan 
![[image mcc entrefer plan.png]]
##### Modélisation 
- On dispose de brins conducteurs de résistance $R$ parcourus par une courante $I$ imposé par une source extérieur
![[image modele mcc.png|300]]
- Or chaque brin est perpendiculaire au champ $\vec{B}$, ils sont soumis à une [[Actions d'un champ magnétique#Forces de Laplace|forces de Laplace]]. 
- Du à la géométrie, $\vec{R_{L}}=\vec{0}$ 
![[image mcc forces.png|300]]
##### Couple moteur 
$\displaystyle \vec{\Gamma_{L}}=n \times \frac{IB\rho^{2}}{2} \vec{e_{z}}$ 
##### Force électromotrice induite dans un brin
$\displaystyle e(t)=- \frac{B \omega \rho^{2}}{2}$ 
##### Bilan de Puissance 
$\mathcal{P}_{gen} = \mathcal{P}_{J} +\mathcal{P}_{méca}$    