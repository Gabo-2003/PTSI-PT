#chapitre30 #electromagnetique #magnetique #electricite 

## Auto-induction 
### Inductance propre 
#### Flux propre et flux appliqué
##### Flux propre $\phi_{p}$
Le circuit génère un [[Actions d'un champ magnétique#Flux magnétique|flux magnétique]] à travers lui-même.
##### Flux appliqué $\phi_{a}$
Flux de un champ extérieur $\vec{B_{ext}}$  
##### Flux total $\phi$
$\phi= \phi_{p}+\phi_{a}$  
- Le flux qui intervienne dans la [[Actions d'un champ magnétique#Loi de Faraday|Loi de Faraday]] c'est le flux total 
- Alors le phénomène d'induction peut se produire sans recourir à un inducteur "extérieur".
#### Coefficient d'auto-induction $L$
$\phi_{p}= L \times i(t)$ 
- $L$ ne dépend que de la géométrie du circuit. Alors constante si la géométrie ne varie pas.  
- Unité usuelle : henry ($H$) avec $1H = 1Wb/A$. 
- $L>0$ toujours 
### Cas du solénoïde long  
$L= \mu_{0} \frac{N^{2}}{l}S$ 
- avec $\mu_{0}$ la perméabilité magnétique du vide.
- avec $S$ la surface de d'une spire
### Force électromotrice auto-induite
Déduit de la [[Actions d'un champ magnétique#Loi de Faraday|Loi de Faraday]] 
- Convention générateur : $\boxed{e_{p}(t)=-L \frac{di}{dt}}$
- Convention récepteur : $u(t)=L \frac{di}{dt}$ 
### Etude énergétique 
$E_{m}(t)=\frac{1}{2}Li^{2}$
 
## Induction mutuelle
On a deux circuits $\mathcal{C}_{1}$ et $\mathcal{C}_{2}$ d'inductances propres $L_{1}$ et $L_{2}$ et parcourus par des courantes $i_{1}(t)$ et $i_{2}(t)$
### Coefficient d'induction mutuelle $M$
$\begin{align*}   \Phi_{1\rightarrow2} = M \times i_{1}(t)  \\ \Phi_{2\rightarrow 1} = M \times i_{2}(t) \end{align*}$    $M$ exprimé en Henry
- Dépend de la géométrie des deux circuits et de la position et orientation relative entre eux.
- Positif si le flux appliqué s'ajoute au flux propre, négative sinon.
### Influence totale entre deux bobines longues 
Deux circuits sont en influence totale lorsque chacun capte l'integralité du flux magnétique envoyé par l'autre.
- $M=L_{1}L_{2}$ 
- $|M|=\mu_{0} \frac{N_{1}N_{2}}{\sqrt{l_{1}l_{2}}}S$
- Dans le cas où il n'y a pas d'influence totale : $|M|=k \sqrt{L_{1}L_{2}} ; \quad  0 \leq k \leq 1$ 
### Circuits couplés
#### Etablissement du système d'équations couplées
$\begin{cases} \displaystyle e_{1}(t)=-L_{1} \frac{di_{1}}{dt} -M\frac{di_{2}}{dt} \\ \displaystyle e_{2}(t)=-L_{2} \frac{di_{2}}{dt} -M\frac{di_{1}}{dt} \end{cases}$
#### Régime sinusoïdal forcé 
$\underline{E_{g}} = \underline{Z} \times \underline{I_{1}}$ 
$\displaystyle \underline{Z}=R_{1}+j \omega L_{1} + \frac{(\omega M)^{2}}{R_{2}+j \omega L_{2}}$ 
- Donc du POV du circuit n°1, la bobine se comporte comme un dipôle dont l'impédance complexe dépend des caractéristiques de deux circuits et leur positions relatives.
#### Etude énergétique 
$\displaystyle E_{m}(t)=\frac{1}{2}L_{1}i_{1}^{2}+\frac{1}{2}L_{2}i_{2}^{2} + M i^{1} i^{2}$ 
### Transformateur électrique 
Système électrique utilisé pour modifier un signal électrique alternatif en un signal de même forme et même fréquence mais d'amplitudes de tensions et de courants différents.
#### Loi de tensions 
$m = \frac{v_{2}(t)}{v_{1}(t)}=\frac{N_{2}}{N_{1}}$ 

