#chapitre10 #mecanique #electricite #signal
On appelle signal physique une grandeur physique qui dépend du temps.

## Oscillateur harmonique mécanique
### Force de rappel d'un ressort 
$\overrightarrow{F_{rm}} = \pm k((l_{0}\pm d)-l_{0}) \overrightarrow{e_{x}}$
- Compression : $+$ 
- Extension : $-$
- $(l_{0}\pm d)$ : longueur ressort affecté 
### Equation du mouvement
$\ddot{x}+\frac{k}{m} x =0$   
#### Forme canonique 
$\ddot{x}+\omega^{2} x =0$  
- Avec $\omega^{2} = \frac{k}{m}$ en $rad \cdot s^{-1}$ 

## Résolution de l'équation 
### Forme générale 
$\begin{cases} S_{1}= C_{1}\cos(\omega_{1} t)  \\ S_{2}= C_{2}\sin(\omega_{2} t) \end{cases}$ 
$S(t)=S_{1}(t)+ S_{2}(t) = C_{1}\cos(\omega_{1} t) + C_{2}\sin(\omega_{2} t)$ 
$S(t)=A \cos(\omega_{0}t+ \varphi)$ 
### Conditions aux limites 
Il faut autant des conditions aux limites indépendantes que de constantes. 
$\begin{cases} x(0)=x_{0}  \\ \dot{x}(0)=v_{0} \end{cases}$ 
- $\varphi = - \arctan(\frac{v_{0}}{\omega_{0} x_{0}})$       si $x_{0}>0$
- $\varphi =\pi - \arctan(\frac{v_{0}}{\omega_{0} x_{0}})$    si $x_{0}<0$ 
- $A = x_{0}\sqrt{1+(\frac{v_{0}}{\omega_{0} x_{0}})^{2}}$     si $x_{0}>0$ 
- $A = - x_{0}\sqrt{1-(\frac{v_{0}}{\omega_{0} x_{0}})^{2}}$  si $x_{0}<0$ 

## Etude énergétique 
### Energie potentielle d'un ressort 
$E_{p}=\frac{1}{2} k x^{2}$ 
### Conservation de l'énergie mécanique 
On multiplie l'équation du mouvement par la quantité de mouvement $m\dot{x}$ :
$\displaystyle \frac{d}{dt}(\underbrace{\underbrace{\frac{1}{2} m \dot{x}^{2}}_{E_{c}} + \underbrace{\frac{1}{2} k x^{2}}_{E_{p}}}_{E_{m}})=0$  

## Oscillateur harmonique électrique 
Ici on va étudier le circuit LC série. 
### Mise en équation du système 
Même équation et don même réponse.
$\frac{d^{2} i(t)}{dt^{2}}+ \omega_{0}^{2} i(t)=0$    avec  $\omega_{0}=\frac{1}{\sqrt{LC}}$ 
### Etude énergétique 
#### Obtention de l'équation caractérisant de l'énergie en électricité 
On multiplie la [[Signaux électiques dans l'ARQS#Loi des Mailles|loi de maille]] par $i(t)$ :  "$LDM \times i$" 
On obtient $P_{gen}= P_{L} + P_{R}$ 
#### Cas du générateur éteint 
$E=0$    et   $P_{gen}=0$ 
- $P_{L}(t)=-P_{c}(t)$ 
- L'énergie et directement échange entre la bobine et le condensateur. 
