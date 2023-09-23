Exercice 1- 
Dans l'espace muni d'un repère orthonormal $(O,\vec{i},\vec{j},\vec{k})$ on considère l'ensemble $S_m$ d'equation : 
$x^{2}+y^{2}+z^{2}-2(1+m)x+2(2m-1)y -4mz=11-6m$ avec $m$ un réel
1- On cherche a montrer que $S_{m}$ est une sphère
On a :
$$\begin{align*} (x-(1+m))^{2}&=x^{2}-2(1+m)x+1+2m+m^{2} \\ (y+(2m-1))^{2}&=y^{2}+2(2m-1)y +4m^{2}-4m+1 \\ (z-2m)^{2}&=z^{2} -4mz+4m^{2}  \end{align*}$$
On remplace dans $S_m$
$$(x-(1+m))^{2}-1-2m-m^{2}+(y+(2m-1))^{2}-4m^{2}+4m-1+(z-2m)^{2}-4m^{2}=11-6m$$
$$\Leftrightarrow \boxed{(x-(1+m))^{2}+(y+(2m-1))^{2} +(z-2m)^{2}=9m^{2}-8m+13}$$
On a bien l'equation d'une sphère  
de centre $\boxed{\Omega_{m}=\begin{pmatrix} 1+m  \\ 1-2m  \\ 2m \end{pmatrix}}$
et de rayon $\boxed{R_{m}^{2}=9m^{2}-8m+13}$

2-
a- On cherche l'ensemble de points appartenant a toutes les sphères $S_m$ 
$$x^{2}+y^{2}+z^{2}-2(1+m)x+2(2m-1)y -4mz=11-6m$$
$$\Leftrightarrow x^{2}+y^{2}+z^{2}-2x-2y+m(-2x+4y-4z)=11-6m$$
Par identification :
$$\Leftrightarrow \begin{cases} x^{2}+y^{2}+z^{2}-2x-2y=11  \\ -2x+4y-4z=-6 \end{cases}$$
On a :
$$(x-1)^{2}=x^{2}-2x+1$$
$$(y-1)^{2}=y^{2}-2y+1$$
On remplace et on trouve 
$$\Rightarrow \boxed{\begin{cases} (x-1)^{2}+(y-1)^{2}+z^{2}-13=0  \\ -2x+4y-4z+6=0 \end{cases}} \quad (Ts)$$
On a bien une equation de sphère et une equation de plan, donc un cercle.

