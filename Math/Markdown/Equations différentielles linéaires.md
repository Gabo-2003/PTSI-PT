## Equations différentielles linéaires scalaires du première ordre  
### Théorème de Cauchy
Soit  l'équation :
$\begin{equation*} \tag{E} \quad y'(t)+a(t)y(t)=b(t) \end{equation*}$
Soit $a$ et $b$ deux fonctions continues d'un intervalle $I \subset \mathbb{K}$. Si $(t_{0}, y_{0}) \in I \times \mathbb{K}$, 
alors il existe une unique solution $f$ définie sur  $I$ au problème de Cauchy :
$\displaystyle  \begin{cases} y' + a(t) = b(t)  \\ y(t_{0}) = y_{0} \end{cases}$
### 1èr étape : Solution à l'équation homogène
On normalise l'équation $(E)$ : 
$\begin{equation*} \tag{H} \quad y'(t)+a(t)y(t)= 0\end{equation*}$ Solutions sur $I$ : $\boxed{y_{h}: t \longmapsto C e^{-A(t)}}$        
Avec $C \in \mathbb{K}$  et $A$ une primitive de $a$ sur $I$. 
### 2èm étape : Solution particulière
- Si $b(t)$ est un polynôme : $y_{p}(t) = \alpha t^{2}+\beta t + \gamma$ 
- Si $b(t)=e^{mt}$:                    $y_{p}(t)=\alpha e^{mt}$ 
- Si $b(t)=P(t)e^{mt}$ :            $y_{p}(t)= Q(t) e^{mt}$   avec $P(t)$ et $Q(t)$ polynômes
- Si $b(t)= \alpha_{1}\cos(\beta t ) + \alpha_{2}\sin(\beta t )$ :  $y_{p}(t) = A \cos(\beta t) + B \sin(\beta t )$ 
#### Principe de superposition 
Tout combinaison linéaires de solutions est une solution :
Si $b(t)=b_{1}(t) + b_{2}(t)$ : 
On pose $y'_{1} +a(t)y_{1}=b_{1}$    et    $y'_{2} +a(t)y_{2}=b_{2}$ 
On a donc  $y_{p}(t)=y_{1}(t) + y_{2}(t)$ 
#### Equations a valeur complexe
On a $b(t)=b_{1}(t) + ib_{2}(t)$ :       $y(t)=y_{1}(t)+i y_{2}(t)$ 
#### Variation de la constante 
$y(t)=C(t) e^{-A(t)}$ 
Avec $C$ une fonction dérivable sur $I$.
### Théorème de structure
L'ensemble des solutions est l'ensemble des fonctions :
$t \longmapsto y_{h}(t) + y_{p}(t)$ 

## Equations différentielles linéaires scalaires du second ordre
### Coefficients continus
$\forall t \in I$ et avec $a,b,c$ fonctions continues de  $I$ dans  $\mathbb{K}$.
$y'' + a(t) y'(t) + b(t) y = c(t) \quad (E)$ 
- Si $f$ est solution, alors $f$ est $C^{2}$ sur $I$.
### Théorème de Cauchy pour une EDL d'ordre 2
Soit l'équation $\begin{equation*} \tag{E} \quad y''(t)+a(t)y'(t)+ b(t)y = c(t) \end{equation*}$
Soit  $a,b,c$ fonctions continues de  $I$ dans $\mathbb{K}$.
Si $(t_{0}, y_{0}, y_{1}) \in I \times \mathbb{K} \times \mathbb{K}$, alors il existe une unique solution $f$ définie sur $I$ au problème de Cauchy :
$\begin{cases} y''+a(t)y' + b(t)y = c(t) \\ y(t_{0}) = y_{0} \\ y'(t_{0}) = y_{1} \end{cases}$
### Théorème de structure
L'ensemble $S_{0}$ des solutions de l'équation $(H)$ est un $\mathbb{K}.e.v$ de dimension $2$.
S'il existe une solution particulière de $(E)$, alors l'ensemble de solutions de $(E)$ est :
$S = \{ f_{p} + f_{h} \setminus f_{h} \in S_{0} \} = f_{p} + S_{0}$ 
### Méthode de Lagrange
On suppose qu'on connait une solution $y_{0}$ de $(H)$.
On peut chercher une solution de $(H)$ ou de $(E)$  sous la forme : $f = \lambda (t) y_{0}$ avec $\lambda$ fonction deux fois dérivable.
$\begin{cases} f = \lambda (t) y_{0} \\f' = \lambda'(t) y_{0} + \lambda (t) y'_{0} \\ f'' = \lambda ''(t) y_{0} + 2 \lambda'(t) y'_{0} + \lambda (t)y''_{0} \end{cases}$
On injecte dans $(E)$ et on obtient une équation différentielle linéaire du premier ordre en $\lambda '$ que l'on résout. 
### Cas à coefficients constants
$\begin{equation*} \tag{E} ay''(t)+by'(t)+cy(t)=d(t) \end{equation*}$
#### Solution homogène 
$\begin{equation*} \tag{H}  ay''(t)+by'(t)+cy(t)=0 \end{equation*}$
- Equation caractéristique : 
$\begin{equation*} \tag{K}  ar^{2}+br + c =0 \end{equation*}$
- Si $\Delta > 0$ :                        $y_{h}(t)=C_{1}e^{r_{1}t}+C_{2}e^{r_{2}t}$
- Si $\Delta < 0$, $r_{1}= \alpha+i \beta$ :    $y_{h}(t)=e^{\alpha t }(C_{1}\cos(\beta t) + C_{2} \sin(\beta t))$ 
- Si $\Delta = 0$ :                        $y_{h}(t)=(C_{1}t+C_{2})e^{r_{1}t}$ 
#### Solution particulière 
##### De la forme $d(t)=A e^{\lambda t}$
- Si $\lambda$ pas de racine :     $y_{p}(t)= \gamma e^{\lambda t}$ 
- Si $\lambda$ racine simple :     $y_{p}(t)= \gamma t e^{\lambda t}$ 
- Si $\lambda$ racine double :    $y_{p}(t)= \gamma t^{2} e^{\lambda t}$ 
##### De la forme $d(t)=B \cos(\omega t ) \text{  ou  } B \sin(\omega t )$ 
- Si $i \omega$ pas de racine :   $y_{p}(t)=\gamma \cos(\omega t )+ \delta \sin(\omega t)$
- Si $i \omega$ est racine :         $y_{p}(t)=\gamma t \cos(\omega t )+ \delta t \sin(\omega t)$
##### Cas générale
On peut utiliser le méthode de Lagrange. 
### Cas à coefficients non constants 
On cherche
- Une solution évidente.
- Une solution polynomiale.
- Une solution de forme particulière. 
- Une solution par changement de variable.
- Une solution par changement de fonction inconnue.
- Une solution développable en série entière.
Après, on utilise le méthode de Lagrange.
#### Recherche de solutions développables en série entière