#calcul

## Première ordre : $u(t)y'(t)+v(t)y(t)+w(t)=0$ 
### 1èr étape : 
On normalise l'équation.
$\begin{equation*} \tag{E} \bullet \quad y'(t)+a(t)y(t)=b(t) \end{equation*}$ 
$\begin{equation*} \tag{H} \bullet \quad y'(t)+a(t)y(t)= 0\end{equation*}$ Solutions : $\boxed{y_{h}: t \longmapsto C e^{-A(t)}}$        Avec $A$ une primitive de $a$
### Problème de Cauchy 
$\begin{cases} y'(t)+a(t)y(t)=b(t) \\ y(t_{0})=y_{0} \end{cases}$
Solution unique : $\boxed{y_{c}: \mathbb{R} \longrightarrow \mathbb{C}: t \longmapsto y_{0} e^{-A(t)+A(t_{0})}}$ 
### 2èm étape :
- Si $b(t)$ est un polynôme : $y_{p}(t) = \alpha t^{2}+\beta t + \gamma$ 
- Si $b(t)=e^{mt}$:                    $y_{p}(t)=\alpha e^{mt}$ 
- Si $b(t)=P(t)e^{mt}$ :            $y_{p}(t)= Q(t) e^{mt}$   avec $P(t)$ et $Q(t)$ polynômes
- Si $b(t)= \alpha_{1}\cos(\beta t ) + \alpha_{2}\sin(\beta t )$ :  $y_{p}(t) = A \cos(\beta t) + B \sin(\beta t )$ 
#### Principe de superposition 
Si $b(t)=b_{1}(t) + b_{2}(t)$ : 
On pose $y'_{1} +a(t)y_{1}=b_{1}$    et    $y'_{2} +a(t)y_{2}=b_{2}$ 
On a donc  $y_{p}(t)=y_{1}(t) + y_{2}(t)$ 
#### Equations a valeur complexe
On a $b(t)=b_{1}(t) + ib_{2}(t)$ :       $y(t)=y_{1}(t)+i y_{2}(t)$ 
#### Variation de la constante 
$y(t)=C(t) e^{-A(t)}$ 
### Equation complète 
$y(t)=y_{h}(t) + y_{p}(t)$ 

## Second Ordre : $ay''(t)+by'(t)+cy(t)=d(t)$
### Solution homogène 
$\begin{equation*} \tag{H}  ay''(t)+by'(t)+cy(t)=0 \end{equation*}$
- Equation caractéristique : 
$\begin{equation*} \tag{K}  ar^{2}+br + c =0 \end{equation*}$
- Si $\Delta > 0$ :                        $y_{h}(t)=C_{1}e^{r_{1}t}+C_{2}e^{r_{2}t}$
- Si $\Delta < 0$, $r_{1}= \alpha+i \beta$ :    $y_{h}(t)=e^{\alpha t }(C_{1}\cos(\beta t) + C_{2} \sin(\beta t))$ 
- Si $\Delta = 0$ :                        $y_{h}(t)=(C_{1}t+C_{2})e^{r_{1}t}$ 
### Solution particulière 
#### De la forme $d(t)=A e^{\lambda t}$
- Si $\lambda$ pas de racine :     $y_{p}(t)= \gamma e^{\lambda t}$ 
- Si $\lambda$ racine simple :     $y_{p}(t)= \gamma t e^{\lambda t}$ 
- Si $\lambda$ racine double :    $y_{p}(t)= \gamma t^{2} e^{\lambda t}$ 
#### De la forme $d(t)=B \cos(\omega t ) \text{  ou  } B \sin(\omega t )$ 
- Si $i \omega$ pas de racine :   $y_{p}(t)=\gamma \cos(\omega t )+ \delta \sin(\omega t)$
- Si $i \omega$ est racine :         $y_{p}(t)=\gamma t \cos(\omega t )+ \delta t \sin(\omega t)$
