#analyse
## Généralités
### Applications
Une application est la donnée d'une ensemble de départ $E$, d'un ensemble d'arrive $F$, et d'une relation qui associe tout $x$ de $E$ à une élément de $F$ :       $f: E \longrightarrow F; \quad x \longmapsto f(x)$   
#### Application identique :
$Id_{E} : E \longrightarrow E; \quad x \longmapsto x$ 
### Domaine de définition 
Plus grand sous-ensemble de $\mathbb{R}$ ou on peut définir $f$.
### Parité
Soit $f$ définie sur $D$ 
#### Pair
Si $\forall x \in D,$  $f(-x)=f(x)$ 
#### impaire 
$f(-x)=-f(x)$ 
### Périodicité
Soit $f$ définie sur $D$, $f$ de période $T$ si :
$\forall x \in D, \; x+T \in D$   et   $f(x+T)=f(x)$
### Composition des applications
![[image composition des applications.jpg]]

## Plan d'etude d'une fonction
- Recherche du domaine de définition 
- Réduction du domaine d'étude (parité, périodicité, symétries)
- Calcul de la dérivée, recherche de son signe. Tableau de variation (y compris limites aux bords)
- Mise en évidence d'éventuelles asymptotes 
### Asymptote horizontale
$\displaystyle \lim_{t \to \pm \infty} f(x)=b$ la droite d'équation $y=b$ est asymptote.
### Asymptote vertical
$\displaystyle \lim_{t \to a} f(x)= \pm \infty$ la droite d'équation $x=a$ est asymptote.
### Asymptote oblique
$\displaystyle \lim_{t \to \pm \infty} f(x)-ax-b=0$ la droite d'équation $y=ax+b$ est asymptote.

## Fonctions bijectives 
### Bijections 
Une application $f: E \longrightarrow F$ est dite bijective si:
$$\forall y \in F, \; \exists! x \in E \text{  tel que  } y=f(x)$$ Dans ce cas $f^{-1}: F \longrightarrow E$  s'appelle la bijection réciproque de $f$.
$$\forall x \in E, \; \forall y \in F, \; y=f(x) \Leftrightarrow x=f^{-1}(y)$$
### Bijection des fonctions continues strictement monotones sur un intervalle

### Dérivation d'une fonction réciproque
On suppose que $f$ est continue, strictement monotone sur $I$ et réalise ainsi une bijection de $I$ sur $J=f(I)$. Soit $x \in J$. 
Si $f$ est dérivable en $f^{-1}(x)$ et si $f'(f^{-1}(x)) \ne 0$, alors $f^{-1}$ est dérivable en $x$ et 
$$(f^{-1})'(x)= \frac{1}{f'(f^{-1}(x))}$$ 