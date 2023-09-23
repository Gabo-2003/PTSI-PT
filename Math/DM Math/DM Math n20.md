1-
a- D'apres les relations d'Euler, on a :
$$\begin{align*} \cos(a)\cos(b)&= \frac{e^{ia}+e^{-ia}}{2} \times \frac{e^{ib}+e^{-ib}}{2} = \frac{1}{4}(e^{i(a+b)}+e^{i(a-b)}+e^{-i(a-b)}+e^{-i(a+b)}) \\ &= \frac{1}{2}(\frac{e^{i(a+b)}+e^{-i(a+b)}}{2} + \frac{e^{i(a-b)}+e^{-i(a-b)}}{2}) \\ &= \frac{1}{2}(\cos(a+b)+\cos(a-b)) \end{align*}$$
On a bien démontre que, $\forall a,b \in \mathbb{R}$
$$\boxed{\cos(a)\cos(b)=\frac{1}{2}(\cos(a+b)+\cos(a-b))}$$

b- d'après la formule precedent :
$$\begin{align*} &\cos(x)\cos((n+1)x)=\frac{1}{2}(\cos(x+(n+1)x)+\cos(x-(n+1)x)) \\ \Leftrightarrow& 2\cos(x)\cos((n+1)x) = \cos((n+2)x)+\cos(-nx)=cos((n+2)x)+cos(nx) \end{align*}$$
On a bien démontre que $\forall n \in \mathbb{N}, \forall x \in \mathbb{R}$
$$\boxed{2\cos(x)\cos((n+1)x)=cos((n+2)x)+cos(nx)}$$

2- 
$T_{0}=1$
$T_{1}=X$
$T_{2}=2X(X)-1=2X^{2}-1$
$T_{3}=2X(2X^{2}-1)-X=4X^{3}-3X$
$T_{4}=2X(4X^{3}-3X)-2X^{2}+1=8X^4-8X^{2}+1$

Il semble que $\forall n>0$,  $\boxed{deg(T_{n})=2^{n-1}}$
et que $\boxed{coeff(Tn)=2^{n-1}}$ 

3- On va le démontrer par recurrence
**Initialization :**
pour $n=0$,  $T_{0}=1$ ça marche
pour $n=1$,  $T_{1}=X$ ça marche

**Hérédité :** On suppose que la propriété est vrai pour le rang $n$ et $n+1$
On veut le démontrer pour le rang $n+1$

$$T_{n+2} = 2XT_{n+1} -T_{n}$$
Donc $deg(T_{n+2}) = 1+ deg(T_{n+1})=1+n+1=n+2$
et $coeff(T_{n+2})= 2 \times coeff(T_{n+1})=2 \times 2^{n}=2^{n+1}$

**Conclusion :** On a bien  démontre que $\forall n>0$
$\boxed{deg(T_{n})=2^{n-1}}$ et $\boxed{coeff(Tn)=2^{n-1}}$

4- On veut montrer par recurrence que $\forall n \in \mathbb{N}$, $\forall x \in \mathbb{R}$
$$T_{n}=(-1)^{n}T_{n}(x)$$

**Initialisation :**
$n=0$    $T_{0}(-X)=1=T_{0}$ 
$n=1$   $T_{1}(-X)=-X=-T_{1}(-X)$ ça marche

**Hérédité :** On suppose la propriété est vrai pour les rangs $n$ et $n+1$ 
On veut le démontrer pour $n+2$

$$\begin{align*} T_{n+2}(-X) =& -2XT_{n+1}(-X) -T_{n}(-X) \\ =&-2X(-1)^{n+1}T_{n+1}(X)-(-1)^{n}T_{n}(X) \\ =& (-1)^{n}(2XT_{n+1}(X)-T_{n}(X)) \\ =& (-1)^{n}T_{n+2}(X) = (-1)^{n+2}T_{n+2}(X) \end{align*}$$

**Conclusion :** On a bien démontre que $\forall n \in \mathbb{N}$, $\forall x \in \mathbb{R}$
$$\boxed{T_{n}=(-1)^{n}T_{n}(x)}$$

5- On veut montrer par recurrence que $\forall n \in \mathbb{N}$, $\forall x \in \mathbb{R}$ 
$$T_{n}(\cos(x))=\cos(nx)$$

