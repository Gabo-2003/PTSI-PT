---
tags:
  - analyse
---
## Convergence d'une série entière et somme
### Définition 
Soit $(a_{n})_{\mathbb{N}}$ une suite de nombres complexes, la série entière de coefficients $(a_{n})$ est :
$\displaystyle \sum _{n\geq0} a_{n}z^{n}$ avec $z \in \mathbb{K}$.
### Lemme d'Abel 
Si il existe $z_{0} \in \mathbb{C}$ tel que $(a_{n}z_{0}^{n})$ est bornée, alors $\forall z \in \mathbb{C} ; \; |z| \leq |z_{0}|$, 
la série $\displaystyle \sum a_{n}z^{n}$ est absolument convergente.
- Si $\sum a_{n}z_{0}^{n}$ converge alors, $\forall z \in \mathbb{C} ; \; z\leq z_{0}$, la série $\sum a_{n}z^{n}$ est absolument convergente. 
### Rayon de convergence
Le rayon de convergence $R$ est le borne supérieur de $\displaystyle \mathcal{E} = \{ r \in \mathbb{R}^{+}  \setminus \, (a_{n}z^{n})_{\mathbb{N}} \text{  bornée}\}$
- $R$ peut être égal à $+\infty$
- Si $|z| < R$, alors $\sum a_{n}z^{n}$ est absolument convergent. 
- Si $|z| > R$, alors $\sum a_{n}z^{n}$ est grossièrement divergente. 
- Si pour un réel $r$ la série converge, alors $R \geq r$. Et si pour $r$ la série diverge, alors  $R \leq r$.
### Domaine de convergence
#### Disque ouverte de convergence
$D_{R} = \{ z \in \mathbb{C} \setminus \, |z|<R  \}$
#### Intervalle ouverte de convergence
$I_{R} = ]-R,R[$
- $\displaystyle S(x) = \sum_{n}^{+\infty } a_{n}z^{n}$ est définie sur $D_{R} \cup \{ \text{points où la série converge} \}$
### [[Séries numériques#Règle de d'Alembert|Règle de d'Alembert]]
Très utile
### Techniques de comparaison
- Si $a_{n} \sim b_{n}$ alors $R_{a} = R_{b}$.
- Si $|a_{n}| \leq |b_{n}|$ alors $R_{b} \leq R_{a}$.
- Si $a_{n} = o(b_{n})$ ou $= O(b_{n})$ alors $R_{b} \leq R_{a}$.
- Soit $\lambda \in \mathbb{C}^{*}$, les séries $\sum a_{n}z^{n}$ et  $\sum \lambda a_{n}z^{n}$ ont le même rayon de convergence.
### Série faussement dérivée
Les séries $\sum a_{n}z^{n}$ et  $\sum n a_{n}z^{n}$ ont le même rayon de convergence.
- Soit  $\alpha \in \mathbb{R}$, $\quad R\left( \sum n^{\alpha } z^{n} \right) =1$
### Somme et produit de séries entières 
#### Somme
Soit $\rho = R\left( \sum (a_{n}+ b_{n}) z^{n} \right)$ 
$$\begin{cases} \rho = \min(R_{a}, R_{b}) \text{  si  } R_{a} \neq R_{b} \\ \rho \geq R_{a} = R_{b} \text{  si  } R_{a} = R_{b}\end{cases}$$
- Si $|z| < \rho$,  $\displaystyle \sum_{n=0}^{+\infty } a_{n}+b_{n} = \sum_{n=0}^{+\infty }a_{n} + \sum_{n=0}^{+\infty } b_{n}$ 
#### [[Séries numériques#Produit de Cauchy de deux séries absolument convergentes|Produit de Cauchy]]
Soit $\sum p_{n}z^{n}$ la série produit de Cauchy des séries entières $\sum a_{n}z^{n}$ et $\sum b_{n}z^{n}$.
Soit $\rho = R\left( \sum p_{n} z^{n} \right)$, $\rho \geq  \min(R_{a}, R_{b})$
Si $|z| \leq \rho$,   $\displaystyle \sum_{n=0}^{+\infty }p_{n}z^{n} = \left( \sum_{n=0}^{+\infty} a_{n}z^{n} \right)  \left( \sum_{n=0}^{+\infty} b_{n}z^{n} \right)$

## Régularité de la fonction somme pour une variable réel
### Continuité 
La fonction somme $S(z)$ d'une série entière est $C^{\infty }$ sur $I_{R}$. 
### Relation entre coefficients et dérivées successives
Si $R>0$,  $\displaystyle \forall  n \in \mathbb{N}, \quad a_{n} = \frac{S^{(n)}(0)}{n!}$
Si pour un réel $0 < r < \min(R_{a},R_{B}), \quad \displaystyle \sum_{n=0}^{+\infty } a_{n}z^{n} = \sum_{n=0}^{+\infty }b_{n}z^{n}$. Alors, $a_{n} = b_{n}$.

## Développement en série entière d'une fonction réelle
### Fonctions développables en série entières 
Soit $f : I \subset \mathbb{R} \longrightarrow \mathbb{C}$, $f$ est développable en série entière au voisinage de $0$ si :  
- Il existe une série entière $\sum a_{n}z^{n}$ de rayon de convergence $R>0$
- Et il existe un réel $0 < r < R$ tel que :
$\displaystyle \forall t \in ]-r,r[, \quad f(t) =  \sum_{n=0}^{+\infty }a_{n}t^{n}$
### Unicité du développement - Série de Taylor
Si $f$ est une fonction développable en série entière au voisinage de $0$ alors il existe une unique série entière dont la somme est égal à $f$ au voisinage de $0$ : 
$\exists r > 0$ tel que $\forall t \in ]-r,r[$,    $\displaystyle f(t) = \sum _{n\geq 0} \frac{f^{(n)}(0)}{n!}t^{n}$
### Formules de Taylor
#### Formule de Taylor avec reste intégral
Soit $f : I \subset \mathbb{R} \longrightarrow \mathbb{K}$ de classe $C^{p+1}$ avec $p \in \mathbb{N}$ et $a\in I$. Alors $\forall x \in I$,
- $\displaystyle f(x) = \sum_{k=0}^{p} \frac{f^{(k)}(a)  }{k!} (x-a)^{k} + \int_{0}^{x} \frac{f^{(p+1)}(t) }{p!}(x-t)^{p} \: d{t}$
#### Inégalité de Taylor-Lagrange
Soit $f : I \subset \mathbb{R} \longrightarrow \mathbb{K}$ de classe $C^{p+1}$ avec $p \in \mathbb{N}$ et a $a \in I$. Si il existe un réel $M$ tel que $\forall t \in I, \quad |f^{(p+1)}(t)| \leq M$.
Alors $\forall x \in I$,
$\displaystyle \left| f(x) - \sum_{k=0}^{p} \frac{f^{(k)}(a) }{k!}(x-a)^{k} \right| \leq M \frac{|x-a|^{p+1}}{(p+1)!}$ 
### Développements usuels de fonctions réelles 
$\displaystyle - \ln(1-x) = \sum_{n=1}^{+\infty } \frac{x^{n}}{n}$

## Séries usuelles d'une variable complexe 
### Série géométrique 
Pour $z \in \mathbb{C}$ avec $|z| <1$,
$\displaystyle \sum_{n=0}^{+\infty } z^{n} = \frac{1}{1-z}$ 
### Série exponentielle 
Pour $z \in \mathbb{C}$, 
$\displaystyle e^{z} = \sum_{n=0}^{+\infty } \frac{z^{n}}{n!}$ 