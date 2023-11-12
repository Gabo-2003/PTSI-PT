#chapitre19 #electromagnetique 
Il est toujours justifiée de négliger le poids
## Champ électrostatique : charge Q sur q
### Loi de Coulomb : $\vec{F_{el}}=q \vec{E}$
- $\displaystyle \vec{F_{el}}=\frac{1}{4\pi \epsilon_{0}} \frac{qQ}{r^{2}} \vec{u}$ 
- $\lVert \vec{E} \rVert$ en $V/m$
### Principe de superposition : $\vec{F_{tot}}= \sum_{}^{}\vec{F_{i}}$

## Champ magnétostatique : 
Les charges en mouvement exercent les uns sur les autres forces magnétiques 
- $\vec{F_{mag}}=q \vec{v}\wedge \vec{B}$
- $\vec{F_{mag}}$ ne travaille pas

## Force de Lorentz : $\vec{F_{L}} = \vec{F_{el}} + \vec{F_{mag}}$ 
- $\vec{F_{L}}=q(\vec{E}+\vec{v}\wedge \vec{B})$
- $\mathcal{P}_{L}=q \vec{E} \cdot \vec{v} = \mathcal{P}_{el}$

## Mouvement dans un champ $\vec{E}$ uniforme:
- $\begin{cases} x(t) = v_{0x}t+ \frac{qE}{2m}t^{2} \\ y(t)=v_{0y}t \\ z(t)=v_{0z}t \end{cases}$
### Acceleration entre deux electrodes : $\vec{E}=E \vec{e_{x}}$
$$\begin{align*} \vec{F}&=-\vec{grad}(E_{p})\\ \Rightarrow E_{p}(x)&=-qEx+cte \\ \text{Or  } &V(x)=\frac{E_{p}(x)}{q} \\ &\boxed{V(x)=-Ex+C}  \end{align*}$$
Alors 
$$\begin{align*} &U = V(-\frac{d}{2})-V\left(\frac{d}{2}\right)\\ &\boxed{E=\frac{U}{d}} \end{align*}$$
### Conservation de l'énergie mécanique 
- $v_{f} = \sqrt{\frac{2|q|U}{m}}$ 
## Mouvement dans un champ $\vec{B}=B \vec{e_{z}}$ uniforme
- $\lVert \vec{v} \rVert$ est constante donc le mouvement est uniforme (on le démontre avec le théorème de la puissance cinétique)
- Mouvement circulaire et plane (on le démontre avec une PFD sur $\vec{e_{z}}$)
### Sense de parcours : $\vec{v}=R\dot{\theta} \vec{e_{\theta}}$
- Direct si $\dot{\theta}>0$
- Indirect si $\dot{\theta}<0$
### Pulsation cyclotron : $\displaystyle \omega_{c}= \frac{|q|B}{m}$
- démontré avec une PFD et les [[Mouvement d'un point#Système polaire|coordonnées polaires]]
### Rayon : $\displaystyle R=\frac{v_{0}m}{|q|B}$
- d'après $\displaystyle R=  \frac{\lVert \vec{v} \rVert}{\omega_{c}}$
