#chapitre15 #electricite #mecanique #signal 
## Résonance d'intensité RLC série, vitesse
Phénomène par lequel une système susceptible d'osciller présente une amplitude de sortie particulière élevée. 
### Détermination de l'expression du courant
$\displaystyle \underline{I} = \frac{E}{R} \frac{1}{1+jQ(\frac{\omega}{\omega_0}-\frac{\omega_0}{\omega})}$ 
### Etude de l'amplitude 
$\displaystyle \frac{dI}{d \omega}(\omega_{r})=0 \Leftrightarrow \omega_{r}=\omega_{0}$ 
- On a résonance en intensité (ou vitesse) lorsqu'un système est excité à sa pulsation propre (toujours vrai pour un système linéaire du 2nd ordre).
- Du point de vue de l'amplitude, l'ensemble bobine / condensateur se comporte comme un fil. 
#### Etude expérimentale 
On cherche $\omega_{1}$ et $\omega_{2}$ solutions de $I(\omega)= \frac{I(\omega_{0})}{\sqrt{2}}$ 
- $\displaystyle Q= \frac{\omega_{0}}{\Delta \omega}$ 
### Etude du déphasage 
$\displaystyle\varphi = \arctan(Q(\frac{\omega_{0}}{\omega}- \frac{\omega}{\omega_{0}}))$ 
- $\varphi(\omega_{0})=0$ donc il n'y a pas de déphasage.
- $\underline{Z_{L-C}}=0$ 
#### Etude expérimental
On resout $\varphi(\omega)= \pm \frac{\pi}{4}$ qui donne $\omega_{1}$ et $\omega_{2}$. 

## Résonance mécanique en élongation, charge du condensateur
### Excitation sinusoïdale
$\Delta l(t)=x(t)-e(t)$              $\overrightarrow{F_{r}}=-k(x-e)\overrightarrow{e_{x}}$ 
- $\displaystyle\ddot{x}+ \frac{\omega_{0}}{Q}\dot{x}+ \omega_{0}^{2}=\omega_{0}^{2} E \cos(\omega t)$ 
- $\displaystyle \frac{\underline{X}}{\underline{E}}= \frac{1}{1-(\frac{\omega}{\omega_{0}})^{2}+j \frac{1}{Q}\frac{\omega}{\omega_{0}}}$ 
### Etude de l'amplitude
$\displaystyle X = \frac{E}{\sqrt{(1-(\frac{\omega}{\omega_{0}})^{2})^{2}+(\frac{\omega}{Q \omega_{0}})^{2}}}$ 
- Pour $\omega \to 0$ : $X \to E$
- Pour $\omega \to + \infty$ : $X \to 0$ 
- $\frac{dX}{d \omega}(\omega_{r})=0 \Leftrightarrow \omega_{r}=\omega_{0}\sqrt{1- \frac{1}{2Q^{2}}}$ 
- $X(\omega_{0})=Q$
### Etude du déphasage 
- $\varphi(0)=0$
- $\varphi(\omega_{0})= -\frac{\pi}{2}$
- $\varphi(\infty)= - \pi$ 
