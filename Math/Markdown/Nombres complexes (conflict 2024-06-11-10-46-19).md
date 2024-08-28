![[image plan complexe.png|300]]
## Ecriture algébrique
### Conjugué 
$\overline{z}=a-ib$ 
- $\overline{\overline{z} } =z$ 
- $\overline{z+z'} = \overline{z} + \overline{z'}$
- $\overline{z \times z'} = \overline{z} \times \overline{z'}$ 
- $\displaystyle = \overline{\left(\frac{z}{z'}\right)} = \frac{\overline{z} }{\overline{z'} }$
- $\displaystyle Re(z) = \frac{z+\overline{z} }{2}$ 
- $\displaystyle Im(z)=\frac{z-\overline{z} }{2i}$ 

### Module 
$|z|=\sqrt{a^{2}+b^{2}}= \sqrt{z \cdot \overline{z} }$ 
- $|z \cdot z'|= |z||z'|$ 
- $|z|^{2}=\overline{z} z$ 
- $\displaystyle \left|\frac{z}{z'}\right| = \frac{|z|}{|z'|}$ 
- $\displaystyle  z^{-1}= \frac{\overline{z} }{|z|^{2}} = \frac{a-ib}{a^{2}+b^{2}}$
- $|z+z'| \leq |z|+|z'|$
- $|z-z''| \leq |z-z'| + |z'-z''|$

## Nombres complexes de module 1
Ensemble $\mathbb{U}=\{ z \in \mathbb{C} \setminus |z|=1 \}$  
- Dans le plan, $\mathbb{U}$ est représenté par le cercle trigonométrique 
### Forme trigonométrique
$\cos(\theta)+ i \sin(\theta)= e^{i\theta}$ 
- $|e^{i \theta }|=1$
- $e^{i \theta}= e^{i \theta'} \Leftrightarrow \theta = \theta' + 2k \pi$

| $e^{i \pi}  =-1$ | $e^{i2 \pi}=1$ | $e^{i \frac{\pi}{2}}=i$ |
| ---------------- | -------------- | ----------------------- |
### Relations d'Euler 
$\forall \theta \in \mathbb{R}$ 
- $\displaystyle \cos(\theta)= \frac{e^{i \theta}+e^{-i \theta}}{2}$ 
- $\displaystyle \sin(\theta)= \frac{e^{i \theta}-e^{-i \theta}}{2i}$
### L'angle moitie

| $\displaystyle 1+ e^{i \theta}=2\cos\left(\frac{\theta}{2}\right)e^{i \frac{\theta}{2}}$ | $\displaystyle 1-e^{i \theta}= -2i \sin\left(\frac{\theta}{2}\right)e^{i \frac{\theta}{2}}$ |
| ---------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------- |
|    $\displaystyle e^{ip}+e^{iq}=2\cos \left( \frac{p-q}{2} \right) e^{i \frac{p+q}{2}}$                                                                                       |     $\displaystyle e^{ip}-e^{iq}=2i \sin \left( \frac{p-q}{2} \right) e^{i \frac{p+q}{2}}$                                                                                         |
### Formule de Moivre
$\forall \theta \in \mathbb{R}, \forall n \in \mathbb{Z}$ 
$\cos(n \theta)+i \sin(n \theta)=(\cos(\theta)+i \sin(\theta))^{n}$

## Forme trigonométrique
$z=|z|e^{i \theta}=|z|(\cos(\theta)+i \sin(\theta))$ 
### Argument
$\theta = \arg(z)$

| $\displaystyle \cos(\theta)= \frac{a}{\sqrt{a^{2}+b^{2}}}$ | $\displaystyle \sin(\theta)= \frac{b}{\sqrt{a^{2}+b^{2}}}$ | $\displaystyle \tan(\theta)= \frac{b}{a}$ |
| ---------------------------------------------------------- | ---------------------------------------------------------- | ----------------------------------------- |
| $\displaystyle \arg(zz')= \arg(z)+\arg(z')$                | $\displaystyle \arg(z^{n})=n \arg(z)$                      | $\displaystyle \arg \left( \frac{z}{z'} \right) = \arg(z)-\arg(z')$                                           |
### Module
$\rho = |z|$ 
- $\overline{z}= |z|e^{-i \theta}$
- $\displaystyle z^{-1}= \frac{1}{|z|} e^{i \theta}$
- $zz' = |z||z'|e^{i(\theta+\theta')}$
- $a \cos(t) + b \sin(t) = A \cos(t - \varphi)$ 

## Equations 
### Racine carre de un polynôme complexe
Soit $X = \alpha + \beta i$ on pose $\delta = r+si$
et $\delta ^{2}=X \Leftrightarrow \begin{cases} r^{2}+s^{2} = |X| \\ r^{2}-s^{2}= Re(x) \\ 2rs = Im(x)\end{cases}$
### Equations de 2èm dégrée 
si $\Delta \neq 0$ :   $z_{1}= \frac{-b-\delta }{2a}$ et $z_{2}= \frac{-b+\delta }{2a}$
- si $\Delta$ réel positif :  $z_{1}= \frac{-b-\sqrt{\Delta} }{2a}$ et $z_{2}= \frac{-b+\sqrt{\Delta} }{2a}$
- si $\Delta$ réel négatif :  $z_{1}= \frac{-b-i \sqrt{|\Delta|} }{2a}$ et $z_{2}= \frac{-b+ i \sqrt{|\Delta|} }{2a}$
si $\Delta = 0$ :   $z= \frac{-b}{2a}$

### Racines n° de l'unité et d'un nombre complexe $a$ 
#### Solutions de l'equation $z^{n}=1$ :
$\mathbb{U}_{n} = \{ \omega_{k} = e^{i \frac{2k \pi}{n}} \setminus k \in \{ 0, 1, \ldots, n-1 \} \}$
#### Resolution de $z^{n}=a$
$\displaystyle z_{k} = \sqrt[n]{\beta}e^{i(\frac{\alpha}{n}+ \frac{2k \pi}{n})}=\sqrt[n]{\beta}e^{i \frac{\alpha}{n}}\omega_{k}$   

## Exponentielle complexe
Soit $z=a+ib$
- $e^{z}=e^{a+ib}=e^{a}\cdot e^{ib}= e^{a}(\cos(b)+i \sin(b))$ 
- $|e^{z}|=e^{a}$
- $\arg(e^{z})=b$ 

## Nombres complexes et géométrie plane
### Distance entre deux points 
$d(M,M')=|z'-z|$
### Mesure d'un angle
$\displaystyle (\overrightarrow{OM_1 }, \overrightarrow{OM_2 }) = \arg(\frac{z_{2}}{z_{1}})$
$\displaystyle (\overrightarrow{AB}, \overrightarrow{AC}) = \arg(\frac{c-a}{b-a})$
### Alignement 
$\displaystyle M$, $M'$ et $O$ sont alignés  $\Leftrightarrow \arg(z)=\arg(z')[\pi] \Leftrightarrow\displaystyle  \frac{z'}{z}\in \mathbb{R}$ 
$A$, $B$ et $C$ sont alignés $\displaystyle \Leftrightarrow Z= \frac{c-a}{b-a} \in \mathbb{R} \Leftrightarrow Z=\overline{Z}$
### Orthogonalité
$\displaystyle OM \perp OM' \Leftrightarrow \arg(z)= \frac{\pi}{2} + \arg(z')[\pi] \Leftrightarrow\displaystyle \frac{z'}{z} \in i\cdot \mathbb{R}$
$\displaystyle AB \perp CD \Leftrightarrow Z= \frac{d-c}{b-a} \in i \cdot \mathbb{R} \Leftrightarrow Z=-\overline{Z}$

