#espace_vectoriel 
## Applications linéaires, endomorphismes  
Soit $E$  et $F$ deux $k.e.v$ et $f : E \longrightarrow F$ 
$f$ est linéaire si : $\begin{cases} \forall (u,v) \in E^{2} , f(u+v)=f(u)+f(v) \\ \forall u \in E, \forall \lambda \in \mathbb{K}, f(\lambda u)=\lambda f(u) \end{cases}$
- On appelle l'ensemble $\mathcal{L}(E,F)$ 
### Vocabulaire
#### Endomorphisme
$f :E \longrightarrow E$
#### Isomorphisme 
$f : E \longrightarrow F$ avec $f$ bijective
#### Automorphisme 
$f : E \longrightarrow E$ avec $f$ bijective
### Noyau et image d'une application linéaire 
#### Noyau 
Soit $f \in \mathcal{L}(E,F)$ :
$\ker(f)=\{ u \in E / f(u) = 0_{F} \}=f^{-1}(\{0_{E}\})$ 
- $u \in \ker(f) \Leftrightarrow f(u) = 0_{F}$ 
- $f$ [[Algèbre et arithmétique#Injective|injective]]  $\Leftrightarrow \ker(f)=\{ 0_{F} \}$ 
#### Image 
Soit $f \in \mathcal{L}(E,F)$ :
$Im(f)=\{ v \in F / \exists u \in E ; v = f(u) \}$ 
- $v \in Im(f) \Leftrightarrow \exists u \in E ; v=f(u)$ 
- $f$ [[Algèbre et arithmétique#Surjective|surjective]] $\Leftrightarrow \forall  v \in F, v \in Im(f)$ 
- Si $(x_{i})_{i \in I}$ est une [[Espaces vectoriels#Famille génératrice|famille génératrice]] finie de $E$, alors $Im(f)=vect(f(x_{i})_{i \in I} )$ 
### Operations sur les applications linéaires 
Soit $f$ et $g$ linéaires :
$f+g$ linéaire         $\lambda f$ linéaire          $f \circ g$ linéaire 
$f^{-1}$ linéaire 
### Endomorphismes 
On peut utiliser le [[Sommes#Formules du binôme de Newton|binôme]] pour $(f+g)^{n}$ si $f \circ g = g \circ f$ 
- Si $f$ est une isomorphisme, $f^{-1}$ est un isomorphisme.
- Si $f,g \in GL(E)^{2} : \begin{cases} f \circ g \in GL(E) \\ f^{-1}\in GL(E) \end{cases}$

## Projecteurs 
Si $E = F \oplus G \Rightarrow u = u_{F} + u_{G}$ 
- $p(u)=u_{F}$ projection de $E$ sur $F$ selon la direction de $G$ 
- $p$ est une endomorphisme 
- $u = u_{F}+ u_{G} \Rightarrow u=p(u)+u-p(u)$ 
- Caractéristiques : $\ker(p)=G$  $Im(p)=F=\ker(p-Id)$    
- $u \in F \Leftrightarrow p(u)=u$
- $p$ projecteur $\Leftrightarrow \begin{cases} p \text{  endomorphisme} \\ p \circ p = p \end{cases}$ 

## Symétries 
Si $E = F \oplus G \Rightarrow u = u_{F} + u_{G}$ 
$s : u \longmapsto u_{F}-u_{G}$ symétrie par rapport à $F$ selon la direction de $G$. 
- $s=2p-Id_{E}$
- $\ker(s)=\{ O_{E} \}$    $Im(s)=E$ 
- Caractéristiques : $F = \ker(s-Id_{E})$    $G=\ker(s+Id_{E})$ 
- $s$ symétrie $\Leftrightarrow \begin{cases} s \text{  endomorphisme} \\ s\circ s = Id \end{cases}$ 
