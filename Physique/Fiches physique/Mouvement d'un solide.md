#chapitre23 #mecanique #dynamique 
## Dynamique d'un solide indéformable en rotation 
### Moment cinétique d'un système de points
Point : $\displaystyle \overrightarrow{\mathcal{L}_{O}}(\sigma)= \sum_{k=1}^{N} \overrightarrow{\mathcal{L}_{O}}(M_{k})$  
Axe : $\displaystyle \mathcal{L}_{\Delta}(\sigma)= \sum \mathcal{L}_{\Delta,k}$ 
### Moment d'inertie 
$\mathcal{L}_{\Delta}(\sigma)=J_{\Delta}\,\dot{\theta}$ 
- $\displaystyle J_{\Delta}=\sum_{k=1}^{N} m_{k}\,r_{k}^{2}$ 
### Théorème scalaire du moment cinétique 
[[Théorème du moment cinétique#Théorème du moment cinétique par rapport à un point|TMC]]
- $\displaystyle J_{\Delta} \ddot{\theta}=\sum_{F_{ext}} M_{\Delta}(\overrightarrow{F_{ext}})$ 

## Couple 
Tout ensemble de forces qui se compensent mais dont les moments ne se compensent pas. 
- $\overrightarrow{\Gamma}$ ne dépende pas du point.

## Pendule pesant
$\ddot{\theta}= -\frac{mg}{J_{z}} l \sin(\theta)$ 
- On obtient l'intégrale première du mouvement en multipliant par $\theta$  :  $\displaystyle J_{z} \frac{\dot{\theta^{2}}}{2} - mgl \cos(\theta) =cst$ 

## Etude énergétique 
$E_{c}= \frac{1}{2} J_{z} \dot{\theta ^{2}} \quad\longleftrightarrow\quad  E_{c}=\frac{1}{2}mv^{2}$ 
### Puissance d'une force 
$\mathcal{P}(f)= r_{k}\,f_{\theta}\,\dot{\theta}=\dot{\theta}M_{z}(\overrightarrow{f})$ 
### Travail 
$\delta W (\overrightarrow{f})=M_{z}(\overrightarrow{f})\, d \theta$  
- $\displaystyle W_{\theta_{k,i}\to\theta_{k,f}}(\overrightarrow{f})= \int_{\theta_{k,i}}^{\theta_{k,f}} M_{z}(\overrightarrow{f}) \, d \theta$ 
### Théorème de la puissance  cinétique
$\displaystyle \sum_{i}^{} \mathcal{P}(\overrightarrow{f_{ext}})= \frac{d E_{c}}{dt}$ 
### Théorème de l'énergie cinétique 
$\Delta E_{c}= \sum W_{\theta_{k,i}\to\theta_{k,f}}(\overrightarrow{f_{i}})$ 
- $\Delta E_{c}=\Gamma \Delta \theta$ 
- $\Gamma = J_{z} \dot{\omega}$ 
### Cas du solide indéformable
$\displaystyle \frac{d E_{c}}{dt}= \sum_{}^{} P(\overrightarrow{f_{ext}}) + \sum_{}^{}P(\overrightarrow{f_{int}})$  