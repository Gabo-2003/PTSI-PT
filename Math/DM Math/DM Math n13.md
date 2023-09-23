Exercice 1: 

1- Première calcule de $M^{n}$

a- Vérifier que $M^{2}+6M+8I=0$
On commence par calculer
$$M^{2}=\begin{pmatrix} -5&3&-3 \\ -2&0&-2  \\ -1&1&-3\end{pmatrix} \begin{pmatrix} -5&3&-3 \\ -2&0&-2  \\ -1&1&-3\end{pmatrix} = \begin{pmatrix} 22&-18&18 \\ 12&-8&12  \\ 6&-6&10\end{pmatrix}$$
On a donc: 
$$\begin{split} M^{2}+6M+8I=& \begin{pmatrix} 22&-18&18 \\ 12&-8&12  \\ 6&-6&10\end{pmatrix}+6\begin{pmatrix} -5&3&-3 \\ -2&0&-2  \\ -1&1&-3\end{pmatrix} + 8\begin{pmatrix} 1&0&0 \\ 0&1&0  \\ 0&0&1\end{pmatrix} \\ =&  \begin{pmatrix} -8&0&0 \\ 0&-8&0 \\ 0&0&-8\end{pmatrix} + \begin{pmatrix} 8&0&0 \\ 0&8&0 \\ 0&0&8\end{pmatrix} = \begin{pmatrix} 0&0&0 \\ 0&0&0 \\ 0&0&0\end{pmatrix} \end{split}$$
Donc: $\boxed{M^{2}+6M+8I=0}$

b- On veut montrer par récurrence qu'il existe un couple 
$(an,bn) \in \mathbb{R}^{2}$$  ;  $M^{n}= anM +bnI$   $\forall n\in \mathbb{N}$ 

**Initialisation:**

pour $n=0$ , $a_{0} = 0$  et $b_{0} = 1$

$M^{0}=0 \times M + 1\times I=I$ ça marche

mais encore pour: $n=1$ , $a_{1} = 1$ et $b_{1} = 0$
$M^{1}=1 \times M + 0\times I=M$ ça marche

**Initialisation:**
pour $n=0$ , $a_{0} = 0$  et $b_{0} = 1$
$M^{0}=0 \times M + 1\times I=I$ ça marche

mais encore pour: $n=1$ , $a_{1} = 1$ et $b_{1} = 0$
$M^{1}=1 \times M + 0\times I=M$ ça marche

**Hérédité:** Supposons que $\forall n\in \mathbb{N}$ il existe  $(an,bn) \in \mathbb{R}^{2} ; M^{n}= anM +bnI$. 
On veut démontrer qu'il existe $(a_{n+1},b_{n+1}) \in \mathbb{R}^{2} ; M^{n+1}= a_{n+1}M +b_{n+1}I$ $\forall n\in \mathbb{N}$

