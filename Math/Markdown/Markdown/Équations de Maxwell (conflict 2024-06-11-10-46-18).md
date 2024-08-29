## Conservation de la charge
### Macroscopique 
$\displaystyle \frac{d Q}{dt} + \oint \oint_{(S)} \overrightarrow{j} \cdot  d \overrightarrow{S}_{sortant} = 0$ 
### Microscopique 
$\displaystyle \frac{\partial \rho}{\partial t} + div(\overrightarrow{j}) = 0$
### Bilan à une dimension 
On utilise des différents expressions de $I_{entrant}$ :
- $\displaystyle  I_{entrant} = \frac{dQ}{dt} = \frac{d}{dt}\left( \rho d\tau \right)$ 
- $\displaystyle  I_{entrant} = \iint \overrightarrow{j} \cdot  \overrightarrow{ds}_{entrant}$

## Les équations de Maxwell
### Formes locales 
#### Équation de Maxwell-Gauss
$\displaystyle div(\overrightarrow{E}) = \frac{\rho}{\epsilon_{0}}$ 
#### Équation de Maxwell-Faraday 
$\displaystyle \overrightarrow{rot}(\overrightarrow{E}) = - \frac{\partial \overrightarrow{B}}{\partial t}$ 
#### Équation de Maxwell du flux magnétique 
$\displaystyle div(\overrightarrow{B}) = 0$
#### Équation de Maxwell-Ampère
$\displaystyle \overrightarrow{rot}(\overrightarrow{B}) = \mu_{0} \left( \overrightarrow{j} + \epsilon_{0} \frac{\partial \overrightarrow{E}}{\partial t}  \right)$ 
### Formes macroscopiques 
#### Theorème de Gauss
On passe de l'équation de Maxwell-Gauss au théorème de Gauss avec le théorème d'Ostrogradski.
$\displaystyle \oint \oint_{S} \overrightarrow{E} \cdot  \overrightarrow{dS} = \frac{Q_{int}}{\epsilon_{0}}$ 
- Implique que le [[champ]] électrique à des sources polaires : les charges électriques. 
#### Loi de Faraday
On utilise le théorème de Stokes
- Implique que le champ électrique possède une source axiale qui est la variation temporelle du champ magnétique. 
$\displaystyle e = - \frac{d \phi_{B}}{dt}$ 
#### Champ magnétique à flux conservatif 
On le trouve avec le théorème d'Ostrogradski.
- Implique que le champ magnétique n'a pas des sources polaires.
$\displaystyle \oint \oint_{S}\overrightarrow{B} \cdot \overrightarrow{dS} = 0$ 
#### Forme généralisé du théorème d'Ampère 
On le trouve avec le théorème de Stokes
$\displaystyle \oint_{C} \overrightarrow{B}(M) \cdot  \overrightarrow{dOM} = \mu_{0} \left( \iint_{Sc} \overrightarrow{j} \cdot  \overrightarrow{dS} + \epsilon_{0} \frac{d}{dt} \left( \iint_{Sc} \overrightarrow{E} \cdot  \overrightarrow{dS} \right)  \right)$ 
- Il faut utiliser la même surface $Sc$ dans les deux integrales.
- Implique que le champ magnétique possède deux sources axiales : les courant et les variations temporelles du champ électrique.
#### Équation de conservation de la charge à partir des équations de Maxwell
Équation de Maxwell-Ampère $\longrightarrow$ on prend sa divergence $\longrightarrow$ on utilise le théorème de Schwartz $\longrightarrow$ équation de Maxwell-Gauss :
$\displaystyle div(\overrightarrow{j}) + \frac{\partial \rho}{\partial t} = 0$ 
### Retrouver les équations de la statique
#### Électrostatique
Les charges sont immobiles donc il n'y a pas champ magnétique, alors on a :
$\displaystyle  div(\overrightarrow{E}) = \frac{\rho}{\epsilon_{0}} \quad \quad \quad\overrightarrow{rot}(\overrightarrow{E}) = \overrightarrow{0}$
#### Magnétostatique 
Pas de variation de charge locale donc du champ électrique :
$div(\overrightarrow{B}) = 0 \quad \quad \quad \overrightarrow{rot}(\overrightarrow{B}) = \mu_{0} \overrightarrow{j}$
### ARQS Magnétique 
Le champ $\overrightarrow{B}$ domine.
- On néglige les variations du champ électrique dans l'équation de Maxwell-Ampère :
$\overrightarrow{rot}(\overrightarrow{B}) = \mu_{0}\overrightarrow{j}$ 
- On considère que le champ électrique à comme source les variations de $\overrightarrow{B}$. Alors $\overrightarrow{E}$ est inclus dans les plans de symétrie de $\overrightarrow{j}$ et orthogonal à ses plans d'antisymétrie. On utilise la forme intégrale de la Loi de Faraday. 
#### Conséquences
Il ne se produit aucune accumulation de charge: la loi des noeuds s'applique.
Pour être en ARQS magnétique il faut que : taille du système $<< \lambda$ 
### ARQS Électrique 
Il existe aussi.

