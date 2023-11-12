#comportement_des_systemes_analogiques 
On va étudier des entrées de type $\displaystyle e(t)=e_{0} \sin(\omega t ), \quad E(p)= \frac{e_{0} \omega}{p^{2}+\omega^{2}}$ 
- $A(\omega)=| H(j \omega) |$ 
- $A_{db}(\omega)=20 \log|H(j \omega)|$ 
## Diagramme de Bode 1èr ordre 
$\displaystyle H(p)= \frac{k}{1+ \tau p}$      $\displaystyle \omega_{c}=\frac{1}{\tau}$
### Diagramme de gain
$\displaystyle A_{dB}=20 \log(\frac{k}{\sqrt{1+T^{2}\omega^{2}}})$ 
- Si $\omega \rightarrow 0$  alors  $T^{2}\omega^{2}<< 1$  Donc  $A_{dB} \approx 20 \log k$  
- Si $\omega \rightarrow + \infty$  alors  $T^{2}\omega^{2} >> 1$  Donc  $A_{dB} \approx 20 \log k - 20 \log(T \omega)$ 
$\quad \quad \bullet$  Pente $-20 dB/décade$ 
- Intersection des deux asymptotes : $\displaystyle \omega_{c}= \frac{1}{T}$ 
### Diagramme de phase 
$\varphi = \arctan(-T \omega)$ en degrés 
- Si $\omega \rightarrow 0$  alors  $\varphi \rightarrow 1$ 
- Si $\omega \rightarrow + \infty$  alors  $\varphi \rightarrow -90°$ 
- à $\omega_{c}$ on a $\varphi = -45°$ 
![[image diagrame bode 1.png]]

## Diagramme de Bode 2èm ordre 
$\displaystyle H(p)=\frac{k}{1+ \frac{2 \xi}{\omega_{0}}p+ \frac{p^{2}}{\omega_{2}}}$ 
### Cas où $\xi>1$ 
$\displaystyle H(p)= \frac{k}{(1+T_{1}p)(1+T_{2}p)}$ 
- 3 fonctions de transfert : constante, $-20dB/déca$, $-40dB/déca$. 
![[image diagrame de bode 21.png]]
### Cas où $\xi =1$ 
$\displaystyle H(p)= \frac{k}{(1+T_{0}p)^{2}}$ 
- 2 fonctions de transfert : constante, $-40dB/déca$.
![[image diagrame bode 22.png]]
### Cas où $\xi<1$
$\displaystyle A_{dB}=20 \log \left(\frac{k}{\sqrt{(1- \frac{\omega^{2}}{\omega_{0}^{2}})^{2}+(2 \frac{\omega \xi}{\omega_{0}})^{2}}}\right)$  
- Présence d'un maximum 
- $\omega_{r}= \omega_{0} \sqrt{1-2\xi^{2}}$ il faut que $\displaystyle \xi< \frac{1}{\sqrt{2}} \approx 0,7$ 
- $\displaystyle A_{dBmaxi}=20 \log \left( \frac{k}{2 \xi \sqrt{1-\xi^{2} }}\right)$  