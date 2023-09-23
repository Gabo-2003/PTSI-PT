#chapitre3 #signal
## Echelon de tension 
$e(t)= \begin{cases} 0 \text{  si  }t<0  \\ E \text{  si  }t>0 \end{cases}$ 
### Réponse indicielle et régime libre 
#### Entre : 
Grandeur qu'on commande.  
#### Sortie : 
Grandeur qu'on mesure.
#### Réponse indicielle :
Evolution temporelle de la sortie lorsque l'entrée est un échelon.
#### Régime libre :
C'est l'évolution lorsque l'entrée est nulle.

## Circuit R-C Série 
![[image circuit rc.png|350]]
Entre : tension $e(t)$, GBF source de tension idéal
Sortie : tension $u_c(t)$
### Etablissement de l'équation différentielle 
Loi de mailles : $e(t)= u_{R}+u_{c}$ 
Loi d'Ohm : $U=R i(t)$
Condensateur :  $i(t)=c \frac{du(t)}{dt}$ 
$\begin{align*} & \quad \; e(t) = u_{R}+u_{c} \\ &\Leftrightarrow e(t) =Ri(t)+u_{c} \\ &\Leftrightarrow e(t) =RC \frac{du_{c}}{dt} +u_{c} \\ &\Leftrightarrow \frac{d u_{c}(t)}{dt} + \frac{u_{c}(t)}{RC} = \frac{e(t)}{RC} \end{align*}$
Soit $\tau = RC$
$\boxed{\frac{d u_{c}(t)}{dt}+ \frac{u_{c}}{\tau} = \frac{E}{\tau}}$ 
### Résolution de l'équation différentielle 
 $\boxed{\text{On a toujours continuité de la tension aux bornes d'un condensateur.}}$
 $\displaystyle u_{c}(t)=E(1-e^{-\frac{t}{\tau}})$ 
### Régime transitoires et permanents 
![[image Graphe RC.jpg]]
#### Régime permanent 
La sortie est constante. Correspond a la solution de particulière de l'équation différentielle associée au système.   
#### Régime Transitoire 
La sortie évolue de l'état initial vers le régime permanent. Il correspond a la solution de l'équation homogène.
#### Temps de réponse
- Pente à l'origine : $\displaystyle \frac{d u_{c}(0)}{dt}= \frac{E}{\tau}$ 
- $u_{c}(\tau)=0,63 E$ 
- 5% : $t=3 \tau$ 
- régime permanent : $5 \tau$ 
### Aspect énergétique 
$E_{R}= \frac{C E^{2}}{2}$
$E_{gen}= C E^{2}$ 
$P_{gen}(t) = P_{R}(t)+ P_{C}(t)$ 
### Régime libre 
On s'intéresse aux circuit lorsque l'on cesse tout activité extérieur.
- $e(t) = \begin{cases} E \text{  si   } t<0  \\ 0 \text{  si   } t>0 \end{cases}$ 
- $\displaystyle \frac{d u_{c}}{dt}+ \frac{u_{c}}{\tau}=0$ 
- $u_{c}(t)= E e^{-\frac{t}{\tau}}$ 
#### Temps de réponse
- Pente a l'origine : $\frac{d u_{c}(0)}{dt}=- \frac{E}{\tau}$ 
- $u_{c}(\tau)=0,37 \tau$
- $u_{c}(t)=0,01 E \Rightarrow t=4,6 \tau \approx 5 \tau$ 

## Etude du circuit RL série 
![[image circuit rl.png|350]]
Entre : tension $e(t)$, GBF source de tension idéal
Sortie : intensité $i(t)$
### Equation différentielle
$\displaystyle \frac{d i(t)}{dt}+ \frac{1}{\tau}i(t)= \frac{1}{\tau} \frac{e(t)}{R}$ 
Avec $\displaystyle \tau = \frac{L}{R}$ 
### Réponse indicielle
$\boxed{\text{Le courant traversant une bobine est toujours continue.}}$
$\displaystyle i(t)= \frac{E}{R}(1- e^{\frac{t}{\tau}})$
### Régime libre
$\displaystyle i(t)= \frac{E}{R} e^{-\frac{t}{\tau}}$ 