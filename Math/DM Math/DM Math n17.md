1- $\Gamma$ représente le cercle qui passe par les points $A$, $B$, $C$
![[Pasted image 20230205205638.png]]

2- 
$\alpha = 1+(1-\sqrt{2})^{2}=1+1+2\sqrt{2}=4+2\sqrt{2}$
$\beta=(4-2\sqrt{2})(4+2\sqrt{2})=16+8\sqrt{2}-8\sqrt{2}-8=8$
$\gamma=(3-2\sqrt{2})(3+2\sqrt{2})=9+6\sqrt{2}-6\sqrt{2}-8=1$

3- On cherche une equation cartésienne de droites de $(AB)$
$\vec{AB}=\begin{pmatrix} 0-\sqrt{2} \\ \sqrt{2}-0 \end{pmatrix} = \begin{pmatrix} -\sqrt{2}  \\ \sqrt{2} \end{pmatrix}$ alors on a $\vec{n_1}\begin{pmatrix} -\sqrt{2} \\ -\sqrt{2} \end{pmatrix}$ une vecteur normal de AB. 
On a donc :
$-\sqrt{2}x-\sqrt{2}y+cst =0$ 
On vérifie avec le point $A$ :
$\begin{align*} -\sqrt{2}\times(\sqrt{2}) -\sqrt{2}\times0 +cst&=0 \\ \Leftrightarrow cst&=2 \end{align*}$
Alors on a $\boxed{-\sqrt{2}x-\sqrt{2}y+2=0}$, une equation de droite de $(AB)$

On cherche une equation cartésienne de droites de $(AC)$
$\vec{AC}= \begin{pmatrix} -1 -\sqrt{2} \\ -1-0 \end{pmatrix}=\begin{pmatrix} -1-\sqrt{2} \\ -1 \end{pmatrix}$ alors on a $\vec{n_2}=\begin{pmatrix} 1 \\ -1-\sqrt{2} \end{pmatrix}$
On a donc :
$x+(-1-\sqrt{2})y+cst=0$
On vérifie avec $A$ : 
$\begin{align*} \sqrt{2}+0 +cst=0 \\ \Leftrightarrow cst =-\sqrt{2} \end{align*}$
Alors on a $\boxed{x+(-1-\sqrt{2})y-\sqrt{2}=0}$, une equation de droite de $(AC)$

On cherche une equation cartésienne de droites de $(BC)$
$\vec{BC}= \begin{pmatrix} -1-0  \\ -1-\sqrt{2} \end{pmatrix} = \begin{pmatrix} -1 \\ -1-\sqrt{2} \end{pmatrix}$ alors on a $\vec{n_3}=\begin{pmatrix} 1+\sqrt{2} \\ -1 \end{pmatrix}$
On a donc : 
$x(1+\sqrt{2})-y+cst=0$
On vérifie avec $B$ :
$\begin{align*}0-\sqrt{2}+cst&=0\\ \Leftrightarrow cst &= \sqrt{2}\end{align*}$
Alors on a $\boxed{x(1+\sqrt{2})-y+\sqrt{2}=0}$, une equation de droite de $(BC)$

4- 
a- On cherche les coordonnées de $P$, projeté orthogonal de $M$ sur $(AB)$. On pose $P=\begin{pmatrix} x  \\ y \end{pmatrix}$
Par définition, $\vec{PM}$ et $\vec{AB}$ sont orthogonales, Alors :
$$\begin{align*} &\vec{PM} \cdot \vec{AB}=0 \\ \Leftrightarrow& (a-x)(-\sqrt{2})+(-a-y)(\sqrt{2})=0 \\ \Leftrightarrow&-a \sqrt{2}+x \sqrt{2} -a \sqrt{2} -y \sqrt{2} =0 \\ \Leftrightarrow& x-y-2a = 0 \end{align*}$$

