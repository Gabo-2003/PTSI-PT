#chapitre15 #electricite 
$\displaystyle \underline{H}(\omega)= \frac{\underline{s}}{\underline{e}}$            $G(\omega)=|\underline{H}(\omega)|$         $\varphi(\omega)= \arg(\underline{H}(\omega))$  
## Diagramme de Bode (cas filtre RC, sortie sur le condensateur) 
$\displaystyle \underline{H}(\omega)= \frac{1}{1+ j \frac{\omega}{\omega_{0}}}$     $G(\omega)= \frac{1}{\sqrt{1+ (\frac{\omega}{\omega_{0}})^{2}}}$      $\displaystyle\varphi(\omega)= -\arctan\left(\frac{\omega}{\omega_{0}}\right)$   
- $G_dB(\omega)= -10 \log(1+(\frac{\omega}{\omega_{0}})^{2})$ 
### Gain 
C'est le rapport des amplitudes en tension entre sortie et entrée.
- $\omega \to 0$ : $\displaystyle\lim_{\omega \to 0} G_{dB}(\omega)=0$  asymptote horizontale
- $\omega \to + \infty$ : $G_{dB}(\omega) \approx -20 \log(\frac{\omega}{\omega_{0}})$ pente de $-20 dB/deca$
- $\omega = \omega_{0}$ : $G_{dB}(\omega_{0})=-10\log(2) \approx -3dB$ 
### Phase
C'est l'avance du signal de sortie sur celui d'entrée. 
- $\omega \to 0$ : $\displaystyle\lim_{\omega \to 0} \varphi(\omega) =0$  
- $\omega \to + \infty$ : $\displaystyle\lim_{\omega \to + \infty} \varphi(\omega) =- \frac{\pi}{2}$   
- $\omega = \omega_{0}$ : $\varphi(\omega_{0})=- \frac{\pi}{4}$ 

## Diagramme de Gabarit
![[image diagramme gabarit.png|400]]
### Bande passante
$G_{dB}>G_{min}$  ,   $[f_{p1}, f_{p2}]$ 
### Bande atténue
$G_{dB}<G_{min}$  ,   $[0, f_{p1}]$ et $[f_{p2}, + \infty]$ 

