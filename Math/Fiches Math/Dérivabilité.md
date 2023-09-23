$\displaystyle f'(a)=\lim_{x \to a} \left(\frac{f(x)-f(a)}{x-a}\right)=\lim_{h \to 0} \left(\frac{f(a+h)-f(a)}{h}\right)$    avec   $x=a+h$

- Si $f$ dérivable en $a$, alors $f$ continue en $a$.
- $f$ dérivable en $a \Leftrightarrow$ elle admet une [[développement limité]] à l'ordre $1$ en $a$ : $f(a+h)=f(a)+f'(a)h+h \varepsilon(h)$    avec $\displaystyle \lim_{h \to 0} \varepsilon(h)=0$
- Tangente à la courbe en $a$ : $y=f'(a)(x-a)+f(a)$.
- Si $f$ dérivable en $f^{-1}(x)$ et si $f'(f(x)) \neq 0$, alors $(f^{-1})'(x)= \frac{1}{f'(f^{-1}(x))}$. 

## Propriétés des fonctions dérivables 
### Théorème de Rolle 
Soit $f$ continue sur $[a,b]$ et dérivable sur $]a,b[$  (avec $a<b$) 
- Si $f(a)=f(b)$ alors $\exists c \in ]a,b[ ; f'(c)=0$ 
### Accroissement finis 
#### Egalité 
Soit $f$ continue sur $[a,b]$, dérivable sur $]a,b[$. Alors $\exists c \in ]a,b[ ; f(b)-f(a)=f'(c)(b-c)$
#### Inégalité
Soit $f$ dérivable sur $I$, on suppose que $\exists K \geq 0; |f'(t)| \leq K$. Alors $\forall (x,y) \in I^{2}, |f(y)-f(x)|\leq K|y-x|$
### Fonctions de classe $C^{1}, C^{p}, C^{\infty}$ 
- Une fonction est de classe $C^{1}$ sur $I$ si $f$ est dérivable et $f'$ est continue sur $I$.
- Une fonction est de classe $C^{p}$ sur $I$ si $f$ est $p$ fois dérivable et $f^{(p)}$  continue sur $I$. 
#### Formule de Leibniz 
Soit $f$ et $g$ définies et dérivables jusqu'à l'ordre $n$. $\forall n \in \mathbb{N}$ :
$\displaystyle (fg)^{(n)}= \sum_{k=0}^{n} \binom{n}{k} f^{(k)}g^{(n-k)}=\sum_{k=0}^{n} \binom{n}{k} f^{(n-k)}g^{(k)}$ 
- Similaire à la [[Sommes#Formules du binôme de Newton|Formules du binôme de Newton]].  
### Théorème de la limite de la dérive 
- Si $f$ continue en $I$ et si $f'$ admet une limite finie en $a$, alors $f$ est dérivable en $a$ et $\displaystyle f'(a)=l=\lim_{x \to a}f'(x)$. $f'$ est alors [[Limites et continuité#Continuité et prolongement par continuité|continue]] en $a$.  
- Si $f'$ admet un limite infinie en $a$, alors $f$ n'est pas dérivable en $a$  