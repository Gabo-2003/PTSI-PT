---
tags:
  - electronique
---
## Numériser un signal électrique 
$T_{a}$ : temps d'acquisition.  
$T_{e}$ : temps d'échantillonnage. 
$\displaystyle F_{e} = \frac{1}{T_{e}}$ : fréquence d'échantillonnage.
$n$ : nombre de points pris 
 $\Delta S$ : pas de la signal
 $N$ : nombre de bits utilisées 
Nombre de points possibles en verticale :  $\displaystyle \frac{S_{max} - S_{min}}{\Delta S} = 2^{n}$ 

![[image numérisation.png|300]]
## Critère de Nyquist - Shannon
Pour éviter les phénomènes de repliement de spectre pour un signal portant une fréquence $f$, il faut échantillonner à une fréquence $f_{e}$ telle que :
$\displaystyle f_{e} > 2 f$    et    $2T_{e} < T$
- Cet critère doit être appliqué à la plus haute fréquence que l'on veut représenter. 