## Diagramme de Bode 
### Pulsation coupure 
C'est la pulsation pour laquelle le gain est égal au gain maximal diminué de $3dB$ 
- Il peut avoir plusieurs pulsations de coupure.
- $\displaystyle |H(\omega_{c}|= \frac{G_{max}}{\sqrt{2}}$           
- $\omega_{c}=\omega_{0}$  pour ordre 1
### Passage de fonction de transfert à équation différentielle 
$\displaystyle \underline{H}(j \omega)= \frac{P_{e}(j \omega)}{P_{s}(j \omega)} = \frac{\underline{u_{s}}}{\underline{u_{e}}}$
donc $\underline{u_{s}}P_{s}(j \omega)=\underline{u_{e}}P_{e}(j \omega)$
### Stabilité d'un montage 
Pour qu'une équation différentielle d'ordre un ou deux décrive un système stable (qui revienne à l'équilibre si on le perturbe momentanément), il faut que les signes des différentes termes de l'équation soient identiques.  

## Filtres d'ordre 1
### Passe-bas
Coupe les hautes fréquences.
- $\displaystyle \underline{H}(\omega)= \frac{G_{0}}{1+j \frac{\omega}{\omega_{0}}}$  pente de $-20 dB/deca$ 
### Passe-haut
Coupe les bas fréquences.
- $\displaystyle \underline{H}(\omega)= \frac{G_{0}}{1-j \frac{\omega_{0}}{\omega}}$  pente de $20 dB/deca$ 
### Filtre  dérivateur 
En complexe, dériver revient à multiplier par $j \omega$ 
- $\displaystyle \underline{H}(j \omega)= j \omega$ 
- Possède une phase constante $\varphi = \frac{\pi}{2}$ et pente de $+20 dB / deca$ 
- Ce filtre amplifie le bruit à haut fréquences il faut donc l'utiliser que pour un domaine spécifique de fréquences.
### Filtre intégrateur
En complexe, intégrer revient à multiplier par $\displaystyle \frac{1}{j \omega}$ 
- $\displaystyle \underline{H}(j \omega)= \frac{1}{j \omega}$
- Possède une phase constante $\varphi = - \frac{\pi}{2}$ et pente de $-20 dB / deca$
- Ce filtre amplifie le bruit en basse fréquences il faut donc l'utiliser que pour un domaine spécifique de fréquences.
### Déphaseur 
Permet de déphaser les signaux sans les atténuer ou les amplifier.
- $\displaystyle \underline{H}(j \omega) =H_{0} \frac{1- j \frac{\omega}{\omega_{0}}}{1+j \frac{\omega}{\omega_{0}}}$
- Gain : $G=H_{0}$ 
- Déphasage : $\displaystyle \varphi = -2 \arctan\left(\frac{\omega}{\omega_{0}}\right)$  
## Filtres d'ordre 2
### Passe-bas
$\displaystyle\underline{H}(\omega)= \frac{G_{0}}{1-(\frac{\omega}{\omega_{0}})^{2}+j \frac{1}{Q} \frac{\omega}{\omega_{0}}}$   pente $-40 dB / deca$ 
- Résonance si $Q > \frac{1}{\sqrt{2}}$. 
- #### En basse fréquence
On est en basse fréquence pour $\omega << \omega_{0}$
- $\displaystyle \underline{H} = \frac{-jQ \frac{\omega_{0}}{\omega}}{1+jQ(\frac{\omega}{\omega_{0}})} \approx 1$ 
#### En haut fréquence
On est en haut fréquence pour $\omega >> \omega_{0}$
- $\displaystyle \underline{H} =- \frac{\omega_{0}^{2}}{ \omega^{2}}$ 
#### Détermination de la résonance 
On cherche quand le dénominateur du gain est minimum.
### Passe-bande
$\displaystyle\underline{H}(\omega)= G_{0} \frac{j \frac{1}{Q} \frac{\omega}{\omega_{0}}}{1-(\frac{\omega}{\omega_{0}})^{2}+j \frac{1}{Q} \frac{\omega}{\omega_{0}}} = \frac{G_{0}}{1+jQ(\frac{\omega}{\omega_{0}} - \frac{\omega_{0}}{\omega})}$    
- pente $\pm 20 dB / deca$ 
- $Q$  traduit l'acuité de la résonance.
#### En basse fréquence
On est en basse fréquence pour $\omega << \omega_{0}$
- $\displaystyle \underline{H} = \frac{j \omega}{Q \omega_{0}}$
#### En haut fréquence
On est en haut fréquence pour $\omega >> \omega_{0}$
- $\displaystyle \underline{H} =\frac{1}{Q} \frac{\omega_{0}}{j \omega}$ 
#### Pulsation de coupure 
Gain maximum :   $\displaystyle 1+Q^{2}(\frac{\omega}{\omega_{0}}- \frac{\omega_{0}}{\omega})=0$ 
$\displaystyle |H(\omega_{c}|= \frac{G_{max}}{\sqrt{2}}$
## Comportement bobine et condensateur aux limites
$$\underline{Z_{c}}= \frac{1}{jC \omega} \text{  alors  } \begin{cases} \text{si  } \omega \to 0 \text{  alors  } |\underline{Z_{c}}|= + \infty \text{  (int ouverte)} \\ \text{si  } \omega \to + \infty \text{  alors  } |\underline{Z_{c}}|= 0 \text{  (fil)} \end{cases}$$
$$\underline{Z_{L}}= jL \omega \text{  alors  } \begin{cases} \text{si  } \omega \to 0 \text{  alors  } |\underline{Z_{L}}|= 0\text{  (fil)} \\ \text{si  } \omega \to + \infty \text{  alors  } |\underline{Z_{L}}|= + \infty \text{  (int ouverte)} \end{cases}$$



