11- 
a- On connais $T_{n}(x)= 2^{n+1} \prod_{k=1}^{n} (x-x_{k)}$
On commence a dériver :
$$\begin{align*} (\prod_{k=1}^{n}(x-x_{k}))'&=1(x-x_{2}) \ldots(x-x_{n})+(x-x_{1})1(x-x_{3})\ldots(x-x_{n})+\ldots \\ &= \frac{\prod_{k=1}^{n}(x-x_{k})}{x-x_{1}} + \frac{\prod_{k=1}^{n}(x-x_{k})}{x-x_{2}} + \ldots + \frac{\prod_{k=1}^{n}(x-x_{k})}{x-x_{n}}\end{align*}$$
Alors on en déduit :
$$\boxed{T_{n}'(x)=\sum_{k=1 }^{n}\frac{T_{n}(x)}{x-x_{k}}}$$

b- d'après la question 7, $T_{n}'(1)= n^{2}$
$$\begin{align*} \Leftrightarrow& \sum_{k=1}^{n} \frac{T_{n}(1)}{1-x_{k}}=n^{2} \\ \Leftrightarrow& \sum_{k=1}^{n} \frac{1}{1-x_{k}}=n^{2} \end{align*}$$
$$\Leftrightarrow \boxed{\sum_{k=1}^{n} \frac{1}{1-\cos(\frac{2k-1}{2n} \pi)}=n^{2}}$$

c- On a $\cos(2x)=1-2\sin^{2}(x)$    Soit $x=\frac{\theta}{2}$
Alors $\cos(\theta)-1=-2\sin^{2}(\frac{\theta}{2})$
$$\Leftrightarrow \boxed{1-\cos(\theta)=2\sin^{2}(\frac{\theta}{2})}$$

On a aussi $\sin^{2}(\theta)+\cos^{2}(\theta)=1$
$$\Leftrightarrow 1+ \frac{\cos^{2}(\theta)}{\sin^{2}(\theta)}= \frac{1}{\sin^{2}(\theta)}$$ 
$$\Leftrightarrow \boxed{1+\frac{1}{\tan^{2}(\theta)}=\frac{1}{\sin^{2}(\theta)}}$$

d- Alors on peut avoir
$$\begin{align*} &\sum_{k=1}^{n} \frac{1}{1-\cos(\frac{2k-1}{2n} \pi)}=n^{2} \\ \Leftrightarrow& \sum_{k=1}^{n} \frac{1}{2\sin^{2}(\frac{2k-1}{4n} \pi)}=n^{2} \end{align*}$$
$$\Leftrightarrow \boxed{\sum_{k=1}^{n} \frac{1}{\sin^{2}(\frac{2k-1}{4n} \pi)}=2n^{2}}$$ 
Si on remplace encore on a  
$$\sum_{k=1}^{n} \frac{1}{\tan^{2}(\frac{2k-1}{4n} \pi)}+1=2n^{2}$$
$$\Leftrightarrow \boxed{\sum_{k=1}^{n} \frac{1}{\tan^{2}(\frac{2k-1}{4n} \pi)}=2n^{2}-n}$$

12- Par propriété, $\forall x \in [0, \frac{\pi}{2}[$, On a $\sin(x) \leq x$ 

On cherche quand $\tan(x) \geq x \Leftrightarrow x-\tan(x) \leq 0$
Alors on a la fonction difference : $g(x)=x-\tan(x)$ définie et dérivable sur $[0, \frac{\pi}{2}[$
$g'(x)=1-1-\tan^{2}(x)=\tan^{2}(x)$ 
Or $\tan(x) \geq 0$ sur $[0, \frac{\pi}{2}[$
****Tableau****

Alors $\forall x \in [0, \frac{\pi}{2}[$,   $x-\tan(x) \leq$
On en déduit que $\boxed{\sin(x) \leq x \leq \tan(x)}$

b- 
$$\begin{align*} &\sin(x) \leq x \leq \tan(x) \\ \Rightarrow& \frac{1}{\tan(x)} \leq \frac{1}{x} \leq \frac{1}{\sin(x)} \\ \Rightarrow& \frac{1}{\tan^{2}(x)} \leq \frac{1}{x^{2}} \leq \frac{1}{\sin^{2}(x)} \\ \Rightarrow& \sum_{k=1}^{n} \frac{1}{\tan^{2}(x)} \leq \sum_{k=1}^{n} \frac{1}{x^{2}} \leq \sum_{k=1}^{n} \frac{1}{\sin^{2}(x)} \quad \text{Soit  } x=\frac{2k-1}{4n} \pi)\\ \Rightarrow& \sum_{k=1}^{n} \frac{1}{\tan^{2}(\frac{2k-1}{4n} \pi)} \leq \sum_{k=1}^{n} \frac{1}{(\frac{2k-1}{4n} \pi)^{2}} \leq \sum_{k=1}^{n} \frac{1}{\sin^{2}(\frac{2k-1}{4n} \pi)}   \end{align*}$$
$$\Rightarrow \boxed{2n^{2}-n \leq \sum_{k=1}^{n} \frac{1}{(\frac{2k-1}{4n} \pi)^{2}} \leq 2n^{2}}$$
$$\begin{align*} \Rightarrow& 2n^{2}-n \leq \sum_{k=1}^{n} \frac{1}{(2k-1)^{2}(\frac{\pi}{4n})^{2}} \leq 2n^{2} \\ \Rightarrow& 2n^{2}-n \leq \Big( \frac{4n}{\pi}\Big)^{2} \sum_{k=1}^{n} \frac{1}{(2k-1)^{2}} \leq 2n^{2} \end{align*}$$
$$\Rightarrow \boxed{\frac{\pi^{2}}{8}- \frac{\pi^{2}}{16n} \leq \sum_{k=1}^{n}  \frac{1}{(2k-1)^{2}} \leq \frac{pi^{2}}{8}}$$

c- Or $\begin{align*} \lim_{n \to +\infty}\frac{\pi^{2}}{8}- \frac{\pi^{2}}{16n}=\frac{\pi^{2}}{8} \end{align*}$

D'après le théorème d'éncadrement, $\forall n \in \mathbb{N}^{*}$ 
$$\boxed{\lim_{n \to +\infty}I_{n}=\frac{\pi^{2}}{8}}$$

**Exercice 2:**
1- On pose $\begin{align*} F=\frac{3X^{2}-1}{(X-1)^{2}X^2 (X+1)^{2}} \end{align*}$ 
Soit $B=(X-1)^{2}X^2 (X+1)^{2}$ de racines $1,-1,0$ tous doubles
Par propriété, il existent des uniques $(a,b,c)\in \mathbb{R}$ tel que 
$$F=\frac{a}{X^{2}} + \frac{b}{(X-1)^{2}} + \frac{c}{(X+1)^{2}}$$
On a donc
$$\frac{a}{X^{2}} + \frac{b}{(X-1)^{2}} + \frac{c}{(X+1)^{2}}=\frac{3X^{2}-1}{(X-1)^{2}X^2 (X+1)^{2}}$$

On cherche $a$ :
$$a+ \frac{bX^{2}}{(X-1)^{2}} +\frac{cX^{2}}{(X+1)^{2}} =\frac{3X^{2}-1}{(X-1)^{2} (X+1)^{2}}$$
soit $X=0$
$$a=\frac{-1}{(-1)^{2} (1)^{2}}=-1$$

On cherche $b$ :
$$\frac{a(X-1)^{2}}{X^{2}} + b + \frac{c(X-1)^{2}}{(X+1)^{2}}=\frac{3X^{2}-1}{X^2 (X+1)^{2}}$$
Soit $X=1$
$$b=\frac{3-1}{4}=\frac{1}{2}$$

On cherche $c$ :
$$\frac{a(X+1)^{2}}{X^{2}} + \frac{b(X+1)^{2}}{(X-1)^{2}} + c=\frac{3X^{2}-1}{(X-1)^{2}X^2 }$$
Soit $x=-1$
$$c=\frac{2}{4}=\frac{1}{2}$$

Alors $\boxed{F=-\frac{1}{X^{2}} + \frac{1}{2}\frac{1}{(X-1)^{2}} + \frac{1}{2}\frac{1}{(X+1)^{2}}}$

 2- on a donc
$$\begin{align*} S_{n}= \sum_{k=2}^{n} u_{k} = \sum_{k=2}^{n} -\frac{1}{k^{2}} + \frac{1}{2}\frac{1}{(k-1)^{2}} + \frac{1}{2}\frac{1}{(k+1)^{2}} \end{align*}$$
 On repère une somme télescopique, après simplifier on trouve :
 $$\boxed{S_{n}=- \frac{1}{2n^{2}}+ \frac{1}{2(n+1)^{2}}+ \frac{3}{8}}$$

3- $\begin{align*} \lim_{n \to +\infty}- \frac{1}{2n^{2}}+ \frac{1}{2(n+1)^{2}}+ \frac{3}{8}= \frac{3}{8} \end{align*}$
Alors $\boxed{\lim_{n \to +\infty} S_{n}=\frac{3}{8}=l}$

4- $S_{n}-l=\frac{1}{2n^{2}}+ \frac{1}{2(n+1)^{2}}=\frac{-4n+2}{4n^{4}+8n^{3}+4n^{2}}$
On pose comme tentative de équivalent simple $g_{n}=\frac{-1}{n^{3}}$
$$\frac{S_{n}-l}{g_{n}} =\frac{4n^{4}-n^{3}}{4n^{4}+8n^{3}+4n^{2}}= \frac{4n^{2}-n}{4n^{2}+8n+4}=\frac{4- \frac{1}{n}}{4+ \frac{8}{n}+ \frac{4}{n^{2}}}$$
On a donc $\begin{align*} \lim_{n \to +\infty} \frac{S_{n}-l}{g_{n}}=1 \end{align*}$
On a bien
$$\boxed{S_{n}-l \sim \frac{-1}{n^{3}}}$$