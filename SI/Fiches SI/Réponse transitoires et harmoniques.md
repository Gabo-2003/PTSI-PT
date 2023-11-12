#comportement_des_systemes_analogiques
## Réponses du première ordre 
- $\displaystyle a \frac{dy(t)}{dt}+by(t)=x(t) \longrightarrow (ap+b)Y(p)=X(p)$
- $\displaystyle H(p)= \frac{Y(p)}{X(p)}= \frac{1}{ap+b}= \frac{1 / b}{\frac{a}{b}p+1} = \frac{K}{1+Tp}$ 
### Gain statique 
$\displaystyle \lim_{t \to + \infty} h(t)= \frac{\displaystyle \lim_{t \to + \infty} y(t)}{\displaystyle \lim_{t \to + \infty} x(t)}=K$ valeur finale 
### Calcule de la réponse indicielle
Pour une entre $E(p)= \frac{E}{p}$
- On cherche :$\displaystyle S(p)=H(p)E(p)= \frac{EK}{p(1+Tp)}= \frac{A}{p} + \frac{B}{1+Tp} = EK (\frac{1}{p}- \frac{1}{(\frac{1}{T})+p})$ 
- On applique $\mathcal{L}^{-1}$ et on trouve : $\displaystyle s(t)=EK(1-e^{-\frac{t}{T}}\cdot u(t))$ 

## Réponse du second ordre 
- $\displaystyle H(p) = \frac{K}{\displaystyle 1+2 \frac{\xi}{\omega_{0}}p+ \frac{p^{2}}{\omega_{0}^{2}}}$ 
- $\xi$ : Coefficient d'amortissment.
- $\omega_{0}$ : Pulsation propre.

| ![[image reponse 2em ordre.png\|300]] | $\begin{align*} &\text{Pseudo période :  } T_{a} = \frac{2 \pi}{\omega_{0} \sqrt{1-\xi^{2}}} \\ &\text{Prémier maximum :  }T_{m}= \frac{T_{a}}{2} = \frac{\pi}{\omega_{0}\sqrt{1-\xi^{2}}} \\ &\text{Depassement :  } D = KE e^{-\frac{\pi \xi }{\sqrt{1-\xi^{2}}}} \\ &T\rightarrow 63 \% KE \\ &3T\rightarrow 95 \% KE \end{align*}$ |
| ------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
### Détermination de $K$
Valeur finale qui faut $KE$
### Détermination de $T$
tangente à l'origine

- $\displaystyle\frac{D_{1}}{KE}=e^{-\frac{\xi \pi}{\sqrt{1-\xi^{2}}}}$ 
- $\displaystyle t_{1}= \frac{\pi}{\omega \sqrt{1- \xi^{2}}}$ 