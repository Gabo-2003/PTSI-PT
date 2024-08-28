---
tags:
  - probabilite
---
## Variables aléatoires discrètes 
### Ensembles dénombrables 
Si $X$ est dénombrable, alors il existe
$\begin{align*} \varphi : \mathbb{N} &\longrightarrow X \\ n &\longmapsto \varphi (n) = x_{n}\end{align*}$
- On a une énumération de $X$,  $X= \{ x_{n} \setminus n \in \mathbb{N} \}$
- Un ensemble est dit "au plus dénombrable" si il est fini ou dénombrable. 
### Tribus des évènements 
Soit $\Omega$ un univers (un ensemble). Si $\Omega$ est au plus dénombrable, alors $\mathcal{P}(\Omega )$, l'ensemble des parties de $\Omega$, est l'ensemble des évènements. 
Si $\Omega$ n'est pas au plus dénombrable on ne peut pas utiliser $\mathcal{P}(\Omega)$. On se contente d'une partie $\mathcal{A} \subset \mathcal{P}(\Omega )$ qu'on appelle une tribu.
Une telle tribu doit vérifier : 
- $\Omega \subset \mathcal{A}$
- Stabilité par passage au complémentaire.
- Stabilité par union dénombrable. 
Alors on dit que $(\Omega, \mathcal{A})$ est un espace probabilisé. 
#### Propriétés d'une tribu $\mathcal{A}$ sur $\Omega$
- ...
### Probabilité 
Une probabilité sur $(\Omega , \mathcal{A})$ est une application 
$P: \mathcal{A} \longrightarrow [0,1]$ 
vérifiant $P(\Omega )=1$.
- On dit que $(A_{n})_{\mathbb{N}}$ est une suite d'évènements deux à deux incompatibles si $\forall (i,j) \in \mathbb{N}^{2}, i \neq j, A_{i} \cap A_{j} = \varnothing$ 
#### Additivité dénombrable
Si $(A_{n})_{\mathbb{N}}$ est une suite d'évènements deux à deux incompatibles :
- La série $\sum P(A_{n})$ converge et $\displaystyle P \left( \bigcup_{n=0}^{+\infty } A_{n} \right) = \sum_{k=0}^{+\infty } P(A_{n})$
- On dit que $(\Omega , \mathcal{A}, P)$ est un espace probabilisé.
### Conséquence de l'additivité dénombrable 
#### Continuité croissante 
Si $(A_{n})_{\mathbb{N}}$ vérifie $A_{n }\subset A_{n+1}$ alors :
- $\displaystyle P \left( \bigcup_{n}^{+ \infty }A_{n} \right) = \lim_{n \to \infty} P(A_{n})$
#### Continuité décroissante
Si $(A_{n})_{\mathbb{N}}$ vérifie $A_{n +1}\subset A_{n}$ alors :
- $\displaystyle P \left( \bigcap_{n}^{+ \infty }A_{n} \right) = \lim_{n \to \infty} P(A_{n})$
#### Limite de la probabilité d'une union dénombrable quelconque
Soit $(\omega , \mathcal{A}, P)$ une espace probabilisé et $( A_{n} )_{\mathbb{N}}$ une suite dénombrable quelconque d'évènements, alors : 
- $\displaystyle \lim_{N \to \infty} P \left( \bigcup_{n=0}^{N} A_{n} \right) = P \left( \bigcup_{n=0}^{+ \infty } A_{n} \right)$
- $\displaystyle \lim_{N \to \infty} P \left( \bigcap_{n=0}^{N} A_{n} \right) = P \left( \bigcap_{n=0}^{+ \infty } A_{n} \right)$
