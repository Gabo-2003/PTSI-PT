#chapitre13 
## Etude spectral d'une signal
### Principe de Fourier
$\displaystyle s(t)=\sum_{i} s_{i}(t)=\sum_{i} A_{i} \cos(2\pi f_{i} t+ \varphi_{i})$ 
- $s_{i}$ composante spectrale
- ensemble de $f_{i}$ : spectre
### Signal périodique 
$\displaystyle s(t)=A_{0}+\sum_{n=1}^{\infty} A_{n} \cos(n \omega_{s}t + \varphi_{n})$ 
- $A_{0}$ est égal a la moyenne.
- à $n=1$ : même fréquence que $s(t)$, fréquence fondamental
- à $n\geq 2$ : harmonique de rang $n$. 
- Si le signal est symétrique en monté et en descente, les termes $n$ pair sont nulles.
- Plus la fonction périodique a des domaines de variation rapides et plus les termes d'ordre élevés sont présents. 
#### Moyenne 
$\displaystyle<s(t)> = \frac{1}{T_{s}} \int_{1 \text{  période}} s(t)dt$  
#### Valeur efficace 
Grandeur continue donnant le même effet Joule moyen que la grandeur. 
$\displaystyle <s(t)>= \frac{1}{T}$
##### Signal périodique : 
$S_{eff}=\sqrt{<s^{2}(t)>}$ 
##### Signal harmonique : 
$S_{eff}=\frac{S}{\sqrt{2}}$ 
##### Théorème de Parceval
L'énergie transportée par un signal périodique est égal à l'énergie transportées par ses harmoniques.  
$\displaystyle S^{2}_{eff}= S_{0}^{2} + \sum_{n=1}^{+ \infty}s_{n,eff}^{2}$ 

## Régime sinusoïdal forcé
### Système excité par une entrée sinusoïdal 
$\displaystyle \dot{s}(t)+ \frac{1}{\tau}s(t)= k \cos(\omega t + \varphi_{e})$ 
$\displaystyle \ddot{s}(t) + 2 \xi \omega_{0} \dot{s}(t) + \omega_{0}^{2}s(t)= k \cos(\omega t + \varphi_{e})$ 
#### Réponse 
$s(t)=S \cos(\omega t + \varphi)$
### Notation complexe
$Re(\underline{x}(t))= x(t)$
- $\displaystyle \underline{x}(t)=X e^{j(\omega t + \varphi)}$          et          $\underline{X}=X e^{j\varphi}$
- $\underline{x}(t)= \underline{X}e^{j \omega t}$ 
- $X = |\underline{x}(t)|=|\underline{X}|$                       $\varphi = \arg(\underline{X})$ 
#### Dérivation 
$\underline{\dot{x}}(t)=j \omega \underline{x}$ 
#### Intégration 
$\displaystyle \int\underline{x}(t)= \frac{1}{j \omega} \underline{x}$ 
#### Déphasage 
$\varphi_{y / x} = \varphi_{y}-\varphi_{x}$ 
- $\displaystyle \varphi_{y / x} = \arg\left(\frac{\underline{Y}}{\underline{X}}\right)$                     $\displaystyle\varphi_{y / x} = \arg\left(\frac{\underline{y}(t)}{\underline{x}(t)}\right)$  

## Impédance complexe 
- $i(t)= I \cos(\omega t + \varphi_{i})$               $\underline{i}(t)=I e^{j(\omega t + \varphi_{i})}$ 
- $u(t)= U \cos(\omega t + \phi_{u})$             $\underline{u}(t)=U e^{j(\omega t + \phi_{u})}$ 
- $\underline{u}(t)=\underline{Z} \times i(t)$ 
- $\underline{Z_{R}}=R$              $\displaystyle \underline{Z_{C}}= \frac{1}{jC \omega}$             $\underline{Z_{L}}=jL \omega$ 
### En série
$\displaystyle \underline{Z_{eq}}=\sum_{k=1}^{N}\underline{Z_{k}}$              $\underline{Z_{eq}}= \underline{Z_{1}} + \underline{Z_{2}}$ 
### Parallèle 
$\displaystyle\frac{1}{\underline{Z_{eq}}} = \sum_{k=1}^{N} \frac{1}{\underline{Z_{k}}}$                             $\displaystyle\frac{1}{\underline{Z_{eq}}} = \frac{1}{\underline{Z_{1}}} + \frac{1}{\underline{Z_{2}}}$ 
### Ponts diviseurs
- En série : $\displaystyle\underline{u_{1}}= \underline{U} \times \frac{\underline{Z_{1}}}{\underline{Z_{eq}}}$ 
- En parallèle : $\displaystyle\underline{i_{1}}= \underline{i} \times \frac{\underline{Z_{1}}}{\underline{Z_{1}} + \underline{Z_{2}}}$ 