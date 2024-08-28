---
tags:
  - algebre_lineaire
---
## Produit et somme des espaces vectoriels 
Soit la famille finie $(E_{i})_{[ [1,p]]}$ on a :

$\displaystyle \dim \left( \sum_{i=1}^{p} E_{i} \right) \leq \sum_{i=1}^{p} \dim(E_{i})$
- La somme est directe $\Leftrightarrow$ on a égalité.

## Sous - espaces stables 
### Sous espaces stables par endomorphisme
Soit $E$ un $\mathbb{K}.e.v$ et  $u \in \mathcal{L}(E)$. Un $s.e.v$ $F$ de $E$ est stable par $u$ si : $u(F) \subset F$
- $\ker(u)$ stable par $u$ 
- $Im(u)$ stable par $u$ 
- Si $Im(u) \subset F$, $F$ stable par $u$
### Matrice par blocs 
Soit $E$ un espace vectoriel de dimension finie $n$, soit $u \in  \mathcal{L}(E)$ et $F$ un $s.e.v$ de  $E$
-  $F$ stable par $u \Leftrightarrow Mat_{\mathcal{B}}(u) = \begin{pmatrix} A & B \\ (0) & D \end{pmatrix}$ 

## Trace
### Trace d'une matrice carré 
C'est un scalaire égal à la somme des éléments diagonaux de la matrice :
$\displaystyle tr(A) = \sum_{i=1}^{n} a_{ii}$
- $tr(A) = tr(A^{\intercal})$ 
- $tr : A \mapsto tr(A)$ est une application linéaire
- $tr(AB)= tr(BA) \implies tr(P^{-1}AP) = tr(A)$
- Deux matrices semblables ont la même trace
### Trace d'un endomorphisme en dimension finie
$tr(u)$ : trace de la matrice de $u$ dans n'importe quelle base

## Hyperplans en dimension finie
### Hyperplan d'un $\mathbb{K}.e.v$ en dimension finie
Une hyperplan est tout  $s.e.v$ admettant une droite vectorielle comme supplémentaire 
$H$ est un hyperplan de $E \Leftrightarrow \dim(H) = \dim(E)-1$ 
### Équation d'un hyperplan
Soit $E$ de dimension finie et de base  $B$ 
- Si $H$ hyperplan de $E$, $\exists (a_{1}, a_{2}, \ldots, a_{n}) \in \mathbb{K}^{n}$ non tous nuls tel que $\forall x \in  E$ de coordonnais $(x_{1}, x_{2}, \ldots, x_{n})$ dans $\mathcal{B}$ 
$x \in H \Leftrightarrow a_{1}x_{1} + a_{2}x_{2}+ \ldots + a_{n}x_{n}=0$ 
### Intersection d'hyperplans 
Soit $E$ de dimension $n$ et $p \leq n$
L'intersection de $p$ hyperplans de $E$ est de dimension au moins $n-p$