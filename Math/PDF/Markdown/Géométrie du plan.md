#geometrie 
- $\mathcal{P}$ : ensemble des points du plan de repère cartésienne$\mathcal{R}=(O,\vec{e_{1}},\vec{e_{2}})$ 
- $\mathcal{V}$ : ensemble des vecteurs du plan de base$\mathcal{B}=(\vec{e_{1}}, \vec{e_{2}})$ 
- Repère orthonormal $\mathcal{R}$ direct si pour passer de $\vec{e_{1}}$ à $\vec{e_{2}}$ on fait $+ \frac{\pi }{2}$ dans le sens trigo.
### Changement de repère 
On part de l'égalité $\overrightarrow{OM}=\overrightarrow{OO'}+\overrightarrow{O'M}$ 
- $\overrightarrow{OO'}=a \vec{e_{1}} + b \vec{e_{2}}$ 
- $\vec{e'_{1}} = \alpha \vec{e_{1}} + \beta \vec{e_{2}}$
- $\vec{e'_{2}} = \gamma  \vec{e_{1}} + \delta  \vec{e_{2}}$
### Coordonnées polaires
- $x=r \cos(\theta)$ 
- $y = r \sin(\theta)$ 

## Produit scalaire 
- $\overrightarrow{u} \cdot \overrightarrow{v} = \| \overrightarrow{u} \| \cdot \| \overrightarrow{v} \| \cos(\overrightarrow{u},\overrightarrow{v})$           $\overrightarrow{u} \cdot \overrightarrow{v} = \overline{OA} \cdot \overline{OH}$
- $\| \overrightarrow{u} \| = \sqrt{x^{2}+y^{2}}$                        $\| \overrightarrow{u} \|^{2} = \overrightarrow{u} \cdot \overrightarrow{u}$

## Produit mixte 
- $[\overrightarrow{u}, \overrightarrow{v}] = \|  \overrightarrow{u} \| \| \overrightarrow{v} \| \sin(\overrightarrow{u}, \overrightarrow{v})$            $[\overrightarrow{u}, \overrightarrow{v}] = \overline{OA} \cdot \overline{HB}$
- Aire du triangle $OAB$ :  $\frac{1}{2}[\overrightarrow{OA}, \overrightarrow{OB}]$
- $\overrightarrow{u}$ et $\overrightarrow{v}$ colinéaires $\Leftrightarrow [\overrightarrow{u}, \overrightarrow{v}] = 0$
- $A$,  $B$ et  $C$ alignes  $\Leftrightarrow [\overrightarrow{AB}, \overrightarrow{AC}]=0$
- $[\overrightarrow{u}, \overrightarrow{v}] = - [\overrightarrow{v}, \overrightarrow{u}]$ 
- $[\overrightarrow{u}, \overrightarrow{v}]= xy' -yx' = \begin{vmatrix} x & x' \\ y & y' \end{vmatrix}$

## Droites du plan 
Soit la droite $D$ passant par $A \begin{pmatrix} x_{A} \\y_{A} \end{pmatrix}$ et dirigé par $\overrightarrow{u} \begin{pmatrix} \alpha  \\ \beta  \end{pmatrix}$ 
- $M \in D  \Leftrightarrow \overrightarrow{AM}$ colinéaire à $\overrightarrow{u} \Leftrightarrow \overrightarrow{AM} = t \overrightarrow{u} \Leftrightarrow \begin{cases} x= x_{A} + t \alpha \\ y=y_{A} +t \beta \end{cases}$  
### Equation de la droite
- $M \in D \Leftrightarrow [\overrightarrow{AM}, \overrightarrow{u}]=0 \Leftrightarrow \beta x - \alpha y + \alpha y_{A} - \beta x_{A}=0$.           $ax+by+c=0$        $\overrightarrow{n}=\begin{pmatrix} a \\ b \end{pmatrix}$
- $M \in D \Leftrightarrow \overrightarrow{AM} \cdot \overrightarrow{n} = 0 \Leftrightarrow a(x-x_{A}) + b(y-y_{A})=0$ 
### Projeté orthogonal d'un point sur une droite
$d(M,D)=MH$
- $\displaystyle HM= \frac{|\overrightarrow{n} \cdot \overrightarrow{AM}|}{\| \overrightarrow{n} \|} = d(M,D)$ 
- $\displaystyle HM= \frac{|[\overrightarrow{u}, \overrightarrow{AM}]|}{\| \overrightarrow{u} \|} = d(M,D)$
- $\displaystyle HM = \frac{|a x_{M}+b y_{M} + c|}{\sqrt{a^{2}+b^{2}}}$

## Cercles dans le plan
Cercle $\mathcal{C}$ de centre $\Omega (a,b)$ et de rayon $R>0$.
- $(x-a)^{2}+(y-b)^{2}=R^{2}$  
- $x^{2}+y^{2}-2ax -2by +c=0$ 

