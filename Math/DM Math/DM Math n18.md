**Exercice 1 :**
On définie $f(x)=\frac{1}{e^{-2x}-1}+ \frac{1}{\sin(2x)}$ et $g(x)=(x^{2}+1)\ln(\frac{x+1}{x})+ \frac{x^{2}+x-1}{x+1}$

1- $f$ définie sur $\mathbb{R}^{*}$

a- On cherche le $DL_{5}(0)$ de $e^{-2x}$ 
On a $e^{u} \underset{0} = 1+u + \frac{u^{2}}{2!} + \frac{u^{3}}{3!} + \frac{u^{4}}{4!} + \frac{u^{5}}{5!} + u^{5}\varepsilon(n)$
Soit $u=-2x$,     $\begin{align*} &u \longrightarrow 0\\ &x \rightarrow 0 \end{align*}$
Alors  $e^{-2x}=1-2x + \frac{4x^{2}}{2} -\frac{8x^{3}}{6} + \frac{16x^{4}}{24} - \frac{32x^{5}}{120} +x^{5}\varepsilon(x)$ 
$\boxed{e^{-2x}=1-2x+2x^{2} - \frac{4}{3}x^{3} + \frac{2}{3} x^{4} - \frac{4}{15}x^{5} +x^{5} \varepsilon(x)}$

On cherche le $DL_{5}(0)$ de $\sin(2x)$ 
On a $\sin(u)=u- \frac{u^{3}}{3!} + \frac{u^{5}}{5!} +u^{5}\varepsilon(x)$
Soit $u=2x$,     $\begin{align*} &u \longrightarrow 0\\ &x \rightarrow 0 \end{align*}$  
Alors  $\sin(2x) = 2x- \frac{8x^{3}}{6} + \frac{32x^{5}}{120} +x^{5}\varepsilon(x)$
$\boxed{\sin(2x) = 2x - \frac{4}{3}x^{3} + \frac{4}{15}x^{5}+ x^{5}\varepsilon(x)}$

b- Soit $f=\frac{\sin(2x)+e^{-2x}-1}{(e^{-2x}-1)\sin(2x)}$, alors :
$$\begin{align*} f(x)&= \frac{2x - \frac{4}{3}x^{3}+ \frac{4}{15}x^{5} +1 - 2x+2x^{2}- \frac{4}{3}x^{3} + \frac{2}{3}x^{4} - \frac{4}{15}x^{3} -1 +x^{5}\varepsilon(x)}{(1-2x+2x^{2}- \frac{4}{3}x^{3}+ \frac{2}{3}x^{4}- \frac{4}{15}x^{5}-1)(2x-\frac{4}{3}x^{3}+ \frac{4}{15}x^{5})+ x^{5}\varepsilon(x)} \\ &=\frac{\frac{2}{3} (3-4x+x^{2}+x^{3}\varepsilon(x))}{\frac{4}{9}(-9+9x-3x^{3}+4x^{4}+x^{4}\varepsilon(x))} = \frac{9-12x+3x^{2}+x^{3}\varepsilon(x)}{-18+18x-6x^{3}+8x^{4}+x^{4}\varepsilon(x)}\\&= (9-12x+3x^{2}+x^{3}\varepsilon(x)) \times -\frac{1}{18} \times \frac{1}{1-x+ \frac{1}{3}x^{3}- \frac{4}{9}x^{4}+ x^{4} \varepsilon(x)} \end{align*}$$

On sait que $\frac{1}{1-u}=1+u+u\;\varepsilon(u)$
Soit $u=x- \frac{1}{3}x^{3}- \frac{4}{9}x^{4} +x^{4}\varepsilon(x)$
Alors $f(x)=(9-12x+3x^{2}+x^{3}\varepsilon(x)) \times -\frac{1}{18} \times (1+x- \frac{1}{3}x^{3})$
$$\boxed{f(x)=- \frac{1}{2} + \frac{1}{6}x+ \frac{1}{2}x^{2}+ x^3 \varepsilon(x)}$$

c- Alors par troncature $f$ admet une $DL_{0}(0)$
Donc $f$ admet un limite en $0$ , $\lim_{x \to 0}f(x)=- \frac{1}{2}$ donc on peut prolonger $f$ par continuité:
$$\boxed{\tilde{f}(x): \mathbb{R}^{*} \cup \{0\} \longrightarrow \mathbb{R}; x \mapsto \begin{cases} f(x) \text{  si  } x \neq 0  \\ - \frac{1}{2} \text{  si  } x=0\end{cases}}$$

Aussi $\boxed{f \text{  admet  } DL_{1}(0) \text{  donc  } f \text{  est dérivable en  } 0}$

On en déduit aussi l'équationde la tangente en $0$
$$\boxed{\Delta = - \frac{1}{2} + \frac{1}{6}x}$$

2- 
a- On cherche l'ensemble de definition de $g$
- $\ln$ définie sur $\mathbb{R}^{*+}$
- $\frac{1}{x+1}$ définie pour $x \neq -1$
alors on cherche quand $\frac{x+1}{x}>0$
$\Leftrightarrow \begin{cases}x>-1  \\ x>0\end{cases} \text{  ou  } \begin{cases} x<-1  \\ x<0\end{cases}$
alors $\boxed{g \text{  définie sur } ]-\infty,-1[ \cup ]0, +\infty[}$

b- 

