#chapitre14 #mecanique 
## Puissance et Travail d'une force 
### Puissance
$\mathcal{P}(\overrightarrow{f}) = \overrightarrow{f}\cdot \overrightarrow{v}$ 
#### Motrice : $\mathcal{P}(\overrightarrow{f})>0$ 
#### Résistante : $\mathcal{P}(\overrightarrow{f})<0$
### Travail 
#### Travail élémentaire
$\delta W(\overrightarrow{f})=\overrightarrow{f}\cdot \overrightarrow{dl}$  en $J$ 
- $\overrightarrow{dl}=\overrightarrow{v} \, dt$ 
#### Travail macroscopique 
$\displaystyle W_{A \to b}(\overrightarrow{f}) = \int_{A,(\mathcal{C})}^{B}\delta W(\overrightarrow{f})$      
- Le travail dépende de la manière dont le trajet est réalisé. 

## Théorème de l'énergie et de la puissance cinétique 
- $E_{c}=\frac{1}{2}m \overrightarrow{v}^{2}$ 
- Valables que pour un [[Dynamique Newtonienne#1ère loi Principe d'inertie|référentielle galiléen]].
### Théorème de la puissance cinétique
$\displaystyle \frac{dE_{c}}{dt}= \sum \mathcal{P}(\overrightarrow{f})$ 
### Théorème de la énérgie cinétique 
$\displaystyle \Delta E_{c}=\sum W_{A \to B}(\overrightarrow{f})$ 

## Forces conservatives et énergie potentielle
### [[Dérivées partielles]] 
Se calcule "normalement" la fonction en faisant comme s'il s'agissait uniquement d'une fonction $x_{i}$. 
### [[Gradient d'une fonction]] 
$\displaystyle\overrightarrow{\nabla}f= \frac{\partial f}{\partial x}\overrightarrow{e_{x}}+ \frac{\partial f}{\partial y}\overrightarrow{e_{y}}+\frac{\partial f}{\partial z}\overrightarrow{e_{z}}$ 
- $\overrightarrow{\nabla}f \cdot \overrightarrow{dl} =df$ 
### Forces conservatives 
Si son travail entre deux points $A$ et $B$ ne dépend que des positions de ces points. 
- $\delta W (\overrightarrow{f})=-d  E_{p}$ 
- $W_{A \to B}(\overrightarrow{f}) = - \Delta E_p$ 
- $\overrightarrow{f}=\overrightarrow{\nabla}E_p$ 
#### Poids
$W_{A \to B}(\overrightarrow{P})=mg(z_{A}-z_{B})$ 
- $E_{p}=mgh$                   $h=z-z_{ref}$ 
#### Gravitationnelle
$\displaystyle W_{A \to B} (\overrightarrow{F_{g}})=G M_{m}(\frac{1}{R_{B}}- \frac{1}{R_{A}})$ 
- $\displaystyle E_{pg}=-G \frac{m M}{r}$  
#### Rappel élastique : 
$\displaystyle W_{A\to B} (\overrightarrow{f_{r}})= \frac{1}{2} k((\Delta x_{B}^{2} - \Delta x_{A}^{2}))$ 
- $E_{p}(x)=\frac{1}{2} k (\Delta x)^{2}$ 
### Forces non-conservatives
- Le frottement 

## Energie mécanique 
$E_{m}=E_{c}+ E_{p}$ 
- L'énergie potentielle totale est la somme des différents formes d'énergie potentielles. 
### Théorème de l'énergie mécanique
$\Delta E_{m}=W(\overrightarrow{F_{nc}})$           (forces non conservatives)

## Mouvement unidimensionnel d'une particule soumise à une force conservative 
### Positions accessibles
$$\begin{align*} E_{m}&=E_{c}+E_{p}=cte \quad \text{  or  } E_{c} \geq 0 \\ E_{m}-E_{p} &\geq 0 \\ E_{m} &\geq E_{p} \end{align*}$$ Alors le mobile ne peut accéder qu'aux positions $x$ pour lesquelles la courbe de l'énergie potentielle $E_{p}=f(x)$ est en dessous de la droite $y=E_{m}$ 
![[image positions accesibles.png|600]]
#### $\textcolor{red}{\text{Etat lié}}$ 
Trajectoire bornée.
- Les position accessibles sont telles que $x \in [x_{1},x_{2}]$.
- On a $E_{c}(x_{1})=E_{c}(x_{2})=0$ : La vitesse est nulle aux positions extrémales.
#### $\textcolor{blue}{\text{Etat de diffusion}}$
Trajectoire non bornée.
- Les positions accessibles vérifient $x \geq x_{3}$ 
### Position d'équilibre, stabilité
Une position $x$ est dit  d'équilibre si le système n'en bouge pas lorsqu'il est à vitesse nulle : $f(x)=0$.
- Les positions d'équilibre sont les extremums locaux. 
- La position est stable si la force s'oppose au déplacement : $\displaystyle \frac{d^{2}E_{p}}{dx^{2}}(x_{0})>0$ 
![[image equilibre stabilite.png]]
#### Stable
Minimum de $E_{p}$.
#### Instable
Maximum de $E_{p}$.
### Petits mouvements au voisinage d'équilibre 
Tout mouvement au voisinage d'une position d'équilibre stable peut s'interpréter comme un oscillateur harmonique.
### Barrière de potentiel 
Le mobile doit posséder une énergie mécanique suffisante pour atteindre chacune de ces positions intermédiaires.
![[image barrière de potentiel.png]]