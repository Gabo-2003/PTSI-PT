#chapitre11 #electricite #signal  
## Etude d'un circuit RLC Série 
### Obtention
$\displaystyle \frac{d^{2}u_{c}^{2}}{dt^{2}}+ \frac{R}{L} \frac{du_{c}}{dt}+ \frac{1}{LC} u_{c}= \frac{e(t)}{LC}$ 
#### Formes canoniques 
$\displaystyle \frac{d^{2}u_{c}^{2}}{dt^{2}}+ \frac{\omega_{0}}{Q} \frac{du_{c}}{dt}+ \omega_{0}^{2} u_{c}= 0$  
$\displaystyle \frac{d^{2}u_{c}^{2}}{dt^{2}}+ 2\xi \omega_{0} \frac{du_{c}}{dt}+ \omega_{0}^{2} u_{c}= 0$   
- Pulsation propre : $\omega_{0}=\frac{1}{\sqrt{LC}}$ en $rad/s$ 
- Facteur de qualité : $Q=\frac{1}{R} \sqrt{\frac{L}{C}}$ 
- Amortissement : $\xi = \frac{R}{2} \sqrt{\frac{C}{L}}= \frac{1}{2Q}$ 
### Résolution 
Résolution d'une [[Equations différentielles linéaires#Second Ordre $ay''(t)+by'(t)+cy(t)=d(t)$|équation différentielle d'ordre 2]].
#### Régime pseudopériodique 

| $\Delta<0$ | $Q>\frac{1}{2}$ | $\xi<1$ |
| ---------- | --------------- | ------- |
- $\omega=\omega_{0} \sqrt{1- \frac{1}{4Q^{2}}}=\omega_{0}\sqrt{1-\xi^{2}}$ 
- $\displaystyle u_{c,h}(t)=A \underbrace{e^{-\frac{\omega_{0}t}{2Q}}}_{*}\cos(\omega t+ \varphi)$        * amortissement de l'amplitude
#### Régime apériodique 

| $\Delta>0$ | $Q<\frac{1}{2}$ | $\xi>1$ |
| ---------- | --------------- | ------- |
- $\begin{cases} \omega_{1}=-\omega_{0}\left(\frac{1}{2Q}+ \sqrt{\frac{1}{4Q^{2}}-1}\right) \\ \omega_{2}=-\omega_{0}\left(\frac{1}{2Q}- \sqrt{\frac{1}{4Q^{2}}-1}\right) \end{cases}$ 
- $u_{c,h}(t)=A e^{-\omega_{1} t} +B e^{-\omega_{2} t}$ 
#### Régime critique 

| $\Delta=0$ | $Q=\frac{1}{2}$ | $\xi=1$ |
| ---------- | --------------- | ------- |
- $u_{c,h}(t)=(At+B)e^{- \omega_{0} t}$ 
#### Conditions initiales 
Quel que soit le régime, il faut déterminer 2 constantes.
##### Continuité de la tension aux bornes d'un condensateur 
$u_{c}(0^{+})=u_{c}(0^{-})$ 
##### Continuité du courante dans une bobine 
$i_{L}(0^{+})=i_{L}(0^{-})$ 
$\displaystyle \frac{d u_{c}}{dt}(0^{+})= \frac{1}{C} i(0^{+})=\frac{1}{C} i(0^{-})=0$ 