b- On cherche les points qui appartient à AUCUNE sphère $S_{m}$
$$\forall m \in \mathbb{R}, M \notin S_{m}$$
$$\Leftrightarrow \boxed{M \text{  ne vérifie pas l'equation }S_{m}}$$

c- On cherche les points qui appartient à une seul sphère de $S_m$
On a :
$$x^{2}+y^{2}+z^{2}-2x-2y-11+m(-2x+4y-4z+6)=0$$
$$\Leftrightarrow m= \frac{-x^{2}-y^{2}-z^{2}+2x+2y+11}{-2x+4y-4z+6}$$
$$\Leftrightarrow m= \frac{x^{2}+y^{2}+z^{2}-2x-2y-11}{2x-4y+4z-6}$$
On a donc $m=0$
$$\Leftrightarrow x^{2}+y^{2}+z^{2}-2x-2y-11=0$$
$$\Leftrightarrow \boxed{(x-1)^{2}+(y-1)^{2}+z^{2}-13=0}$$
C'est qui est la même sphère que la question précédant.

3- On définie la droite $D: \begin{cases} x=3+t  \\ y=3-t  \\ z=-1+t \end{cases}$

a- On cherche a determiner le projeté orthogonal de $\Omega_{m} \text{  sur  } D$
On a $\vec{u}= \begin{pmatrix} 1  \\ -1  \\ 1 \end{pmatrix}$ vecteur directeur de $D$
On a le plan $\mathcal{P}$ qui est orthogonal a $D$ et qui passe par $\Omega_{m}$. Avec $\vec{u}$ normal à $\mathcal{P}$.

Alors $\mathcal{P}: x-y+z+cste=0$
On vérifie avec $\Omega_{m}$ et on trouve
$cste = -5m$
Alors on a $\mathcal{P}: x-y+z-5m=0$

Soit $H$ le projeté qu'on cherche, nn a donc le système :
$$\begin{align*}& \begin{cases} H \in D \\ H \in \mathcal{P} \end{cases} \Leftrightarrow \begin{cases} \begin{cases} x=3+t  \\ y=3-t  \\ z=-1+t \end{cases} \\ x-y+z-5m=0 \end{cases} \Leftrightarrow \begin{cases} \begin{cases} x=3+t  \\ y=3-t  \\ z=-1+t \end{cases} \\ (3+t)-(3-t)+(-1+t)-5m=0 \end{cases} \\ \Leftrightarrow& \begin{cases} x= \frac{10+5m}{3} \\ y= \frac{8-5m}{3} \\ z= \frac{5m-2}{3} \\ t= \frac{5m+1}{3} \end{cases} \end{align*}$$
On trouve donc $\boxed{H \begin{pmatrix} \frac{7+2m}{3}  \\ \frac{5+m}{3}  \\ - \frac{m+2}{3} \end{pmatrix}}$

b- On cherche les sphères tel que :
$d(\Omega_{m}H)=R_{m}$                avec $\vec{\Omega_{m}H}= \begin{pmatrix} \frac{7+2m}{3}  \\ \frac{5+m}{3}  \\ \frac{-2-m}{3} \end{pmatrix}$
On a donc 
$$\begin{align*} &\lVert \vec{\Omega_{m}H} =R_{m} \rVert \\ \Leftrightarrow& \frac{(7+2m)^{2}+(m+5)^{2} + (m+2)^{2}}{9}=9m^{2}-8m+13 \\ \Leftrightarrow& 75m^{2}-114m+39=0 \\ \Leftrightarrow& 25m^{2}-38m+13=0 \end{align*}$$
On cherche le discriminant 
$\Delta = 38^{2}-4\times25\times 13= 144$
On a donc
$$\begin{cases} m_{1}= \frac{38+\sqrt{144}}{50}  \\ m_{2}= \frac{38-\sqrt{144}}{50}\end{cases}$$
$$\Leftrightarrow \boxed{\begin{cases} m_{1}= 1  \\ m_{2}= 13/25\end{cases}}$$

Exercice 2: $A, B \text{ et  } C \text{  non aligné.}$

1- 
$\vec{AM} \wedge \vec{AB}=\vec{0}$
$\Leftrightarrow \text{ le vecteur  }\vec{AM} \text{  et  } \vec{AB} \text{  sont coalineaires, cet-à-dire, si  } M \text{  appartient à la droite  }(AB)$
$$\boxed{M \in (AB): \begin{cases} x = x_{A}+t(x_{B}-x_{A})  \\ y = y_{A}+t(y_{B}-y_{A})  \\ z = z_{A}+t(z_{B}-z_{A}) \end{cases}}$$

2- 
a- Par propiété :
$$\vec{AB} \wedge \vec{AM}=\vec{AC}$$
$$\Leftrightarrow \begin{cases} \vec{AB} \cdot \vec{AC}=0 \: (\vec{AB} \text{  orthogonal à  } \vec{AC} )   \\ \vec{AM} \cdot \vec{AC}=0 \: (\vec{AM} \text{  orthogonal à  } \vec{AC} ) \end{cases}$$

Donc si $\vec{AB} \wedge \vec{AM}=\vec{AC}$
alors $\vec{AB} \cdot \vec{AC}=0$

b- On suppose que $\vec{AB} \cdot \vec{AC}=0$
On considère le repère orthonormé direct $\mathcal{R}=(A,\vec{i},\vec{j},\vec{k})$ où $\vec{i}= \frac{1}{\lVert \vec{AB}\rVert} \vec{AB}$, $\vec{j}= \frac{1}{\lVert \vec{AC}\rVert} \vec{AC}$ et $\vec{k}= \vec{i \wedge \vec{j}}$

On suppose que $\vec{AB} \cdot \vec{AC}=0$
Or $A$ est l'origine de $\mathcal{R}$, 
$B$ appartient à l'axe $(o.i)$ 
$C$ appartient à l'axe $(o.j)$ 
On a donc $\vec{AB} \wedge \vec{AM}=\vec{AC}$   (avec $M \begin{pmatrix} x'  \\ y' \\ z' \end{pmatrix}$)
$\Leftrightarrow M$ appartient à l'axe $(o.k)$
$\Leftrightarrow \boxed{\begin{cases} x'=0  \\ y'= 0  \\ z'=t \end{cases} \: ; t \in \mathbb{R}}$

c- On cherche a faire une changement de repère. 

1ere repère: $\mathcal{B}=(O,\vec{e_{1}},\vec{e_{2}},\vec{e_{3}})$  $coord_{B}(M)= \begin{pmatrix} x \\ y \\ z \end{pmatrix}$
2ème repère : $\mathcal{R}=(A,\vec{i}, \vec{j},\vec{k})$  $coord_{R}(M)= \begin{pmatrix} x' \\ y' \\ z' \end{pmatrix}$

Soit
$\vec{OA}=a\vec{e_{1}}+b\vec{e_{2}}+c\vec{e_{3}}$
$\vec{i}=\alpha \vec{e_{1}}+\beta\vec{e_{2}}+\gamma\vec{e_{3}}$
$\vec{j}=\alpha' \vec{e_{1}}+\beta'\vec{e_{2}}+\gamma'\vec{e_{3}}$
$\vec{k}=\alpha'' \vec{e_{1}}+\beta''\vec{e_{2}}+\gamma''\vec{e_{3}}$

On a :
$$\begin{cases} x=a+x'\alpha+y'\alpha' +z'\alpha''  \\ y=b+x'\beta+y'\beta' +z'\beta''  \\ z=c+x'\gamma+y'\gamma' +z'\gamma'' \end{cases}$$

$$\boxed{\Leftrightarrow \begin{cases} x=a+t\alpha'' \\ y=b+t \beta''  \\ z=c+t\gamma'' \end{cases}}$$