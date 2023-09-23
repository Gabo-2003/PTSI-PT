#espace_vectoriel 
Un espace vectoriel $E$ est de dimension finie / infinie s'il admet une famille génératrice finie / infinie. 
### Théorème de la base extraite 
De tout [[Espaces vectoriels#Famille génératrice|famille génératrice]] de $E$, on peut extraire une base. 
### Théorème de la base incomplète 
Soit $G$ une [[Espaces vectoriels#Famille génératrice|famille génératrice]], il existé $G' \in G$ tel que $G'$ est une base de $E$.

## Dimension d'une espace de dimension finie
- Si une [[Espaces vectoriels#Famille génératrice|famille génératrice]] de $n$ vecteurs engendre une de $n+1$, la 2èm est lié. 
- Soit $E$ une $\mathbb{K}.e.v$ et $\dim(E)=n$. Soit $F=(u_{1}, \ldots, u_{p})$ : 
	- $F$ est une base $\Rightarrow n=p$
	- Si $n=p$ : $F$ [[Espaces vectoriels#Base, coordonnées|base]] $\Leftrightarrow F$ [[Espaces vectoriels#Famille libre|libre]] $\Leftrightarrow F$ [[Espaces vectoriels#Famille génératrice|génératrice]]. 

## Rang d'une famille
$rg(u_{1}, u_{2}, \ldots, u_{p})= \dim(vect(u_{1}, \ldots, u_{p}))$ 
- $rg(u_{1}, u_{2}, \ldots, u_{p})=p \Leftrightarrow (u_{1}, u_{2}, \ldots, u_{p})$ est [[Espaces vectoriels#Famille libre|libre]] 
- $rg(u_{1}, u_{2}, \ldots, u_{p})=n \Leftrightarrow (u_{1}, u_{2}, \ldots, u_{p})$ est [[Espaces vectoriels#Famille génératrice|génératrice]] de $E$ ($\dim(E)=n$)

## $s.e.v$ de dimension finis 
Soit $E$ une $\mathbb{K}.e.v$ et $F$ et $G$  $s.e.v$ de $E$ avec $\dim(E)=n$ 
- Si $\dim(F)=p$   alors  $\dim(F) \leq \dim(E)$ 
- Soit $B_{F}$ une base de $F$. Si $p=n$. $B_{F}$ base de $E \Leftrightarrow vect(B_{F})=E=F$ 
- $\dim(F+G)=\dim(F)+\dim(G)-\dim(F\cap G)$ 
- $E=F\oplus G \Leftrightarrow \begin{cases} \dim(F)+\dim(G)=\dim(E)  \\ F\cap G = \{ 0 \} \end{cases}$ 
- $E=F\oplus G \Leftrightarrow \exists$ une base $B$ de $E\; ; \;B=B_{F}+B_{G}$ 

## Application linéaire de dimension finie
- Soit une $\mathbb{K}.e.v$ de $E$ de base $\mathcal{B}=(\overrightarrow{e_{1}}, \ldots, \overrightarrow{e_{p}})$,  soit $(y_{i})_{1\leq i \leq p}$ une famille de $p$ vecteurs d'un $\mathbb{K},e,v \; F$. $\exists! f :E \longrightarrow E$ tel que $\forall i,  f(e_{i})=y_{i}$. 
- Une application linéaire $f: E \longrightarrow F$ est entièrement déterminé par l'image des vecteurs d'une base $\mathcal{B}$ de $E$. $\dim(\mathcal{L}(E,F))=\dim(E) \times \dim(F)$ 
- Soit $u \in \mathcal{L}(E,F)$, soit $\mathcal{B}=(e_{i})$ base de $E$, soit $E$ et $F$ de dimension finie. Si $Im(u)$ est de dimension finie :
	- $rg(u)=\dim(Im(u))=rg(u(e_{1}), \ldots, u(e_{p}))$ 
	- $rg(u \circ v) \leq \min(rg(u),rg(v))$ 
	- $u$ injective $\Leftrightarrow u(\mathcal{B})$ est libre. 
	- $u$ surjective $\Leftrightarrow u(\mathcal{B})$ génératrice de $F$.
	- $u$ bijective $\Leftrightarrow u(\mathcal{B})$ base de $F$. 
	- $E$ et $F$ isomorphismes s'il existe une isomorphisme $u: E \longrightarrow F$ 
	- $E$ et $F$ isomorphismes $\Leftrightarrow \dim(F)= \dim(E)$ 
	- Si $u \in \mathcal{L}(E,F)$ et si $\dim(E)=\dim(F)$
		- Alors $u$ injective $\Leftrightarrow u$ surjective $\Leftrightarrow u$ bijective. 
### Formule du rang
$\dim(E)=\dim(\ker(u))+\dim(Im(u))$ 