$\begin{align*} M^{n+1} &= M^{n} \times M =(anM +bnI)M \\ &=anM^{2} +bnIM = an(-6M - 8I)+bnIM \quad \text{On remplace par l'expretion trouve dans a.} \\  & =(-6an + bn)M +(-8an)I \end{align*}$

Donc $(a_{n+1})$ et $(b_{n+1})$ existent tel que:
$a_{n+1} = -6an + bn$
et
$b_{n+1} = -8an$

**Conclusion:** Il existe un couple $(an,bn) \in \mathbb{R}^{2} ; \boxed{M^{n}= anM +bnI}$   $\forall n\in \mathbb{N}$ 

c- On a $a_{n+2} = -6a_{n+1} +b_{n+1} = -6a_{n+1} -8an$

On a donc une $SRL_{2}$
Equation caractéristique:  $\text{(k)} \hspace{6pt} r^{2}+6r+8=0$

avec $\Delta = 36-4(8) = 4$  et  $\begin{align*} r1&=\frac{-6+2}{2}=-2 \\ r2&= \frac{-6-2}{2}=-4 \end{align*}$

Donc $an =\lambda r1^{n}+ \mu r2^{n}$
et $\begin{align*} &\begin{cases} \lambda+\mu=a_{0} \\ \lambda r1 +\mu r2 = a_{1} \end{cases}  \Leftrightarrow \begin{cases} \lambda+\mu=0 \\ \lambda r1 +\mu r2 = 1 \end{cases}  \Leftrightarrow \begin{cases} \lambda=-\mu \\ 2 \mu-4\mu=1 \end{cases} \\  \Leftrightarrow &\begin{cases} \lambda=\frac{1}{2} \\ \mu=\frac{-1}{2} \end{cases} \end{align*}$

alors
$\begin{align*} &an = \frac{1}{2}(-2)^{n} - \frac{1}{2}(-4)^{n}\\ &\boxed{an=\frac{1}{2}((-2)^{n} -(-4)^{n})} \end{align*}$

d- Or $b_{n+1} = -8an$
$\Leftrightarrow bn = -8a_{n-1} = -4((-2)^{n-1} -(-4)^{n-1}) =-4\left(\frac{(-2)^{n}}{-2} - \frac{(-4)^{n}}{-4}\right)$
$\Leftrightarrow \boxed{bn=2(-2)^{n}-(-4)^{n}}$

e- $M^{n}= anM +bnI$
On commence par calculer
$\begin{align*} anM &= \frac{1}{2}((-2)^{n} -(-4)^{n})\begin{pmatrix} -5&3&-3 \\ -2&0&-2  \\ -1&1&-3\end{pmatrix}\\ &=\frac{1}{2}\begin{pmatrix} -5((-2)^{n} -(-4)^{n})&3((-2)^{n} -(-4)^{n})&-3((-2)^{n} -(-4)^{n}) \\ -2((-2)^{n} -(-4)^{n})&0&-2((-2)^{n} -(-4)^{n})  \\ -1((-2)^{n} -(-4)^{n})&1((-2)^{n} -(-4)^{n})&-3((-2)^{n} -(-4)^{n})\end{pmatrix} \end{align*}$
Après on calcule
$bnI=(2(-2)^{n}-(-4)^{n})I=\begin{pmatrix} 2(-2)^{n}-(-4)^{n}&0&0 \\ 0&2(-2)^{n}-(-4)^{n}&0 \\ 0&0&2(-2)^{n}-(-4)^{n}\end{pmatrix}$

Donc $\boxed{M^{n}=\frac{1}{2}\begin{pmatrix} -3((-2)^{n} -(-4)^{n})&3((-2)^{n} -(-4)^{n})&-3((-2)^{n} -(-4)^{n}) \\ -2((-2)^{n} -(-4)^{n})&2(-2)^{n}-(-4)^{n}&-2((-2)^{n} -(-4)^{n})  \\ -1((-2)^{n} -(-4)^{n})&1((-2)^{n} -(-4)^{n})&-1((-2)^{n} -(-4)^{n})\end{pmatrix}}$ 


2- Deuxième calcule

a- 
$A^{2}=\begin{pmatrix} -1 & 3 & -3 \\ -2 & 4 & -2 \\ -1 & 1 & 1 \end{pmatrix} \begin{pmatrix} -1 & 3 & -3 \\ -2 & 4 & -2 \\ -1 & 1 & 1 \end{pmatrix} = \begin{pmatrix} -2 & 6 & -6 \\ 4 & 8 & -4 \\ -2 & 2 & 2 \end{pmatrix}$

$B^{2}= \begin{pmatrix} -3 & 3 & -3 \\ -2 & 2 & -2 \\ -1 & 1 & -1 \end{pmatrix} \begin{pmatrix} -3 & 3 & -3 \\ -2 & 2 & -2 \\ -1 & 1 & -1 \end{pmatrix} = \begin{pmatrix} 6 & -6 & 6 \\ 4 & -4 & 4 \\ 2 & -2 & 2 \end{pmatrix}$

Il semble que $\boxed{A^{n}=2^{n-1}A}$ et $\boxed{B^{n}=(-2)^{n-1}B}$   $\forall n>0$

On le démontre par récurrence.
**Initialisation:** 
pour $n=1$, 
$A^{1}=2^{1-1}A =A$ 
$B^{1}=(-2)^{1-1}B =B$ ça marche.

**Hérédité:**
$\begin{split} A^{n+1} =& A^{n}\times A =(2^{n-1}A)\times A=2^{n-1}A^{2} \\ =& 2^{n-1}(2A)=2^{n}A \end{split}$

$\begin{split} B^{n+1} =& B^{n}\times B =((-2)^{n-1}B)\times B=(-2)^{n-1}B^{2} \\ =& (-2)^{n-1}(-2B)=(-2)^{n}B \end{split}$

Donc, $\forall n>1$, $B^{n+1}=(-2)^{n}B$  et  $A^{n+1}=2^{n}A$ 

**Conclusion:** $\boxed{\forall n>0 \text{ , } A^{n}=2^{n-1}A \text{  et  } B^{n}=(-2)^{n-1}B}$   

b-
$M+4I = \begin{pmatrix} -5 & 3 & -3 \\ -2 & 0 & -2 \\ -1 & 1 & -3 \end{pmatrix}  \begin{pmatrix} 4 & 0 & 0 \\ 0 & 4 & 0 \\ 0 & 0 & 4 \end{pmatrix} = \begin{pmatrix} -1 & 3 & -3 \\ -2 & 4 & -2 \\ -1 & 1 & 1 \end{pmatrix} =A$
Donc $\boxed{M+4I = A}$

$M+2I = \begin{pmatrix} -5 & 3 & -3 \\ -2 & 0 & -2 \\ -1 & 1 & -3 \end{pmatrix}  \begin{pmatrix} 2 & 0 & 0 \\ 0 & 2 & 0 \\ 0 & 0 & 2 \end{pmatrix} = \begin{pmatrix} -3 & 3 & -3 \\ -2 & 2 & -2 \\ -1 & 1 & -1 \end{pmatrix} =B$
Donc $\boxed{M+2I = B}$

On peut en déduire que:  $2I =B-M$     
or 
$\begin{split} &A = M+4I \\  \Leftrightarrow & M = A-4I =A-2(2I) =A-2(B-M) \\  \Leftrightarrow & \boxed{M = 2B-A} \end{split}$
Donc M est une combinaison linéaire de $A$ et $B$

c- On fait $M^{n} =( 2B-A)^{n}$, On cherche a utiliser le Binôme de Newton 

On vérifie que $2B \times-A = -A \times 2B$

$2B \times-A= 2 \begin{pmatrix} -3 & 3 & -3 \\ -2 & 2 & -2 \\ -1 & 1 & -1 \end{pmatrix} \times-\begin{pmatrix} -1 & 3 & -3 \\ -2 & 4 & -2 \\ -1 & 1 & 1 \end{pmatrix} = \begin{pmatrix} 0 & 0 & 0 \\ 0 & 0 & 0 \\ 0 & 0 & 0  \end{pmatrix}$

$-A \times 2B=-\begin{pmatrix} -1 & 3 & -3 \\ -2 & 4 & -2 \\ -1 & 1 & 1 \end{pmatrix} \times2 \begin{pmatrix} -3 & 3 & -3 \\ -2 & 2 & -2 \\ -1 & 1 & -1 \end{pmatrix} =\begin{pmatrix} 0 & 0 & 0 \\ 0 & 0 & 0 \\ 0 & 0 & 0  \end{pmatrix}$

ça marche, donc on peut utiliser le binôme de Newton:
$M^{n}=\sum\limits_{k=0}^{n} (2B)^{n-k}(-A)^{k}$
or $2B$ et $-A$ sont diviseurs de $0$. On a:
$M^{n}=(2B)^{n-0}(-A)^{0}+\begin{pmatrix} 0 & 0 & 0 \\ 0 & 0 & 0 \\ 0 & 0 & 0 \end{pmatrix} + \ldots + \binom{n}{n} (2B)^{n-n}(-A)^{n}$
De plus, on sait que: $A^{n}=2^{n-1}A$ et $B^{n}=2^{n-1}B$
Donc
$\begin{align*} &M^{n}=2^{n}\times(-2)^{n-1}B + (-1)^{n} \times 2^{n-1}A = \frac{2^{n}\times(-2)^{n}}{-2}B +  \frac{(-1)^{n}\times2^{n}}{2} A \\ &\boxed{M^{n} =\frac{1}{2}((-2)^{n}A -(-4)^{n}B)} \end{align*}$


3- Trosième calcule
a- Soit $P =  \begin{pmatrix} 3 & 1 & 0 \\ 2 & 1 & 1 \\ 1 & 0 & 1 \end{pmatrix}$ on veut démontrer que $P$ est inversible et trouver $P^{-1}$
On pose $PX = Y$ avec $X= \begin{pmatrix} x \\ y \\ z \end{pmatrix}$ et $Y = \begin{pmatrix} a  \\ b \\ c \end{pmatrix}$ 

$\begin{split} \Leftrightarrow & \begin{cases} 3x +y +0 =a \\ 2x +y+z=b \\ x+0+z=c \end{cases} \overset{L2 \leftarrow L2-L1} \Leftrightarrow \begin{cases} 3x+y+0=a \\ -x+0+z=b-a \\ x+0+z=c \end{cases} \overset{L2 \leftarrow L2-L3}  \Leftrightarrow \begin{cases} 3x+y+0=a \\ -2x+0+0=b-a-c \\ x+0+z=c \end{cases} \\[4mm] \overset{L1 \leftarrow L1+L3}  \Leftrightarrow  & \begin{cases} 4x+y+z=a+c \\ -2x+0+0=b-a-c \\ x+0+z=c\end{cases}  \overset{L2 \leftrightarrow L3}  \Leftrightarrow \begin{cases} 4x+y+z=a+c \\ x+0+z=c \\-2x+0+0=b-a-c \end{cases} \text{(Donc P est inversible)} \\[4mm] \Leftrightarrow & \begin{cases} y=a+c-4x-z = \frac{2a +2c-4a +4b-4c+a-b-c}{2} \\ z=c-x =\frac{2c-a-c+b}{2}  \\ x= \frac{b-a-c}{-2} \end{cases} \Leftrightarrow \begin{cases} y = \frac{-a+3b-3c}{2} \\ z=\frac{-a+3b-3c}{2}  \\ x= \frac{b-a-c}{-2} \end{cases}\end{split}$

Donc $\boxed{P^{-1}=  \begin{pmatrix} \frac{1}{2} & \frac{-1}{2} & \frac{1}{2} \\ \frac{-1}{2} & \frac{3}{2} & \frac{-3}{2} \\ \frac{-1}{2}  & \frac{1}{2} & \frac{1}{2} \end{pmatrix} =\frac{1}{2} \begin{pmatrix} 1 & -1 & 1 \\ -1 & 3 & -3  \\ -1 & 1 & 1 \end{pmatrix}}$

b- Calculer $D=P^{-1}MP$
On commence par calculer
$P^{-1}M=\frac{1}{2} \begin{pmatrix} 1 & -1 & 1 \\ -1 & 3 & -3  \\ -1 & 1 & 1 \end{pmatrix} \begin{pmatrix} -5&3&-3 \\ -2&0&-2  \\ -1&1&-3\end{pmatrix} =\frac{1}{2}  \begin{pmatrix} -4 & 4 & -4  \\ 2 & -6 & 6 \\ 2 & -2 & -2 \end{pmatrix} = \begin{pmatrix} -2 & 2 & -2  \\ 1 & -3 & 3 \\ 1 & -1 & -1\end{pmatrix}$
Après on calcule
$(P^{1}M)P= \begin{pmatrix} -2 & 2 & -2  \\ 1 & -3 & 3 \\ 1 & -1 & -1 \end{pmatrix} \begin{pmatrix} 3 & 1 & 0 \\ 2 & 1 & 1 \\ 1 & 0 & 1 \end{pmatrix} = \begin{pmatrix} -4  & 0 & 0  \\ 0 & -2 & 0 \\ 0 & 0 & -2 \end{pmatrix}$

Donc $D=\begin{pmatrix} -4  & 0 & 0  \\ 0 & -2 & 0 \\ 0 & 0 & -2 \end{pmatrix}$

Or $D^{2}= \begin{pmatrix} 16 & 0 & 0 \\ 0 & 4 & 0 \\ 0 & 0 & 4 \end{pmatrix}$ On peut en deduir que

$\boxed{D^{n}=\begin{pmatrix} (-4)^{n}  & 0 & 0  \\ 0 & (-2)^{n} & 0 \\ 0 & 0 & (-2)^{n} \end{pmatrix}}$

c- On a 
$\begin{split} &D=P^{-1}MP\\ \Leftrightarrow &PD=PP^{-1}MP\\ \Leftrightarrow &PDP^{-1}=MPP^{-1}\\ \Leftrightarrow &M=PDP^{-1}\\ \end{split}$

Montrons par recurrence que $M^{n}=PD^{n}P^{-1}$

**Initialisation:** $n=0$    $\begin{split} &M^{0}=PD^{0}P^{-1}\\ \Leftrightarrow &I=PP^{-1} \: \text{ça marche}  \end{split}$

Mais encore: $n=1$  $\begin{split} &M^{1}=PD^{1}P^{-1}\\ \Leftrightarrow &M=PDP^{-1} \: \text{ça marche}  \end{split}$

**Hérédité:** Supposons que $M^{n}=PD^{n}P^{-1}$ est vrai. 
On veut démontrer que $M^{n+1}=PD^{n+1}P^{-1}$ est vrai

$\begin{split} &M^{n} \times M =PD^{n}P^{-1}PDP^{-1}\\ \Leftrightarrow &M^{n+1}=PD^{n+1}P^{-1} \\ \end{split}$

Conclusion: $\boxed{\forall \in \mathbb{N}, M^{n}=PD^{n}P^{-1}}$

d- On veut retrouver la expression de $M^{n}$

On commence par calculer
$PD^{n}= \begin{pmatrix} 3 & 1 & 0 \\ 2 & 1 & 1 \\ 1 & 0 & 1 \end{pmatrix} \begin{pmatrix} (-4)^{n}  & 0 & 0  \\ 0 & (-2)^{n} & 0 \\ 0 & 0 & (-2)^{n} \end{pmatrix} = \begin{pmatrix} 3(-4)^{n}  & (-2)^{n} & 0  \\ 2(-4)^{n} & (-2)^{n} & (-2)^{n} \\ (-4)^{n} & 0 & (-2)^{n} \end{pmatrix}$

Après on calcule 

$(PD^{n})P^{-1} = \begin{pmatrix} 3(-4)^{n}  & (-2)^{n} & 0  \\ 2(-4)^{n} & (-2)^{n} & (-2)^{n} \\ (-4)^{n} & 0 & (-2)^{n} \end{pmatrix} \frac{1}{2} \begin{pmatrix} 1 & -1 & 1 \\ -1 & 3 & -3  \\ -1 & 1 & 1 \end{pmatrix}$

On trouve $\boxed{M^{n}=\frac{1}{2} \begin{pmatrix} 3(-4)^{n}-(-2)^{n} & -3(-4)^{n}+3(-2)^{n} & 3(-4)^{n}-3(-2)^{n} \\ 2(-4)^{n} & -2(-4)^{n}+2(-2)^{n}  & 2(-4)^{n}-2(-2)^{n} \\ (-4)^{n}+(-2)^{n}  & -(-4)^{n}-(-2)^{n} & (-4)^{n}+(-2)^{n}\end{pmatrix}}$