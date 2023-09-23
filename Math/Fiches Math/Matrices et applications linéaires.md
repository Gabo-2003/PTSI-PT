#espace_vectoriel 
## Matrices d'une application linéaire dans des bases 
Soit $E$ de base $\mathcal{B}=(e_{1}, \ldots, e_{p})$, soit la famille $(u_{1}, \ldots, u_{p})$ vecteurs de $E$
- $M_{B}(u_{1}, \ldots, u_{p})$ matrices dont la j-èm colonne est les coordonnées de $u_{j}$ dans $\mathcal{B}$.   
Soit $f \in \mathcal{L}(E,F)$, $E$ de base $\mathcal{B}=(e_{1}, \ldots, e_{p})$, $F$ de base $\mathcal{B}'=(e_{1}', \ldots, e_{p}')$ 
- $M_{BB'}(f)$ matrice dont la j-èm colonne est les coordonnées de $f(e_{j})$ dans $\mathcal{B'}$ 
### Coordonnées de l'image
$f \in \mathcal{L}(E,F)$ ,   $A=mat_{BB'}(f)$ 
- $x \in E$ de $coord_{B}(x)=X_{B}$ 
- $y \in F$ de $coord_{B'}(y)=Y_{B'}$ 
- $y=f(x) \Leftrightarrow Y_{B'}=A\, X_{B}$ 
- Réciproquement : soit $f: E \longrightarrow F$, si $\exists A ; f(x)$ de coord $Y_{B'}=A\,X_{B}$ alors $f$ est linéaire et $A=mat_BB'(f)$ 
### Matrices de combinaisons linéaires 
$(f,g) \in \mathcal{L}(E,F)^{2}$ 
- $mat_{BB'}(f+g) = mat_{BB'}(f)+mat_{BB'}(g)$ 
- $mat_{BB'}(\lambda f)= \lambda mat_{BB'}(f)$ 
- L'application $mat_{BB'}$ est une isomorphisme.
### Matrices de la composé 
![[image matrice compose.png]]
- $mat_{BB''}(f \circ g)= mat_{B'B''}(f) \times mat_{BB'}(g)$ 
### Matrice inversible et isomorphisme 
$f \in \mathcal{L}(E,F)$ 
- $f$ isomorphisme $\Leftrightarrow A$ inversible $\Rightarrow mat_{B'B}(f^{-1})=(mat_{BB'}(f))^{2}$ 
- Si $f$ endomorphisme de $E$, $f$ automorphisme $\Leftrightarrow mat_{B}(f)$ inversible $\Rightarrow mat_{B}(f^{-1}) = (mat_{B}(f))^{-1}$ 

## Application linéaire canoniquement associe à une matrice, rang d'une matrice
Tout matrice $A$ peut être associe a une application linéaire. Cette application s'appelle application linéaire canonique associe à $A$. 
### Noyau, image et rang
Ces trois caractéristiques sont la même pour la matrice et pour l'application.
- Les colonnes de $A$ engendrent l'image 
- $A$ inversible $\Leftrightarrow \ker(A)=0 \Leftrightarrow$ les colonnes de $A$ engendre l'espace. 

## Changement de bases 
Soit $E$ de base $B=(e_{1}, \ldots, e_{n})$, soit $B'=(u_{1}, \ldots, u_{p})$   
- $B'$ base de $E \Leftrightarrow \dim(E)=\dim(B')$ et $mat_{B}(B')$ inversible. 
- $mat_{B}(u_{1}, \ldots, u_{n})=P_{BB'}$ : matrice de passage de $B$ à $B'$. 
- $P_{BB''} = P_{BB'} \times P_{B'B''}$       
- $(P_{B'B})^{-1}=P_{BB'}$   
### Changement sur les coordonnées
- $X_{B}=P_{BB'} X_{B'}$ 
- $X_{B'}=P_{B'B} X_{B}$ 
### Changement sur les matrices d'une application 
- $f \in \mathcal{L}(E,F) \begin{cases} E \text{  de bases  }B_{1} \text{  et  } B_{1}' \quad P=P_{B_{1}B_{1}'} \\ F \text{  de bases  }B_{2} \text{  et  } B_{2}' \quad Q=P_{B_{2}B_{2}'} \end{cases}$
- $A=mat_{B_{1}B_{2}}(f)$  alors  $A'=Q^{-1}AP$ 
- Cas d'endomorphisme : $A'=P^{-1}AP$ 
- $A$ et $A'$ équivalentes : $A'=Q^{-1}A P$     $P$ et $Q$ inversibles.
- $A$ et $A'$ semblables : $A'=P^{-1}AP$      $P$ inversible.