$P$ appartient a $(AB)$ si $\vec{AP}$ et $\vec{AB}$ sont colinéaires.
$$\begin{align*} &[\vec{AP},\vec{AB}]=0 \\ \Leftrightarrow& \begin{vmatrix} x-\sqrt{2}  & -\sqrt{2}\\ y & \sqrt{2} \end{vmatrix}=0 \\ \Leftrightarrow& x \sqrt{2}-2+y \sqrt{2} =0 \\ \Leftrightarrow& \sqrt{2}(x+y)-2 =0  \end{align*}$$

Alors avec les deux résultats  on a le système :
$$\begin{align*} &\begin{cases} x=y+2a  \\ x \sqrt{2}-2+y \sqrt{2}=0  \end{cases} \Leftrightarrow \begin{cases} x=y+2a  \\ y \sqrt{2}+2a \sqrt{2}-2 +y \sqrt{2} =0 \end{cases} \Leftrightarrow \begin{cases} x = \frac{1}{\sqrt{2}}-a+2a \\ 2y \sqrt{2} =2 - 2a \sqrt{2}  \end{cases} \\ \Leftrightarrow& \begin{cases} x=\frac{\sqrt{2}}{2}+a \\ y=\frac{\sqrt{2}}{2}-a \end{cases} \end{align*}$$
Alors $\boxed{P \begin{pmatrix} \frac{\sqrt{2}}{2}+a \\ \frac{\sqrt{2}}{2}-a  \end{pmatrix}}$

b- 
On cherche les coordonnées de $Q$, projeté orthogonal de $M$ sur $(AC)$. On pose $Q=\begin{pmatrix} x  \\ y \end{pmatrix}$
Par définition, $\vec{QM}$ et $\vec{AC}$ sont orthogonales, Alors :
$$\begin{align*} &\vec{QM} \cdot \vec{AC}=0 \\ \Leftrightarrow& (a-x)(-1-\sqrt{2})+(-a-y)(-1)=0 \\ \Leftrightarrow& x(1+\sqrt{2}) +y -a \sqrt{2}=0 \end{align*}$$

$Q$ appartient a $(AC)$ si $\vec{AQ}$ et $\vec{AC}$ sont colinéaires.
$$\begin{align*} &[\vec{AQ},\vec{AC}]=0 \\ \Leftrightarrow& \begin{vmatrix} x-\sqrt{2}  & -1-\sqrt{2}\\ y & -1 \end{vmatrix}=0 \\ \Leftrightarrow& \sqrt{2}-x+y(1+ \sqrt{2})=0  \end{align*}$$

Alors on a le system : 
$$\begin{align*} &\begin{cases} x(1+\sqrt{2}) +y -a \sqrt{2}=0 \\ \sqrt{2}-x+y(1+ \sqrt{2})=0  \end{cases} \Leftrightarrow \begin{cases} x(1+\sqrt{2})+ \frac{x-\sqrt{2}}{1+\sqrt{2}} -a \sqrt{2}=0 \\ y=\frac{x-\sqrt{2}}{1+\sqrt{2}} \end{cases} \Leftrightarrow \begin{cases} x= \frac{\sqrt{2}}{2\sqrt{2}+4} +\frac{ a \sqrt{2} (1+\sqrt{2})}{2\sqrt{2}+4} \\ y=\frac{1}{1+\sqrt{2}}\times(\frac{-\sqrt{2}-1}{2}+ \frac{a}{2} )  \end{cases} \\ \Leftrightarrow& \begin{cases} x=\frac{-1+\sqrt{2}}{2} +\frac{a}{2} \\ y=-\frac{1}{2} +a \frac{\sqrt{2}-1}{2} \end{cases}\end{align*}$$
Alors $\boxed{Q \begin{pmatrix} \frac{-1+\sqrt{2}}{2} +a\frac{1}{2}  \\ -\frac{1}{2} +a \frac{\sqrt{2}-1}{2}  \end{pmatrix}}$

