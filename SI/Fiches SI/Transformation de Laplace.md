#comportement_des_systemes_analogiques
$\displaystyle X(p)=\int_{-\infty}^{+\infty}x(t)e^{-pt}dt$ 
- $p = \sigma + j \omega$ (complexe)

## Pour les fonctions causales 
- $x(t)=0$ pour $t<0$
- $\displaystyle X(p)=\int_{0}^{+\infty}x(t)e^{-pt}dt$ 

$\begin{cases} u(t)= 0 \text{  si  } t<0 \\ u(t)=1 \text{  si  } t \geq 0\end{cases}$

| $x(t)=$                                                                                                        | $X(p)$                                  |
| -------------------------------------------------------------------------------------------------------------- | --------------------------------------- |
| $\begin{align*} 0 \text{  pour  } t>\varepsilon \\ ( \varepsilon(t) \text{  impulsion de Dirac} )\end{align*}$ | $1$                                     |
| $A \cdot u(t)$                                                                                                 | $\frac{A}{p}$                           |
| $A e^{-at}t^{n}u(t)$                                                                                           | $A \frac{n!}{(p+a)^{n+1}}$              |
| $Ae^{-at}\sin(\omega t)u(t)$                                                                                   | $A \frac{\omega}{(p+a)^{2}+\omega^{2}}$ |
| $Ae^{-at}\cos(\omega t)u(t)$                                                                                   | $A \frac{p+a}{(p+a)^{2}+\omega^{2}}$    |
| $\begin{align*} f(t) \cdot u(t) \\ f(t-a)\cdot u(t-a) \end{align*}$                                            | $\begin{align*} F(p) \\ e^{-ap}F(p) \end{align*}$                                        |

| $\frac{1}{p}$                                            | constante                          |
| -------------------------------------------------------- | ---------------------------------- |
| $\frac{1}{p-\alpha_{i}}$                                 | $e^{\alpha_{i}t}$                  |
| $\frac{\omega}{(p- \alpha_{j})^{2}+\omega_{j}^{2}}$      | $e^{\alpha_{j}t}\sin(\omega_{j}t)$ |
| $\frac{p-\alpha_{j}}{(p-\alpha_{j})^{2}+\omega_{j}^{2}}$ | $e^{\alpha_{j}t}\cos(\omega_{j}t)$ |

### Linéarité
$\mathcal{L}(af_{1}(t)+bf_{2}(t))=a \mathcal{L} (f_{1}(t))+b \mathcal{L}(f_{2}(t))$ 
### Transformée de Laplace de $\displaystyle \frac{f^{k}x(t)}{dt^{k}}$
- $\displaystyle\mathcal{L}(\frac{d^{k}x(t)}{dt^{k}})=p^{k} \times X(p)$ 
- $\displaystyle\mathcal{L}(\frac{dx(t)}{dt})=pX(p)-x(0^{+})$ 
- $\displaystyle \mathcal{L}(\frac{d^{2}x(t)}{dt^{2}})=p^{2}X(p)-px(0^{+})-\frac{dx(0^{+})}{dt}$ 
### Théorème du retard 
$\mathcal{L}(f(t-t_{1}))=e^{-t_{1}p} \cdot \mathcal{L}(f(t))$ 
### Théorème de la valeur initial 
$\displaystyle \lim_{t \to 0^{+}}x(t)=\lim_{p \to + \infty}pX(p)=x(0^{+})$ 
### Théorème de la valeur finale
$\displaystyle \lim_{t \to + \infty}x(t)=\lim_{p \to 0^{+}}pX(p)=x(\infty)$  