## Énergie électromagnétique 
### Densité volumique de force électromotrice 
Force de Lorentz qui s'applique sur les particules chargées présentes.
- $\overrightarrow{f}_{L,v} = \rho(\overrightarrow{E} + \overrightarrow{v}\wedge\overrightarrow{B})$ 
### Puissance cédée à la matière 
$P_{v} = \rho(\overrightarrow{E} + \overrightarrow{v} \wedge\overrightarrow{B})\cdot \overrightarrow{v}$. Or la puissance du champ magnétique est nulle :
$P_{v} = \overrightarrow{j}\cdot \overrightarrow{E}$ 
- C'est une puissance dissipé, donnée à la matière.
### Loi d'Ohm locale
$\overrightarrow{E} = \frac{1}{\gamma } \overrightarrow{j}$ 
- $\gamma$ : conductivité du milieu en $\Omega^{-1} \cdot m^{-1}$
- On a donc la puissance dissipé : $P_{v} = \overrightarrow{j}\cdot \overrightarrow{E} = \gamma  \overrightarrow{E}^{2}$
- Pour un cylindre on a la resistance : $\displaystyle R = \frac{l}{\gamma  S}$
### Bilan générale : équation de Poynting
Fournis par l'énonce
$\displaystyle \frac{\partial }{\partial t} \underbrace{\left( \frac{1}{2} \epsilon_{0} E^{2} + \frac{1}{2} \frac{B^{2}}{\mu_{0}} \right)}_{\text{énergie volumique}} = \underbrace{- div\left( \frac{\overrightarrow{E} \wedge \overrightarrow{B}}{\mu_{0}} \right)}_{\text{Flux volumique entrant}} - \underbrace{\overrightarrow{j}\cdot \overrightarrow{E}}_{\text{Perte}}$ 
#### Énergie volumique du champ électromagnétique
$\displaystyle  E_{elecmag} = \frac{1}{2} \epsilon_{0} E^{2} + \frac{1}{2} \frac{B^{2}}{\mu_{0}}$
#### Vecteur Poynting
$\displaystyle \overrightarrow{\Pi} = \frac{\overrightarrow{E} \wedge \overrightarrow{B}}{\mu_{0}}$ 
- Puissance surfacique transportée par le champ électromagnétique. 
### Puissance électromagnétique 
Le flux du vecteur Poynting donne la puissance transportée par ce champ au travers d'une surface.
$\displaystyle  P = \iint \frac{\overrightarrow{E} \wedge \overrightarrow{B}}{\mu_{0}} \cdot  \overrightarrow{dS}$
### Forme macroscopique de l'équation de Poynting
$\displaystyle \frac{d E_{elecmag}}{dt} = \iiint_{V(S)} \frac{\partial }{\partial t} \left( \frac{1}{2} \epsilon_{0} E^{2} + \frac{1}{2} \frac{B^{2}}{\mu_{0}} \right) d\tau = \iiint_{V(S)} - div\left( \frac{\overrightarrow{E} \wedge \overrightarrow{B}}{\mu_{0}} \right) - \overrightarrow{j} \cdot  \overrightarrow{E} d\tau$
$\displaystyle \implies \frac{d E_{elecmag}}{dt} = \oint \oint_{S}  \frac{\overrightarrow{E} \wedge \overrightarrow{B}}{\mu_{0}} \overrightarrow{dS}_{entrant} - \iiint \overrightarrow{j} \cdot  \overrightarrow{E} d \tau$ 