5- Montrer que les points $P$, $Q$ et $R$ sont alignés si et seulement si $M$ appartient à $\Gamma$. 
Ces trois points sont alignés si, et seulement si :
$[\vec{PQ}, \vec{PB}]=0$
On commence par chercher les deux vecteurs
$\vec{PQ} \begin{pmatrix} \frac{-1+\sqrt{2}}{2} +\frac{a}{2} - \frac{\sqrt{2}}{2}-a  \\ -\frac{1}{2} +a \frac{\sqrt{2}-1}{2} - \frac{\sqrt{2}}{2} +a\end{pmatrix} = \begin{pmatrix} - \frac{1}{2}-a \frac{1}{2}  \\ - \frac{\sqrt{2}+1}{2} +a \frac{\sqrt{2}+1}{2} \end{pmatrix}$
$\vec{PB} \begin{pmatrix} - \frac{1}{2} +a \frac{1-\sqrt{2}}{ 2} - \frac{\sqrt{2}}{2} -a  \\ \frac{\sqrt{2}-1}{2}-a \frac{1}{2}- \frac{\sqrt{2}}{2}+a \end{pmatrix} = \begin{pmatrix} - \frac{\sqrt{2}+1}{2} -a \frac{\sqrt{2}+1}{2} \\ - \frac{1}{2}+a \frac{1}{2} \end{pmatrix}$
Alors :
$$\begin{align*} &[\vec{PQ}, \vec{PB}]=0 \\ \Leftrightarrow&  \begin{vmatrix} - \frac{1}{2}-a \frac{1}{2}  & - \frac{\sqrt{2}+1}{2} -a \frac{\sqrt{2}+1}{2} \\ - \frac{\sqrt{2}+1}{2} +a \frac{\sqrt{2}+1}{2} & - \frac{1}{2}+a \frac{1}{2} \end{vmatrix} =0 \\ \Leftrightarrow& (\frac{1}{4}-a \frac{1}{4}+a \frac{1}{4}-a^{2} \frac{1}{4})-(\frac{2\sqrt{2}+3}{4} +a \frac{2\sqrt{2}+3}{4}-a \frac{2\sqrt{2}+3}{4} -a^{2}\frac{2\sqrt{2}+3}{4})=0 \\ \Leftrightarrow& - \frac{\sqrt{2}+1}{2} +a^{2} \frac{\sqrt{2}+1}{2} =0 \end{align*}$$
$\boxed{\Leftrightarrow a = \pm 1}$

Or $||\vec{OM}|| = \sqrt{2}$ pour $a = \pm 1$ 
Alors $M \in \Gamma$ si $a=\pm1$
Alors $P$, $Q$ et $R$ sont alignés si et seulement si $M \in \Gamma$

6- 
a- Or $C_a$ tangente a $(AB)$, et $P$ le projeté orthogonal de $M$ sur $(AB)$. Alors la distance $d(M,P)=R$ avec $R$ le rayon de $C_a$.
$||\vec{MP}||=\sqrt{(\frac{\sqrt{2}}{2})^{2}+(\frac{\sqrt{2}}{2})^{2}}=1$
Alors on a l'équation cartésienne 
$\boxed{(x-a)^{2}+(y+a)^{2}=1}$

b- On cherche les valeurs de $a$ tel que $d(M,(AC))=1$

$$\begin{align*} \Leftrightarrow& \frac{|x_{m}+(-1-\sqrt{2})y_{m}-\sqrt{2}|}{\sqrt{2\sqrt{2}+4}}=1 \Leftrightarrow  \frac{|2a+a\sqrt{2}-\sqrt{2}|}{\sqrt{2(\sqrt{2}+2)}}=1 \\ \Leftrightarrow& |2a +a \sqrt{2} -\sqrt{2}|=\sqrt{2(\sqrt{2}+2)} \end{align*}$$ 
$$\Leftrightarrow \boxed{\begin{cases} a_{1}&=\frac{\sqrt{2(\sqrt{2}+2)}+\sqrt{2}}{2+\sqrt{2}} &\approx 1,179 \\ a_{2}&=\frac{-\sqrt{2(\sqrt{2}+2)}+\sqrt{2}}{2+\sqrt{2}} &\approx -0,351 \end{cases}}$$
