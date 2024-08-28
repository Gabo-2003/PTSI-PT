## Intégrale généralisée sur un intervalle quelconque 
### Définition
Soit $I \subset \mathbb{R}$ une intervalle avec une seule singularité  $a \in \overline{\mathbb{R}}$.
Soit $f$ continue sur $I$ alors 
$\displaystyle \int_{I} f$ converge $\displaystyle \Leftrightarrow \begin{cases} \displaystyle \int_{I} f \underset{t \to  a } \longrightarrow \text{  limite finie  } \\ \displaystyle  \text{ou} \\  \text{  Soit  } F \text{   une primitive de  }f, F(t) \underset{t \to  a } \longrightarrow \text{  limite finie  }\end{cases}$
### Propriétés 
Soit $I \subset \mathbb{R}$ une intervalle avec une seule singularité  $a \in \overline{\mathbb{R}}$.
#### Relation de Chasles
On prend par exemple $I = ]a,b]$ avec  $b \in  \mathbb{R}$.
Soit $f$ continue sur $I$ et $c \in ]a,b]$
- $\displaystyle \int_{a}^{b} f \text{  et  } \int_{a}^{c} f$ sont de même nature. 
- Si $\displaystyle\int_{a}^{b} f$ converge, alors $\displaystyle \int_{a}^{b} f = \int_{a}^{c} f + \int_{c}^{b} f$
#### Linéarité 
Soit $f$ et $g$ continues sur $I$
Si  $\displaystyle \int_{I} f$ et $\displaystyle \int_{I} g$ convergent alors  
- $\lambda \in \mathbb{R}, \quad \displaystyle \int_{I} f+ \lambda  g= \int_{I} f + \lambda  \int_{I} f$ converge  
#### Complexes
Soit $f$ continue sur $I \subset \mathbb{C}$ 
- $\displaystyle \int_{I}f$ converge $\displaystyle \Leftrightarrow \int_{I}Re(f) \text{  et  } \int_{I} Im(f)$ convergent
- Et si $\displaystyle\int_{I}f$ converge :  $\displaystyle\int_{I}f = \int_{I}Re(f) + \int_{I} Im(f)$ 
#### Positivité de l'intégrale 
Soit $f$ continue et positive sur $I$ 
- Si $\displaystyle\int_{I} f$ converge alors  $\displaystyle \int_{I} f > 0$
### Théorèmes de convergence pour les fonctions positives
#### Théorème de majoration pour les fonctions positives
Soit $f$  continues et positives sur $I$ 
$\displaystyle \int_{I} f$ converge si $\displaystyle x \mapsto \int_{I}f$ est majorée sur $I$ 
#### Théorème de comparaison des intégrales des fonctions positives
Soit $f$ et $g$ continues et positives sur $I$ 
$\displaystyle \int_{I} f$ converge si
$\begin{cases} \displaystyle f<g \text{  et  } \int_{I} g \text{  converge  }  \\ \text{ou} \\ \displaystyle f \underset{a } \sim g \text{  et  } \int_{I} g \text{  converge  }  \\ \displaystyle \text{ou} \\ \displaystyle f \underset{a } = o(g) \text{  ou  } f \underset{a } = O(g)\text{  et  } \int_{I} g \text{  converge  } \end{cases}$
### Prolongement par continuité 
Soit $f$ continue sur $I$. Si $f \underset{a} \longrightarrow$ limite finie.
- Alors $\displaystyle\int_{I} f$ converge.
### Cas des intervalles ouvertes $]a,b[$ 
On prend $c \in  ]a,b[$ et on étudie séparément
$\displaystyle \int_{a}^{c} f$ et $\displaystyle \int_{a}^{c} f$ 

## Calcule des intégrales
### Changement de variable
Soit $f$ continue sur $]a,b[$ et  $\varphi : ]\alpha , \beta [ \longrightarrow ]a,b[$ strictement monotone, de classe $C^{1}$ et bijective. 
Alors $\displaystyle \int_{a}^{b} f(u) \: d{t}$ de même nature que $\displaystyle \int_{\alpha}^{\beta } f(\varphi (u)) \: \varphi'(u) d{u}$
Et si convergentes, $\displaystyle \int_{a}^{b} f(t) \: d{t} = \int_{\alpha}^{\beta } f(\varphi (u)) \: \varphi'(u) d{u}$
### Intégration par partie
Soit $u$ et $v$ de classe $C^{1}$ sur $]a,b[$ avec  $a \in  \mathbb{R} \cup \{ - \infty  \}$ et $b \in  \mathbb{R} \cup \{ + \infty  \}$.
Si $uv \underset{a} \longrightarrow$ limite finie et $uv \underset{b} \longrightarrow$ limite finie.
Alors $\displaystyle \int_{a}^{b} vu'$ et $\displaystyle \int_{a}^{b} uv'$ de même nature.
Et si convergentes : $\displaystyle \int_{a}^{b} vu' = [uv]_{a}^{b} - \int_{a}^{b} uv'$

## Intégrales de référence
### Sur $[a, + \infty[$
Soit $\alpha \in R$ 
- $\displaystyle \int_{1}^{+ \infty } \frac{1}{t^{\alpha }} \: d{t}$ converge si $\alpha >1$ 
- $\displaystyle \int_{- \infty }^{-1} \frac{1}{t^{\alpha }} \: d{t}$ converge si $\alpha >1$
- $\displaystyle \int_{0}^{+ \infty } e^{-\alpha t} \: d{t}$ converge si $\alpha >0$
### Singularité en $0$ 
- $\displaystyle\int_{0}^{1} \frac{1}{t^{\alpha }} = \frac{1}{1-\alpha }$ donc converge $\Leftrightarrow \alpha <1$ 
- $\displaystyle \int_{0}^{1} ln(t) \: d{t} = -1$ donc converge.
### Pour $a<b$ réels et $\alpha  \in  \mathbb{R}$ 
$\displaystyle \int_{a}^{b} \frac{1}{(t-a)^{\alpha }} \: d{t}$ et $\displaystyle \int_{a}^{b} \frac{1}{(b-t)^{\alpha }} \: d{t}$ convergent $\Leftrightarrow \alpha <1$


## Intégrabilité 
### Convergence absolue
Soit $f$ continue sur $I$. 
Si  $\displaystyle \int_{I} |f|$ converge alors  $\displaystyle \int_{I} f$ converge absolument $\Rightarrow$ converge. 
#### Inégalité triangulaire
Si $\displaystyle \int_{I} f$ converge absolument, alors $\left| \int_{I} f  \right| \leq \int_{I} |f|$
### Intégrabilité 
$f$ est intégrable sur $I$ si :
- $f$ continue sur  $I$ et $\displaystyle \int_{I} f$ absolument convergente.
On peut appliquer le théorème de comparaison
- il faut faire $|f| \leq  |g|$
#### Propriétés
- Inégalité triangulaire 
- $\mathcal{L}^{1}(I, \mathbb{K})$ c'est l'ensemble des fonctions intégrables sur un intervalle $I$.
### Fonctions de référence
- $\displaystyle t \mapsto \frac{1}{t^{\alpha }}$ est intégrable en $0^{+} \Leftrightarrow \alpha  < 1$
- $\displaystyle t \mapsto \frac{1}{t^{\alpha }}$ est intégrable en $+ \infty  \Leftrightarrow	\alpha >1$ 
- $\displaystyle t \mapsto e^{-\alpha t}$ intégrable en $+ \infty \Leftrightarrow	\alpha >0$ 
- $t \mapsto \ln(t)$ est intégrable en $0^{+}$ 
- $\displaystyle t \mapsto \frac{1}{|t-a|^{\alpha }}$ intégrable en $a \Leftrightarrow \alpha < 1$ 

## Théorème d'intégration terme à terme 
Soit $(f_{n})_{\mathbb{N}}$ telle que $fn : I \subset \mathbb{R} \longrightarrow \mathbb{R}$.
- Si tout $f_{n}$ est intégrable sur $I$.
- Si $\forall t \in  I$ la série  $\displaystyle \sum f_{n}(t)$ converge. 
- Si $\forall t \in I$, $\displaystyle S(t) = \sum_{n=0}^{+ \infty }f_{n}(t)$ est continue sur $I$.
- Et si $\displaystyle\sum \int_{I}|f_{n}(t)|$ converge.
Alors $S$ est intégrable sur  $I$
Et  $\displaystyle \int_{I}S(t)dt =\int_{I} \sum_{n=0}^{+ \infty } f_{n}(t)= \sum_{n=0}^{+ \infty } \int_{I} f_{n}(t)$