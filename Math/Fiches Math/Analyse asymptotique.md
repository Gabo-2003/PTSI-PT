## Relation de comparaison 
Le rapport $\displaystyle \frac{f(x)}{g(x)}$ lorsque $x \longrightarrow a$
- $f$ dominé par $g$ : Si le rapport est borné $\displaystyle f(x) \underset{a}= O(g(x))$
- $f$ négligeable devant $g$ : $\displaystyle \lim_{x \to a} \frac{f(x)}{g(x)}=0, \quad f(x) \underset{a}=o(g(x))$
- $f$ équivalente à $g$ : $\displaystyle \lim_{x \to a} \frac{f(x)}{g(x)} = 1, \quad f(x) \underset{a} \sim g(x)$ 
### Propriétés 
- Si $f \sim g$ les limites de  $f$ et $g$ en $a$ sont identiques.
- Si  $f \sim g$ alors ils sont de même signe près de $a$.
- Si$f \sim g$ et $h \sim \phi$ au voisinage de $a$. 
$\quad \quad \begin{cases} f \times h \underset{a}\sim g \times \phi \quad \text{et} \quad \displaystyle \frac{f}{h} \underset{a} \sim \frac{g}{\phi} \\ (f(x))^{\alpha} \underset{a}\sim (g(x))^{\alpha} \quad \alpha \in \mathbb{R} \text{  fixé} \\ \text{Il es faut :  } f+h \sim g+ \phi, \quad \psi(f(x)) \underset{a}\sim \psi(g(x))    \end{cases}$

## Développement limité 
On approche une fonction $f$ "au mieux possible" par un polynôme au voisinage de $x_{0}$.
- Si $f$ admet une $DL_{n}(a)$, les coefficients sont uniques.
- Un $DL_{n}(a)$ donne par troncature $DL_{p}(a)$ où $p<n$.
- $f$ admet un $DL_{0}(a) \Leftrightarrow  f$ admet un limite en $a$.
- $f$ admet un $DL_{1}(a) \Leftrightarrow f$ dérivable en $a$.
$\quad \quad \bullet f(a+h)= \underbrace{f(a)+hf'(a)+h}_{\text{éq tangente}} \epsilon (h)$
### Formule de Taylor-Young 
Soit $f$ de classe $C^{p}$ 
- $f(x_{0}+h)= f(x_{0})+f'(x_{0})h+ \frac{f''(x_{0})}{2!} + \ldots + \frac{f^{(p)}(x_{0})}{p!}+h^{p}\epsilon (h)$  
- $\displaystyle f(x)=\sum_{k=0}^{p} \frac{(x-a)^{k}}{k!} f^{(k)}(a)  +o(x^{p})$ 

## Applications des Développements limités 
- Calculs de limites, [[Limites et continuité#Prolongement par continuité|prolongement par continuité]], calculs de dérivé.
- Position d'une courbe par rapport à sa tangente 
- Asymptote 
- Extremum local d'une fonction 

## Comparaison des suites 

