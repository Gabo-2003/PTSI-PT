#espace_vectoriel 
### Loi de composition interne
$+: E\longrightarrow E ; (u,v)\longmapsto u+v$ 
### Loi de composition externe
$\cdot : \mathbb{K}\times E \longrightarrow E ; (\lambda, u) \longmapsto \lambda u$ 
### Définition
On appelle $\mathbb{K}.e.v$ un ensemble $E$ muni de la loi interne et externe. 

## Sous-ensemble vectoriel
$H$ de $E$ est un *$s.e.v$*  si $(H,+, \cdot)$ est une $\mathbb{K}.e.v$.
$H \: s.e.v \text{  de  } E \Leftrightarrow \begin{cases} H \subset E \\ H \neq \varnothing \quad(\text{on vérifie que  } 0_{E} \in H) \\ H \text{  stable par combinaison linéaire} \end{cases}$ 
### Sous-ensemble engendré
Par la famille finis $\{u_{i}\}_{i \in I}$ l'ensemble de combinaisons linéaires de vecteurs $u_{i}$. Ce $s.e.v$ sera noté $vect(u_{1}, \ldots, u_{n})$. 
- Vérification : Soit $H= \{ \text{Combinaison linéaire de  }u_{1}, u_{2} , \ldots, u_{n} \}$ $H$ est un $s.e.v$ de $E$. 
### Intersection 
Soit $A$ et $B$  $s.e.v$ alors $A \cap B$ $s.e.v$ de $E$ 

## Familles finies de vecteurs
### Famille génératrice 
$(u_{1}, \ldots, u_{n})$ est dit famille génératrice d'un $s.e.v$ $F$ si $F=vect(u_{1}, \ldots, u_{n})$. 
- Tout famille contenant une famille génératrice d'un espace $F$ est, elle même, famille génératrice. 
### Famille libre 
La famille $(x_{1}, \ldots , x_{2})$ est libre si $\forall (\alpha_{1}, \ldots, \alpha_{p}) \in \mathbb{K}^{p}, \quad \alpha_{1} x_{1}+ \ldots + \alpha_{p}x_{p}=0$ 
$\Leftrightarrow \alpha_{1} = \alpha_{2}=\ldots = \alpha_{n}=0$ 
### Famille lié
$\alpha_{1} x_{1}+ \ldots + \alpha_{p}x_{p}=0$ mais $(\alpha_{1}, \ldots, \alpha_{p}) \neq (0, \ldots, 0)$ 
- Tout famille de polynômes non nuls de degrés distincts 2 à 2 (échelonnes) est libre.
### Base, coordonnées
Une base est une famille libre et génératrice.
$B=(e_{i})_{1 \leq i \leq n}$ une base d'une $\mathbb{K}.e.v$ de $E$ $\Leftrightarrow$ pour tout vecteur $x$ de $E$  $\exists! (\alpha_{1}, \alpha_2, \ldots, \alpha_{n}) \in \mathbb{K}^{n}$ tel que $x=\alpha_{1} e_{1}+ \ldots + \alpha_{n} e_{n}$. 
### Somme de deux $s.e.v$ 
Soit $F$ et $G$ deux $s.e.v$ de $E$.  $F+G = \{ u \in E \; / \; \exists (u_{F}, u_{G}) \in F \times G \; ; \; u=u_{F}+u_{G} \}$ 
- Si le couple est unique, alors on dit que la somme est directe : $F \oplus G \Leftrightarrow F \cap G=\{ 0_{E} \}$ 
### Sous espaces supplémentaires
$F$ et $G$ de $E$ supplémentaires $\Leftrightarrow E = F \oplus G$. 