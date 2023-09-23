**Exercice 1 :**
Montrer que l'application $f : ]0, \frac{\pi}{2}[ \: ; \:t\longmapsto \tan(t)^{\cos(t)}$ est bien définie, continue sur $]0, \frac{\pi}{2}[$ et qu'elle peut être prolongée par continuité en $0$ et $\frac{\pi}{2}$

- $\tan$ définie sur $\mathbb{R} \setminus \frac{\pi}{2} +k \pi$,   $k \in \mathbb{Z}$
- $\cos$ définie sur $\mathbb{R}$ 
Donc on n'as pas des problèmes d'existence.
De plus, $\tan(]0; \frac{\pi}{2}[)=]0, +\infty[$ Alors on n'as pas de problème d'existence avec des puissances non entier (par exemple $\tan(x)^{\frac{1}{2}}=\sqrt{\tan(x)}$ ici)

Donc f est bien définie

**étude en "$0$" et en "$\frac{\pi}{2}$":**
$f(0)=\tan(0)^{\cos(0)}=0^{1}=0$ alors $f$ est continue en $0$
$f(\frac{\pi}{2})=\ldots$ n'existe pas

Or
$\begin{align*}\tan(t)^{\cos(t)}&=e^{\cos(t)\ln(\tan(t))}=e^{\cos(t)(\ln(\sin(t))-\ln(\cos(t))} \\ &=e^{\cos(t)(\ln(\sin(t))} \times e^{-\cos(t)\ln(\cos(t))} \\ &=\sin(t)^{\cos(t)} \times e^{-\cos(t)\ln(\cos(t))} \end{align*}$

$$\text{On a: }\lim_{t \to \frac{\pi}{2}^{-}} \sin(t)^{\cos(t)}=1$$
$$\text{or}\lim_{t\to \frac{\pi}{2}^{-}}\cos(t)\ln(\cos(t))=0 \quad (\lim_{x \to O^{+}}x \ln(x)=0)$$
$$\text{On a aussi:  }\lim_{t\to \frac{\pi}{2}^{-}}e^{-\cos(t)\ln(\cos(t))}=1$$
$$\text{Donc:  }\lim_{t\to \frac{\pi}{2}^{-}}\tan(t)^{\cos(t)}=1$$

Alors on peut prolonger par continuité $f$ en $0$ et $\frac{\pi}{2}$:
On pose: 
$\boxed{\tilde{f}:\left[0;\frac{\pi}{2}\right]\; ;\; t\to \begin{cases} \tan(t)^{\cos(t)}\text{      si     } t \in ]0, \frac{\pi}{2}[ \\ 0 \text{    si    }t=0 \\ 1 \text{    si     } t=\frac{\pi}{2}  \end{cases}}$

**Exercice 2 :**
On souhaite trouver dans ce problème toutes les fonctions  $f : \mathbb{R} \longrightarrow \mathbb{R}$ continues sur $\mathbb{R}$ telles que:
$\forall (x,y)\in \mathbb{R}^{2}, \; f(x+y)+f(x-y) = 2(f(x)+f(y))$

1- On considère une fonction f vérifiant les hypothèses de l'énoncé.

a- Calculer $f(0)$
On pose $y = 0$, alors on a 

$\begin{align*} f(x)+&f(x)=2(fx)+f(0)) \\ \Leftrightarrow &\boxed{f(0)=0} \end{align*}$

b- Etudier la parité de $f$.

$\begin{align*} f(-x-y)+f(-x+y) &=2(f(-x)+f(-y)) \quad \text{Soit:  }x=-x \text{  et  }y=-y  \\ \Leftrightarrow f(x+y)+f(x-y) &= 2(f(x)+f(y))\end{align*}$
**Alors $f$ est paire**

**Exercice 3 :** Soit $p \in \mathbb{N}^{*}$
1- Montrer que si $2^{p}-1$ est paire, alors p est premier.

Soit $p = pq, \quad (p, q) \in \mathbb{N}$
On a: $\begin{align*}(2^{p}-1)(1 + 2^{p}+ \ldots + 2^{p(q-1)})&= 2^{p}+ 2^{2p}+\ldots +2^{pq} -1 -2^{p}-\ldots-2^{p-q-1}\\&=2^{pq}-1=2^{m}-1 \end{align*}$

Alors $2^{p}-1 \mid 2^{m}-1$
or $2^{m}-1$ est premier, on en déduit que
$2^{p}-1=1 \Leftrightarrow2^{p}=2 \Leftrightarrow p=1$
ou
$2^{p}-1=2^{m}-1 \Leftrightarrow 2^{p}=2^{m} \Leftrightarrow p=m$
**Alors les diviseur de $m$ sont $1$ et lui-même**
Donc $\boxed{M\; \text{est premier}}$


**Exercice 4 :**
 Soient $E$ et $F$ des ensembles, soit $f \in \mathcal{F}(E,F)$  et soit $Y$ un sous-ensemble de $F$. Montrer que : 
 $$f(f^{-1}(Y))=Y \cap f(E)$$

On raisonne par double inclusion.

D'un part, Soit 
$\begin{align*} x &\in f(f^{-1}(Y)) \\ \Rightarrow x &\in Y  \hspace{1cm} \text{or } Y \subset F \\ \Rightarrow x &\in F \\ \Rightarrow x &\in f(E)  \end{align*}$
Comme $x \in Y$ et $x \in f(E)$
Alors $x \in Y \cap f(E)$
Donc $\underline{f(f^{-1}(Y)) \subset (Y \cap f(E))}$

D'une autre part, Soit 
$\begin{align*} x &\in Y \cap f(E) \\ \Rightarrow x &\in Y \; \text{et} \; x \in f(E) \\ \Rightarrow x &\in f(f^{-1}(Y)) \end{align*}$
donc $\underline{(Y \cap f(E)) \subset f(f^{-1}(Y))}$

Alors, par double inclusion, $\boxed{f(f^{-1}(Y)) = Y \cap f(E)}$