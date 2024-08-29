[[Champ]]
## Les sources du magnétisme
Le [[champ]] magnétique est engendré soit par des courants soit par des aimants permanents. 
### Les distributions 
Linéique : en $A$
Surfacique : en  $A\cdot m^{-1}$
Volumique : en $A \cdot	m^{-2}$
### Intensité 
Courant qui circule dans un conducteur : 
$\displaystyle I = \iint_{Sec} \overrightarrow{j} \cdot \overrightarrow{dS}$
- $\overrightarrow{j} = \rho_{m} \overrightarrow{v}$ avec $\rho_{m}$ la densité de charge mobile.
- $\delta I = \overrightarrow{j} \cdot \overrightarrow{dS}$
- Pour une densité uniforme de courant : $I = j S_{droite}$
- On a additivité des contributions au courant.
- Analogue au [[Fluide en écoulement stationnaire dans une conduite#Débit massique|debit massique]].

## Propriétés de symétrie et d'invariance des distributions de courant
### Symétrie de la distribution
Un plan de symétrie pour les courant est donc un plan d'antisymétrique pour le champ magnétique. 
- Si $M \in \pi_{s}$, $\overrightarrow{B}(M)$ orthogonal au plan
- $sym_{\pi_{s}}(\overrightarrow{B}(M)) = - \overrightarrow{B}(sym_{\pi_{s}}(M))$
### Antisymétrique de la distribution
Un plan d'antisymétrique pour les courants devient donc un plan de symétrie pour le champ magnétique. 
- Si $M \in \pi_{a}$, $\overrightarrow{B}(M)$ appartient au plan
- $sym_{\pi_{a}}(\overrightarrow{B}(M)) = \overrightarrow{B}(sym_{\pi_{a}}(M))$
### Invariances 
[[Le champ électrostatique#Les invariances|Même conséquences]] que pour le champ électrique.

## Propriétés générales 
### Flux conservatif
Dû à l'inexistence de charges magnétiques, le champ magnétique est à flux conservative : 
- $\displaystyle \oint \oint_{s} \overrightarrow{B} \cdot \overrightarrow{dS} = 0$
- $\displaystyle \iint_{s} \overrightarrow{B}\cdot \overrightarrow{dS} = \phi _{c}$
- Le flux magnétique est mesuré en weber $Wb$
### Théorème de Ampère 
Sur toute courbe fermée $(\mathcal{C})$, la circulation du champ magnétique est égale à $\mu _{0}$ multiplié par le courant enlacé par $(\mathcal{C})$.
- $\displaystyle \oint_{C} \overrightarrow{B}(M)\cdot d\overrightarrow{OM} = \mu _{0} I_{enlacé}$ 
- Attention à la orientation de $(\mathcal{C})$ qui induit celle du courant passant au travers de la courbe fermée. 
- $\mu _{0} = 4 \pi \cdot 10^{-7} \;H \cdot m^{-1}$

## Moment magnétique 
### Moment magnétique pour une boucle de courant
$\displaystyle \overrightarrow{m} = i \overrightarrow{S}$ en $A \cdot m^{2}$
- Le théorème de superposition s'applique
### Moment d'une solénoïde :
Somme du moment de chaque spire.
### Moment magnétique d'une aimant :
$\displaystyle \vec{M} = \frac{\vec{\mu}}{V}$ 
- L'aimantation est au moment magnétique ce que la masse volumique est à la masse 


## Cartes de champ
### Cartographie du champ $\vec{B}$
#### Champ créé par un fil rectiligne 

| ![[image fil rectiligne.png]] | ![[image main droite fil rectiligne.png]] |
| ------------------------------------ | ------------------------------------ |
- Plus on s'éloigne du fil, moins le champ génère est intense.
Pour $r<R$ :
- $\displaystyle\overrightarrow{B}(M) = \frac{\mu_{0}Ir}{2 \pi R^{2}} \overrightarrow{e_{\theta}}$ 
Pour $r > R$
- $\displaystyle \overrightarrow{B}(M) = \frac{\mu_{0}I}{2 \pi r} \overrightarrow{e_{\theta}}$ 
#### Champ créé par une spire

| ![[image champ spire.png\|300]] | ![[image main droite spire.png\|300]] |
| ------------------------------- | ------------------------------------- |
#### Champ créé par un solénoïde
![[image champ solenoide.png|300]]
Au centre d'un solénoïde la champ est intense et quasi-uniforme.
A l'interieur :
- $\displaystyle\overrightarrow{B}(M) = \frac{\mu_{0}NI}{l} \overrightarrow{e_{z}}$  
A l'exterieur :
- $\overrightarrow{B}(M)=0$
#### Champ créé par un aimant permanent
![[image champ aimant permanent.png|300]]
### Propriétés des lignes de champ
- Le flux au travers de sections d'un tube de courant est toujours conservé. 
- Les lignes de champ magnétique se referment sur elle-même.
- Les lignes de champ sont orientées et tournent autour des courants. 
- Aucun potentiel scalaire n'est associé au champ magnétique. 

## Forme locale des lois de la magnétostatique 

### Équation de Maxwell du flux magnétique 
$div(\overrightarrow{B})=0$
- Équivalente au [[Le champ électrostatique#Théorème de Gausse|Théorème de Gauss]]
### Forme locale du théorème d'Ampère
$\overrightarrow{rot}(\overrightarrow{B}(M)) = \mu_{0} \overrightarrow{j}$
 