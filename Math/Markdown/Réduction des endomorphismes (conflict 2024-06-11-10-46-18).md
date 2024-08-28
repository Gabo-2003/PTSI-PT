---
tags:
  - algebre_lineaire
---
 ## Éléments propres 
### Valeurs propres 
Soit $f \in  \mathcal{L}(E)$, $\lambda \in \mathbb{K}$ est une valeur propre de $f$ :
$\begin{align*} \Leftrightarrow& f- \lambda id_{E} \text{  n'est pas injective} \Leftrightarrow \lambda id_{E} - f \text{  n'est pas injective}  \\ \Leftrightarrow& \ker(\lambda id_{E} - f) \neq \{ 0 \} \\ \Leftrightarrow& \exists x \in E ;\quad f(x) = \lambda x\end{align*}$
Et aussi 
$\begin{align*}\Leftrightarrow& rg(\lambda I_{n}- A) \neq rg_{max} = n\\ \Leftrightarrow& \det(\lambda I_{n}-A) = 0\end{align*}$
### Vecteurs propres 
Soit $f \in \mathcal{L}(E)$, un vecteur $x \in  E$ non nul est un vecteur propre de $f$ 
$\Leftrightarrow \exists \lambda  \in \mathbb{K}$ vérifiant $f(x) = \lambda x \Leftrightarrow AX = \lambda X$ 
Et aussi 
$\Leftrightarrow \begin{cases} x \neq 0_{E} \\ \text{et } \\ Vect(x) \text{  est stable par  } f \end{cases}$ 
- Une famille de vecteurs propres associes à des valeurs propres distincts est libre.
### Sous-espace propre
Si $\lambda$ est une valeur propre de $f \in \mathcal{L}(E)$, alors :
- $E_{\lambda } = \ker(\lambda id - f) \neq 0$
- $E_{\lambda }$ est un s.e.v de $E$ 
- Une somme finie de s.e.p associe à des valeurs propres distincts est toujours directe. 
### Polynôme caractéristique en dimension finie 
Soit $f \in \mathcal{L}(E)$,  $\det(\lambda \cdot id_{E} -f)$ est le polynôme caractéristique de $f$ noté $\chi_{f}$. 
- Le polynôme caractéristique de $f$ est unitaire de degré $n$.
- Deux matrices semblables ont le même polynôme propre. 
#### Racines du polynôme caractéristique 
$\lambda$ est valeur propre de $f \Leftrightarrow$ $\lambda$ racine de $\chi_{f}.$
Soit $E$ un $\mathbb{R}$.e.v de dimension $n$ et $f \in \mathcal{L}(E)$, $f$ a au plus $n$ valeurs propres comptées avec leur multiplicité.
Soit $E$ un $\mathbb{C}$.e.v de dimension $n$ et $f \in \mathcal{L}(E)$, $f$ a exactement $n$ valeurs propres comptées avec leur multiplicité.
- $1 \leq \dim(E_{\lambda }) \leq m(\lambda)$

## Diagonalisabilité 
$f \in \mathcal{L}(E)$ est diagonalisable s'il existe une base (de vecteurs propres) ou la matrice de $f$ est diagonale. 
### Caractérisation de la diagonalisabilité
$f$ est diagonalisable $\Leftrightarrow$ les sous-espaces propres sont supplémentaires. 
#### Par le polynôme propre
$f$ est diagonalisable $\Leftrightarrow \chi_{f}$ est scindé et $\dim(E_{\lambda}) = m(\lambda)$
#### Cas particulière 
- Si $f$ admet $n$ valeurs propres distinct, $f$ est diagonalisable.
##### ![[Isométries vectorielles#Théorème spectral|Théorème spectrale]] 

## Trigonalisation 
On dit que $f$ est trigonalisable si il existe une base de $E$ dans laquelle la matrice de $f$ est triangulaire. 
### Trigonalisation et polynôme caractéristique
- $f$ est trigonalisable $\Leftrightarrow \chi_{f}$ est scindé sur $\mathbb{K}$ 
	$\Leftrightarrow$ avec $p$ le nombre de valeurs propres distincts :
	 $\displaystyle  \begin{cases} \det(f) = \prod_{i=1}^{p} \lambda _{i}^{m_{i}} \\ \text{et} \\ tr(f) = \sum_{i=1}^{p} m_{i}\lambda_{i}  \end{cases}$
