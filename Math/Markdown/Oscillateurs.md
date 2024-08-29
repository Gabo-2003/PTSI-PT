---
tags:
  - electronique
---
## Principe générale 
On utilise un système linéaire bouclé. Avec un amplificateur de gain ($G>0$) et un [[Filtrage#Passe-bande|filtre passe bande d'ordre 2]]. 
![[image oscillateur.png|400]]

On a donc $\displaystyle G = \frac{\underline{u_{s}} }{\underline{u_{e}} }$  et   $\displaystyle \underline{H} = \frac{\underline{u_{e}} }{\underline{u_{s}} }$ 
D'où $\displaystyle \underline{H}  = \frac{\underline{u_{e}} }{\underline{u_{s}} } = \frac{\epsilon H_{0}}{1+jQ \left( \frac{\omega }{\omega _{0}} - \frac{\omega _{0}}{\omega } \right) } = \frac{1}{G}$
### Équation différentielle de l'oscillateur et condition d'oscillation 
En mettant l'équation précédente en forme de ED, on trouve :
$\displaystyle u_{e} + \frac{1}{Q \omega_{0}} \dot{u_{e}} + \frac{1}{\omega_{0}^{2}} \ddot{u_{e}}  = \frac{\epsilon H_{0}}{Q \omega_{0}}\dot{u_{s}}$  et  $u_{s} G = u_{e}$  donc on a :
$\displaystyle \ddot{u_{e}} + \frac{\omega _{0}}{Q}(1-\epsilon H_{0}G)\dot{u_{e}} + \omega _{0}^{2} u_{e}=0$
#### Condition de stabilité
On a stabilité $\Leftrightarrow 1-\epsilon H_{0}G>0 \implies 1>\epsilon H G$
#### Condition de oscillation
Cas limite : $\epsilon H_{0}G = 1$
- On trouve un oscillateur harmonique 
### Condition obtenues en utilisant les complexes
On sort de la forme de fraction et en prenant la partie réel et imaginaire de l'équation on trouve : 
$\omega = \omega _{0}$   et   $1 = \epsilon H_{0} G$ 