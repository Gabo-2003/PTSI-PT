#chapitre31 #electromagnetique #magnetique #electricite #electromecanique
![[Actions d'un champ magnétique#Motionnelle|Induction Motionnelle :]]
## Conversion de puissance mécanique en puissance électrique
### Méthode de résolution du système électromécanique
- Choix du repérage spatial et des conventions.
- Analyse qualitative.
- Etablissement de l'équation électrique : [[Signaux électiques dans l'ARQS#Loi des Mailles|loi de mailles]] et [[Actions d'un champ magnétique#Loi de Faraday|loi de Faraday]]  
- Etablissement de l'équation mécanique : [[Dynamique Newtonienne#2èm Loi Principe fondamental de la dynamique|PFD]] et [[Mouvement d'un solide#Théorème scalaire du moment cinétique|TMC]].
- Résolution du système d'équations.
### Rails de Laplace (générateurs)
#### Choix du repérage spatial et des conventions
![[image rails generateurs.png|300]]
#### Analyse qualitative
Une force $\vec{F}$ est appliquée sur la tige 
$\hookrightarrow$ cette force conduit à une déplacement
$\hookrightarrow$ Alors il y a une variation du [[Actions d'un champ magnétique#Flux magnétique|flux magnétique]] $\phi$ (car $S$ varie)
$\hookrightarrow$ Apparition d'une courant induit et des [[Actions d'un champ magnétique#Forces de Laplace|forces de Laplace]] $\vec{F_{L}}$ 
- D'après la [[Actions d'un champ magnétique#Loi de Lenz|loi de Lenz]], $\vec{F_{L}}$ s'oppose à $\vec{F}$ 
#### Etablissement de l'équation électrique
$-Blv = Ri$ 
#### Etablissement de l'équation mécanique
$m \frac{dv}{dt}=ilB+F$ 
#### Résolution du système d'équations
$\displaystyle v(t) = v_{\infty} (1-e^{- \frac{t}{\tau}})$ 
avec $\begin{cases} \tau = \frac{mR}{ (Bl)^{2}}  \\ v_{\infty} = \frac{FR}{(Bl)^{2}} \end{cases}$ 
#### Etude énergétique
$\displaystyle \mathcal{P}_{\text{méca}} = \frac{dE_{c}}{dt} + \mathcal{P}_{J}$ 
- Une fois le [[Circuits linéaires du 1èr ordre#Régime transitoires et permanents|régime permanent]] est établie, la conversion d'énergie est totale : $\mathcal{P}(\vec{F})=\mathcal{P}_{J}$ 
### Alternateur 
Système produisant un signal électrique alternatif à partir d'une excitation mécanique caractérisée par une vitesse constant. 
![[image alternateur.png|300]]
- Or la spire est en rotation, le [[Actions d'un champ magnétique#Flux magnétique|flux magnétique]] n'est pas constante : $\phi_{s}= BS \cos(\theta) = BS \cos(\omega t)$ 
#### Résolution du système électromécanique 
##### Equation électrique 
$\displaystyle i(t)=\frac{BS \omega}{R} \sin(\omega t)$ 
##### Equation mécanique 
$\Gamma_{ext,z}(t)=J_{z} \dot{\omega}-iSB \sin(\omega t)$ 
#### Etude énergétique 
$\mathcal{P}_{J}=\mathcal{P}_{ext}$ au [[Circuits linéaires du 1èr ordre#Régime transitoires et permanents|régime permanent]]. 
### Freinage par induction
#### Courants de Foucault 
Courants électriques crées dans une masse conductrice par induction 
#### Freinage 
Grace à la [[Actions d'un champ magnétique#Loi de Lenz|loi de Lenz]], il est possible d'utiliser l'induction dans un volume conducteur afin de générer plus de mouvement des charges par induction et donc obtenir une force de freinage plus important.
- Il n'y a pas de contact entre les pièces.
- Le couple de freinage est proportionnelle à la vitesse, donc pas d'arrête totale.

## Conversion de puissance électrique en puissance mécanique 
### Moteur à courante continue à entrefer plan 
![[image mcc entrefer plan.png]]
#### Modélisation 
- On dispose de brins conducteurs de résistance $R$ parcourus par une courante $I$ imposé par une source extérieur
![[image modele mcc.png|300]]
- Or chaque brin est perpendiculaire au champ $\vec{B}$, ils sont soumis à une [[Actions d'un champ magnétique#Forces de Laplace|forces de Laplace]]. 
- Du à la géométrie, $\vec{R_{L}}=\vec{0}$ 
![[image mcc forces.png|300]]
#### Couple moteur 
$\displaystyle \vec{\Gamma_{L}}=n \times \frac{IB\rho^{2}}{2} \vec{e_{z}}$ 
#### Force électromotrice induite dans un brin
$\displaystyle e(t)=- \frac{B \omega \rho^{2}}{2}$ 
#### Bilan de Puissance 
$\mathcal{P}_{gen} = \mathcal{P}_{J} +\mathcal{P}_{méca}$    