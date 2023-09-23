#geometrie
- Un plan $\mathcal{P}$ dans l'espace n'a aucune orientation, il suffit de choisir un vecteur $\overrightarrow{k} \perp \mathcal{P}$ 
- Coordonnées cylindriques : $(r, \theta, z) : \begin{cases} x= r \cos(\theta)  \\ y= r \sin(\theta)  \\ z=z \end{cases}$ 
## Produit vectoriel 
$\mathcal{P}$ plan contenant $\overrightarrow{u}$ et $\overrightarrow{v}$, $\overrightarrow{k}$ unitaire et normal à $\mathcal{P}$.
- $\overrightarrow{u} \wedge \overrightarrow{v}=[\overrightarrow{u}, \overrightarrow{v}]\cdot \overrightarrow{k} = \| \overrightarrow{u} \| \| \overrightarrow{v} \| \sin(\theta) \cdot \overrightarrow{k}$ 
- $\| \overrightarrow{u} \wedge \overrightarrow{v} \| = \| \overrightarrow{u} \|  \| \overrightarrow{v} \| |\sin(\theta)|$  aire du parallélogramme. 
- $\overrightarrow{u} \wedge \overrightarrow{v}=\overrightarrow{0} \Leftrightarrow \overrightarrow{u} \text{  et  } \overrightarrow{v}$  sont colinéaires.
- $\overrightarrow{u} \wedge \overrightarrow{v} = \begin{pmatrix} x \\ y \\ z \end{pmatrix} \wedge \begin{pmatrix} x' \\ y' \\ z' \end{pmatrix} = \begin{pmatrix} yz' - zy' \\ -(xz'-zx') \\ xy'-yx' \end{pmatrix}$ 
- $\overrightarrow{w}= \overrightarrow{u} \wedge \overrightarrow{v} \Leftrightarrow \overrightarrow{u} \cdot \overrightarrow{w}=0 \text{  et  } \overrightarrow{v} \cdot \overrightarrow{w}=0$  

## Produit mixte 
$[\overrightarrow{u}, \overrightarrow{v}, \overrightarrow{w}] = (\overrightarrow{u}\wedge \overrightarrow{v})\cdot \overrightarrow{w}$ 
- $[\overrightarrow{u}, \overrightarrow{v}, \overrightarrow{w}] = 0 \Leftrightarrow \overrightarrow{u} \wedge \overrightarrow{v} \perp \overrightarrow{w}$   et  $\overrightarrow{u}, \overrightarrow{v} \text{  et  } \overrightarrow{w}$ sont coplanaires.
- $[\overrightarrow{u}, \overrightarrow{v}, \overrightarrow{w}]$ mesure le volume du parallélépipède. 
- $[\overrightarrow{u}, \overrightarrow{v}, \lambda \overrightarrow{w_{1}}+ \mu \overrightarrow{w_{2}}]= \lambda [\overrightarrow{u}, \overrightarrow{v}, \overrightarrow{w_{1}}] + \mu [\overrightarrow{u}, \overrightarrow{v}, \overrightarrow{w_{2}}]$ 

## Plans
$\begin{cases} x= x_{A}+s \alpha + t \alpha' \\ y= y_{A}+s \beta + t \beta' \\ z= z_{A}+s \gamma + t \gamma' \end{cases}$   $\overrightarrow{AM} = s \overrightarrow{u} + t \overrightarrow{v}$ 
- $ax+by+cz+d=0 \Leftrightarrow \overrightarrow{AM}\cdot \overrightarrow{n}=0$ 
- $M \in \mathcal{P} \Leftrightarrow [\overrightarrow{AM}, \overrightarrow{u}, \overrightarrow{v}]=0$ 

## Droites 
$\begin{cases} x= x_{A}+t \alpha \\ y= y_{A}+t \beta \\ z= z_{A}+t \gamma \end{cases}$ 
- On a besoin de deux équations cartésiennes pour décrire une droite.
### Projeté orthogonal 
- $\displaystyle d(M, \mathcal{P})= \frac{|a x_{M}+b y_{M} + c z_{M}+d|}{\sqrt{a^{2}+b^{2}+c^{2}}}$ 
- $\displaystyle d(M, \mathcal{P})= \frac{|\overrightarrow{AM} \cdot \overrightarrow{n}|}{\| \overrightarrow{n} \|}$  
- $\displaystyle d(M, \mathcal{P})= \frac{|\overrightarrow{AM} \wedge \overrightarrow{u}|}{\| \overrightarrow{u} \|}$ 

## Sphère 
$(x-a)^{2}+(y-b)^{2}+(z-c)^{2}=R^{2}$ 

## Cercle
Il faut une équation de sphère et une équation de plan.