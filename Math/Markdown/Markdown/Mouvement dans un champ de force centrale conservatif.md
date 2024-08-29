## [[Champ]] de force central conservatif
### Force centrale
Une force $\overrightarrow{f}$ appliquée à un point matériel $M$ est centrale si sa droite d'action passe toujours par un point $O$ fixe dans le référentielle d'étude $\mathcal{R}$. 
### Conservative 
$\displaystyle \overrightarrow{f}= f_{r}(r)\overrightarrow{e_{r}} = - \frac{d E_{p}}{dr} \overrightarrow{e_{r}}$       avec $E_{p}=E_{p}(r)$
#### Rappel élastique 
$\overrightarrow{f}= -k(r-l_{0})\overrightarrow{e_{r}}$           $E_{p}= \frac{1}{2}k(r-l_{0})^{2}+C$
#### Gravitation 
$\displaystyle \overrightarrow{f}=-G \frac{M m}{r^{2}} \overrightarrow{e_{r}}$             $E_{p} = -G \frac{Mm}{r}+C$
#### Electrostatique 
$\displaystyle \overrightarrow{f}= \frac{1}{4 \pi \varepsilon_{0} \frac{Qq}{r^{2}}} \overrightarrow{e_{r}}$              $E_{p} = \frac{1}{4 \pi \varepsilon_{0}} \frac{Qq}{r} + C$
### Conséquences
TMC : $\displaystyle \frac{d \overrightarrow{\mathcal{L}}(O)}{dt}= M_{O}(\overrightarrow{F}) = \overrightarrow{OM} \wedge \overrightarrow{F} = \overrightarrow{0}$  car les deux vecteurs sont coalinéaires.        
$\Rightarrow\overrightarrow{\mathcal{L}}(O)=mr^{2}\dot{\theta}\overrightarrow{e_{z}} = cte$ 
- $\dot{\theta}>0$ : trajectoire conique 
#### 1èr Loi de Kepler 
Les planètes du système solaire orbitent autour du soleil selon des trajectoires elliptiques dont le soleil est un des foyers. 
#### 2ème Loi de Kepler
Loi des aires, l'aire balayée par le vecteur position d'un corps pendant une durée $\Delta t$ est constante sur tout la trajectoire.
$\displaystyle d \mathcal{A} = \frac{r \cdot r d \theta}{2 } \Rightarrow \frac{d \mathcal{A}}{dt} = \frac{1}{2} r^{2} \dot{\theta }$
- $\displaystyle \frac{d \mathcal{A}}{dt} =\frac{C}{2}$             avec $C=r^{2}\dot{\theta}$  trove avec le moment cinétique conservative.

## Etude énergétique
- Energie mécanique conservé : $\displaystyle \overrightarrow{v}(r)=\sqrt{\frac{2(E_{m}-E_{p}(r))}{m}}$ 
- Energie potentielle effective : $E_{p,eff}=E_{p}(r) + \frac{1}{2}m \frac{C^2 }{r^{2}}$ 
	- $E_{m} \geq E_{p,eff}$ 
### Théorème du viriel 
$E_{c} = -\frac{1}{2} E_{p}$

## [[Champ]] Newtonien 
(Force gravitationnelle, de Coulomb)
$\displaystyle \overrightarrow{f}(r)= \frac{k}{r^{2}}\overrightarrow{e_{r}}$       $E_{p}(r)= \frac{k}{r}$     $\dot{\theta} =cst$  mouvement uniforme 
### Mouvement circulaire
Système solaire par exemple
- $v=\sqrt{-\frac{k}{mr_{0}}}$                    $\omega = \sqrt{\frac{GM}{r_{0}^{3}}}$ 
#### 3èm Loi de Kepler
$\displaystyle \frac{T^{2}}{r_{0}^{3}} = \frac{4 \pi^{2}}{GM}$ 
- On remplace $r_0$ par $a$ pour un ellipse
- $\displaystyle E_{c}=-\frac{1}{2} \frac{k}{r_{0}}$      $\displaystyle E_{p} = \frac{k}{r_{0}}=-2 E_{c}$      $\displaystyle E_{m}=\frac{k}{2r_{0}}$ 
### Mouvement elliptique 
- Non uniforme $E_{c}$ et $E_{p}$ pas constantes 
- $\displaystyle r= \frac{k \pm \sqrt{k^{2}+2mC^{2}E_{m}}}{2E_{m}}$      $E_{m}=\frac{k}{2a}$ 
### Satellite géostationnaire 
Un satellite ne peut pas être géostationnaire si son orbite n'est pas comprise dans le plan de l'équateur. 

## Champ gravitationnelle 
### Champ
$\displaystyle \overrightarrow{G} = - \mathcal{G} \frac{M}{r^{2}} \overrightarrow{e_{r}}$ 
### Flux
$\displaystyle \phi_{G} = \iint \overrightarrow{G} \cdot \overrightarrow{ds}$  
### Théorème de Gauss  
Le flux du champ gravitationnel au travers d'une surface fermée est égal à la masse contenue dans cette surface multipliée par $-4\pi \mathcal{G}$
$\displaystyle \oint\oint_{S} \overrightarrow{G} \cdot \overrightarrow{ds} = -4\pi \mathcal{G} M$ 
- On peut trouver le champ magnétique engendrée par une distribution de masse (avec beaucoup de symétrie). 
- Les symétries et invariances suivent les mêmes règles que le champ électrique. 