**Initialisation :** 
$n=0$    $T_{0}(\cos(x))=1=\cos(0)$
$n=1$    $T_{1}(\cos(x))=\cos(x)$
O.K
**Hérédité :** On suppose que la proposition est vraie pour les rangs $n$ et $n+1$.
On veut le démontrer pour $n+2$

$$\begin{align*} T_{n+2}\cos(x) &= 2\cos(x)T_{n+1}(\cos(x))-T_{n}(\cos(x)) \\ &= 2\cos(x)(\cos((n+1)x))-\cos(nx) \\ &= \cos((n+2)x) \text{  (D'après la question 1-b)  } \end{align*}$$

**Conclusion :** On a bien démontre que $\forall n \in \mathbb{N}$, $\forall x \in \mathbb{R}$
$$\boxed{T_{n}(\cos(x))=\cos(nx)}$$

6- 
On sait que $\cos(x)=1 \Leftrightarrow x=2k \pi\:, k \in \mathbb{Z}$
Alors $T_{n}(\cos(x))=\cos(nx)$
$\Rightarrow \boxed{T_{n}(1)= cos(2k \pi)=1}$

On sait que $\cos(x)=0 \Leftrightarrow x = \frac{\pi}{2}+k \pi$
Alors $T_{n}(\cos(x))=\cos(nx)$
$\Rightarrow T_{n}(0)=cos(n(\frac{\pi}{2}+k \pi))$

7- D'apres la définition du nombre dérivé, on a :
$$\begin{align*} T_{n}'(1)&=\lim_{\cos(x) \to 1} \frac{T_{n}(\cos(x))-T_{n}(1)}{\cos(x)-1} \\ &=  \lim_{\cos(x) \to 1} \frac{\cos(nx)-1}{\cos(x)-1} \end{align*}$$
On fait une $DL_{1}(1)$ et on trouve 
$$T_{n}'(1)=\frac{1-n^{2}x^{2}-1}{1-x^{2}-1}=n^{2}$$
$$\boxed{\Leftrightarrow T_{n}'(1)=n^{2}}$$


8- Démontrer que $T_{n}$ solution de l'équation différentielle : $(1-X^{2})T_{n}''-XT_{n}'+n^{2}T_{n}=0$

On a $T_{n}(\cos(x))=\cos(nx)$
$$\begin{align*}  \Rightarrow(T_{n}(\cos(x)))'&= (\cos(nx))' \\ \Leftrightarrow -\sin(x)T_{n}'(\cos(x))&=-n\sin(nx)  \end{align*}$$

et encore: 
$$\begin{align*} (\sin(x)T_{n}'(\cos(x)))'&=(-n\sin(nx))' \\ -\cos(x)T_{n}'(\cos(x))+ \sin(x)^{2}T_{n}''(\cos(x))&=n^{2}\cos(x)  \end{align*}$$
$$\boxed{\Leftrightarrow (1-\cos(x)^{2})T_{n}''(\cos(x))-\cos(x)T_{n}'(\cos(x))+n^{2}\cos(x)=0}$$

9-
```Python 
import numpy as np

def T(n):
    if n == 0:
        return [1]
    elif n == 1:
        return [0,1]

    t0 = np.array([1,0,0])
    t1 = np.array([0,1,0])
    tn = np.array([0,0,0])
    for i in range(n-1):
        for j in range(len(tn)-1):
            tn[j+1] = 2*t1[j]
            
        tn[0]=0
        tn = tn - t0
        tn =np.append(tn,[0])
        t0 = np.append(t1,[0])
        t1 = np.copy(tn)

    tn=np.delete(tn,-1)
    return tn
  
print(T(4))
>>>> [ 1  0 -8  0  8]
```

10- on suppose $n \geq 1$
a-On pose $x_{k}=\cos(\frac{2k-1}{2n}\pi)\:, k \in \mathbb{Z}$

$$T_{n}(x_{k})=T_{n}\left(\cos\left(\frac{2k-1}{2n}\pi\right)\right)= \cos(n\frac{2k-1}{2n}\pi)=\cos(\pi k - \frac{\pi}{2})$$
$$\boxed{T_{n}(x_{k})=0}$$