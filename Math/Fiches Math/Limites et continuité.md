
## Continuité et prolongement par continuité 
### 1èr cas : 
Si $\displaystyle \lim_{x \to a}f(x)$ existe et $a \in D_{f}$. 
Alors $\displaystyle \lim_{x \to a}f(x)=f(a)$, $f$ est continue en $a$. 
### 2èm cas :
Si $\displaystyle \lim_{x \to a}f(x)=l$ existe et $a \notin D_{f}$. 
Dans ce cas on peut prolonger $f$ par continuité. 
### Prolongement par continuité
$\tilde{f} : D_{f} \cup \{ a \} \longrightarrow \mathbb{R}; x \longmapsto \begin{cases} f(x) \text{  si  } x \in D_{f}  \\ l=\tilde{f}(a) \text{  si  } x=a \end{cases}$ 
- $f$ continue en $\displaystyle a \Leftrightarrow \lim_{x \to a^{+}}f(x)=\lim_{x \to a^{-}}f(x)=f(a)$ 
- Toute somme, combinaison linéaire, produit, quotient (avec dénominateur non nul), de fonctions continues est une fonction continue. 
### Tableau de limites 
#### Addition 

| $\lim (f)=$   | $l$    | $l$        | $l$        | $+ \infty$ | $- \infty$ | $+ \infty$ |
| ------------- | ------ | ---------- | ---------- | ---------- | ---------- | ---------- |
| $\lim (g)=$   | $l'$   | $+ \infty$ | $- \infty$ | $+ \infty$ | $-\infty$  | $- \infty$ |
| $\lim (f+g)=$ | $l+l'$ | $+ \infty$ | $- \infty$ | $+ \infty$ | $- \infty$ | F.I           |
#### Produit 


| $\lim (f)=$          | $l$           | $l \neq 0$                                                          | $+ \infty \text{ ou  } - \infty$                                    | $0$                              |
| -------------------- | ------------- | ------------------------------------------------------------------- | ------------------------------------------------------------------- | -------------------------------- |
| $\lim (g)=$          | $l'$          | $+ \infty \text{ ou  } - \infty$                                    | $+ \infty \text{ ou  } - \infty$                                    | $+ \infty \text{ ou  } - \infty$ |
| $\lim (f \times g)=$ | $l \times l'$ | $\underset{\text{reglè de signes}}{+ \infty \text{ ou  } - \infty}$ | $\underset{\text{reglè de signes}}{+ \infty \text{ ou  } - \infty}$ | F.I                       |
#### Quotient

| $\lim (f)=$           | $l$            | $l$                              | $+ \infty \text{ ou  } - \infty$                                    | $l' \neq 0 \text{  ou  }+ \infty \text{ ou  } - \infty$             | $0$        | $+ \infty \text{ ou  } - \infty$ |
| --------------------- | -------------- | -------------------------------- | ------------------------------------------------------------------- | ------------------------------------------------------------------- | ---------- | -------------------------------- |
| $\lim (g)=$           | $l' \neq 0$    | $+ \infty \text{ ou  } - \infty$ | $l' \neq 0$                                                         | $0$                                                                 | $0$        | $+ \infty \text{ ou  } - \infty$ |
| $\lim (\frac{f}{g})=$ | $\frac{l}{l'}$ | $0$                              | $\underset{\text{reglè de signes}}{+ \infty \text{ ou  } - \infty}$ | $\underset{\text{reglè de signes}}{+ \infty \text{ ou  } - \infty}$ | F.I | F.I                              |
## Fonctions continues sur un intervalle 
### Théorème des valeurs intermédiaires 
Soit $f$ une fonction continue et $f(a)<f(b)$
$\forall y \in ]f(a),f(b)[, \exists c \in ]a,b[ \text{  tel que  } y=f(c)$.
### Corollaire du TVI 
Soit $f$, une fonction continue strictement monotone sur un intervalle $I$. Alors $f$ est [[Fonctions d'une variable réelle#Bijections|bijective]] de $I$ sur $J=f(I)$. 
### Théorème des bornes atteintes 
Une fonction continue sur un segment $[a,b]$ est bornée et atteint ses bornes. 
$f([a,b])=[m, M]$   où  $m= \inf_{[a,b]}f$   et  $M=\sup_{[a,b]}f$ 
### Bijection des fonctions continues strictement monotones sur $I$
Soit f une application continue sur $I$ :
- $f$ réalise une bijection sur $I$.
- $f^{-1}$ est continue, strictement monotone et de même sens sur $f(I)=J$.  

