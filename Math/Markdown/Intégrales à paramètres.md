## Théorème de continuité des intégrales à paramètres 
Soit $f : A \subset \mathbb{R} \times I \subset \mathbb{R} \longrightarrow \mathbb{K}$. 
1. Hypothèse de régularité en $x$ :    $\forall t \in I$, $x \longmapsto f(x,t)$ est continue sur $A$.
2. Hypothèse de continuité en $t$ :    $\forall x \in A$, $t \longmapsto f(x,t)$ est continue sur $I$.
3. Hypothèse de domination uniforme en $x$ :   $\forall (x,t) \in A \times I$, il existe une fonction $\varphi$ intégrable sur $I$, tel que $|f(x,t)| \leq \varphi (t)$ 

Alors la fonction $\displaystyle x \longmapsto \int_{I} f(x,t)  \: d{t}$ est définie et continue sur $A$.

## Théorème de dérivation des intégrales à paramètres 
Soit $f : A \subset \mathbb{R} \times I \subset \mathbb{R} \longrightarrow \mathbb{K}$. 
1. Hypothèse de régularité en $x$ :   $\forall t \in I$, $x \longmapsto f(x,t)$ est de classe $C^{1}$ sur $A$.
2. Hypothèse de intégrabilité en $t$ :    $\forall x \in A$, $t \longmapsto f(x,t)$ est intégrable sur $I$.
3. $\displaystyle\forall x \in A$, $\displaystyle t \longmapsto \frac{\partial f}{\partial x}(x,t)$ est continue sur $I$.
4. Hypothèse de domination uniforme en $x$ :    $\forall (x,t) \in A \times I$, il existe une fonction $\varphi$ intégrable sur $I$, tel que $\displaystyle|\frac{\partial f}{\partial x} (x,t)| \leq \varphi (t)$
Alors la fonction $g:x \longmapsto \int_{I} f(x,t) \: d{t}$ est de classe $C^{1}$ sur $A$ et vérifie :
$\displaystyle \forall x \in A, g'(x) = \int_{I} \frac{\partial f}{\partial x}(x,t)   \: d{t}$

## Remarques 
- Si $A$ (intervalle de $x$) n'est pas un segment, on peut travailler sur un segment quelconque $K = [a,b]$ inclus dans  $A$.
	- On fait ça quand on peut pas majorer sur un autre intervalle. On utilise avec le théorème des bornes atteintes.
- Si $I$ (intervalle de $t$) est un segment, alors $A\times  I$ est un fermée bornée, alors on peut utiliser le théorème des bornes atteintes sur $\displaystyle  \frac{\partial f}{\partial x}$. Ce qui donne : $\displaystyle  \left| \frac{\partial f}{\partial x}  \right| \leq M$ et $M$ est constante donc intégrable sur le segment $I$.