c- Calculer le $DL_{3}(0)$ de $(1+h^{2})\ln(1+h)$
$$(1+h^{2})\ln(1+h) = (1+h^{2})(h- \frac{1}{2}h^{2}+ \frac{1}{3}h^{3} + h^{3}\varepsilon(h))$$
$$\boxed{(1+h^{2})\ln(1+h) = h - \frac{1}{2}h^{2}+ \frac{4}{3}h^{3}+ h^{3}\varepsilon(h)}$$

Calculer le $DL_{3}(0)$ de $\frac{1+h-h^{2}}{1+h}$
Or $\frac{1}{1-u}=1+u+u^{2}+u^{3} +u^{3}\varepsilon(u)$ Soit $u=-h$ 
On a $\frac{1+h-h^{2}}{1+h}=(1+h-h^{2})(1-h+h^{2}-h^{3})+h^{3}\varepsilon(h)$
$$\boxed{\frac{1+h-h^{2}}{1+h}=1-h^{2}+h^{3}+ h^{3}\varepsilon(h)}$$





**Exercice 2 :**
1- Montrer que $x_{n}$ est l'unique solution à l'équation $\ln(x)=n-x$ dans $]0, +\infty[$

Posons la fonction $h(x)=\ln(x)+x$ définie et dérivable sur $]0, +\infty[$ 
On cherche quand $h(x)=n$,    $n\geq1$

$h'(x)=\frac{1}{x}+1$ , positive por tout $x$

TABLEAU

$$\lim_{x\to0^{+}} h(x)=-\infty \quad \text{et} \quad \lim_{x \to +\infty} h(x)=+\infty$$
Or $h$ continue et monotone sur $]0, +\infty[$ et $n \in ]- \infty, +\infty[$
$$\boxed{\text{D'après le corollaire du TVI, l'équation "}h(x)=n \text{" admet une unique solution que on nom} \; x_{n}}$$

2- On a $h(x)=\ln(x)+x$
$x_{n}$ tel que $h(x_{n})=n$ 
$x_{n+1}$ tel que $h(x_{n+1} )=n+1$
$$\begin{align*} \text{Or  } n&<n+1 \\ \Leftrightarrow& h(x_{n})<h(x_{n+1}) \\ \Rightarrow& x_{n}<x_{n+1} \text{  (car h continue et monotone)} \end{align*}$$
$\boxed{\text{Alors  }x_{n} \text{  strictement croissante sur } ]0, + \infty[}$

3- On sait que $\forall x>-1$,   $\ln(x+1)\leq x$
soit $X = x+1$,   $\ln(X) \leq X-1 <X$
alors $\ln(X)<X$
On a donc :
$$\begin{align*} &ln(x_{n})<x_{n} \\ \Leftrightarrow& n- x_{n} < x_{n} \\ \Leftrightarrow& \frac{n}{2}<x_{n} \end{align*}$$

Or $\lim_{n \to +\infty}\frac{n}{2}=+\infty$
Par propriété $\boxed{lim_{n \to +\infty}x_{n}=+\infty}$

4- On cherche un équivalente à $x_{n}$ lorsque $n$ tend vers l'infinie
Soit $x_{n}=n-\ln(x_{n})$
On a:
$\lim_{n \to +\infty} \frac{n-\ln(x_{n})}{n} = \lim_{n \to +\infty} 1- \frac{\ln(x_{n})}{n}$

On étudie $\lim_{n \to +\infty}\frac{\ln(x_{n})}{n}$

$\begin{align*} \text{On a  } 0&<\ln(x_{n}) \\ \Leftrightarrow x_{n}&<n \end{align*}$
$\text{Et  } \frac{n}{2}<x_{n}$
Alors:
$\begin{align*} &\frac{n}{2}<x_{n}<n \\ \Leftrightarrow& \frac{\ln(\frac{n}{2})}{n}<\frac{\ln(x_{n})}{n} < \frac{\ln(n)}{n} \\ \Leftrightarrow& \frac{\ln(n)}{n}- \frac{\ln(2)}{n}<\frac{\ln(x_{n})}{n} < \frac{\ln(n)}{n} \end{align*}$
Or $\lim_{n \to +\infty}\frac{\ln(n)}{n}=0 \text{  (croissance compare)}$
et $\lim_{n \to +\infty} -\frac{\ln(2)}{n}=0$

Alors, d'après le théorème de croissance comparé :
$\lim_{n \to +\infty} \frac{\ln(x_{n})}{n}=$

Alors $\lim_{n \to +\infty} 1- \frac{\ln(x_{n})}{n}=1$
donc  $\boxed{\lim_{n \to +\infty} \frac{x_{n}}{n}=1 \Leftrightarrow x_{n} \underset{+\infty} \sim n \quad \text{i.e  } x_{n} \text{  equivalent à }n \text{  en   }+\infty}$

5- Soit $y_{n}=n- x_{n}$, on cherche un équivalente en $+\infty$

$y_{n}=n- x_{n}=\ln(x_{n})$

$\begin{align*} &\lim_{n \to +\infty} \frac{\ln(x_{n})}{\ln(n)} \text{ or  }x_{n} \underset{+\infty} \sim n \\ \Leftrightarrow& \lim_{n \to +\infty} \frac{\ln(n)}{\ln(n)}=1\end{align*}$
alors $\boxed{\ln(x_{n}) \underset{+\infty}\sim \ln(n)}$

6- On en déduit que $y_{n} \underset{+\infty} = \ln(n) + \ln(n) \varepsilon(n)$
$\Leftrightarrow \boxed{x_{n}\underset{+\infty} = n- \ln(n)+\ln(n) \varepsilon(n)}$
