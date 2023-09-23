1- On veut démontrer par recurrence l'égalité :
$$\sum_{k=1}^{n} \frac{2k-1}{k!2^{k}}=1- \frac{1}{n!2^{n}}$$

**Initialisation :** 
pour $n=1$    $\begin{align*} \sum_{k=1}^{1} \frac{2k-1}{k!2^{k}}= \frac{2-1}{2}=\frac{1}{2} \end{align*}$
ça marche

**Hérédité :** On suppose que $\begin{align*} \sum_{k=1}^{n} \frac{2k-1}{k!2^{k}}=1- \frac{1}{n!2^{n}} \end{align*}$ est vrai.
On veut démontrer que $\begin{align*} \sum_{k=1}^{n+1} \frac{2k-1}{k!2^{k}}=1- \frac{1}{(n+1)!2^{n+1}} \end{align*}$.

$$\begin{align*} &\sum_{k=1}^{n} \frac{2k-1}{k!2^{k}}=1- \frac{1}{n!2^{n}} \\ \Leftrightarrow& \sum_{k=1}^{n+1} \frac{2k-1}{k!2^{k}} - \frac{2n+1}{(n+1)!2^{n+1}} =1- \frac{1}{n!2^{n}} \\ \Leftrightarrow& \sum_{k=1}^{n+1} \frac{2k-1}{k!2^{k}} =1+\frac{2n+1}{(n+1)!2^{n+1}}- \frac{1}{n!2^{n}} = 1+ \frac{(2n+1)n!2^{n}-(n+1)!2^{n+1}}{(n+1)!n!2^{n+1}} \end{align*}$$
$$\Leftrightarrow \boxed{\sum_{k=1}^{n+1} \frac{2k-1}{k!2^{k}}=1- \frac{1}{(n+1)!2^{n+1}} \text{  CQFD}}$$ 

**Conclusion :** On a bien démontre que $\forall n \in \mathbb{N}^{*}$
$$\boxed{\sum_{k=1}^{n} \frac{2k-1}{k!2^{k}}=1- \frac{1}{n!2^{n}}}$$

Maintenant on veut démontrer la même formule avec une somme télescopique. 

$$\begin{align*} \sum_{k=1}^{n} \frac{2k-1}{k!2^{k}} &=  \sum_{k=1}^{n} \frac{2k}{k!2^{k}} - \frac{1}{k!2^{k}} =\sum_{k=1}^{n} \frac{1}{(k-1)!2^{k-1}} - \frac{1}{k!2^{k}} \\ &= \frac{1}{1} + \frac{1}{2} +\frac{1}{2^{3}} + \ldots + \frac{1}{(n-2)!2^{n-2}} + \frac{1}{(n-1)!2^{n-1}} \\ &-(\frac{1}{2} + \frac{1}{2^{3}} + \frac{1}{2^{4} \times 3}+ \ldots +\frac{1}{(n-1)!2^{n-1}} + \frac{1}{n!2^{n}}) \end{align*}$$

On reconnait une somme télescopique, on a donc :
$$\boxed{\sum_{k=1}^{n} \frac{2k-1}{k!2^{k}}=1- \frac{1}{n!2^{n}}}$$

2- pour $k=1$ on a : 

$U \begin{cases} 1 \text{  noire} \\ 1 \text{  blanche} \end{cases}$         Alors $|\Omega|=2$   et   $|N_{1}|=1$

On en déduit $P(N_{1})= \frac{|\Omega|}{|N_{1}|}$
$$\boxed{P(N_{1})=\frac{1}{2}}$$

3- Si on prend une boule noire à $k=1$ :
$U \begin{cases} 1 \text{  noire} \\ 3 \text{  blanches} \end{cases}$       donc $P_{N_{1}}(N_{2})=\frac{1}{4}$  

Si on prend une boule blanche à $k=1$ :
$U \begin{cases} 3 \text{  noire} \\ 1 \text{  blanches} \end{cases}$       donc $P_{\overline{N_{1}}}(N_{2})=\frac{3}{4}$  

D'après la formule de probabilité totale :
$$P(N_{2})=P(N_{1})P_{N_{1}}(N_{2})+P(\overline{N_{1}})P_{\overline{N_{1}}}(N_{2})$$
$$\boxed{P(N_{2}) = \frac{1}{2}}$$

4- La famille $(N_{k})_{k=1}^{n}$ peut être mutuellement indépendants si : $P(N_{1} \cap N_{2}) = P(N_{1})P(N_{2})$, On le vérifie :

D'après la loi de probabilité composé : 
$P(N_{1} \cap N_{2}) = P(N_{2})P_{N_{2}}(N_{1}) =\frac{1}{2} \times \frac{1}{4}=\frac{1}{8}$
et $\frac{1}{8} \neq \frac{1}{2} \times \frac{1}{2}= P(N_{1}) \times P(N_{2})$

$\text{Alors  }P(N_{1}) \text{  et  } P(N_{2}) \text{  ne sont pas independantes}$
$\boxed{\text{Donc la famille  }(N_{k})_{k=1}^{n} \text{  n'est pas independant}}$

5- D'après la loi de probabilité conditionnelle :
$P_{N_{2}}(N_{1})=\frac{P(N_{1} \cap N_{2})}{P(N_{2})} =\frac{\frac{1}{8}}{\frac{1}{2}}$
$\boxed{P_{N_{2}}(N_{1})=\frac{1}{4}}$

6- A chaque tirage on ajute 2 balle, Alors.
$\begin{align*} Boules_{j}=\sum_{k=0}^{j}2 \end{align*}$
$\boxed{Boules_{j}=2(j+1)}$

7- Chaque fois qu'on prend une boule blanche on ajoute 2 noires et maintient 1 blanche. Alors, d'après la formule de probabilités composées : $\forall k \in [[2,n]]$
$P_{\bigcap_{j=1}^{k-1} \overline{N_{j}}}(\overline{N_{k}})=\frac{1}{2k}$
On en déduit aussi
$P_{\bigcap_{q=1}^{k-1} \overline{N_{q}}}(N_{k})=\frac{2k-1}{2k}$

Alors $\forall k \in [[2,n]]$
$$\begin{align*} P(A_{k})&=P(\overline{N_{1})} \times  \prod_{i=1}^{k-2} P_{\bigcap_{j=1}^{i} \overline{N_{j}}}(\overline{N_{i+1}}) \times P_{\bigcap_{i=1}^{k-1} \overline{N_{i}}}(N_{k})   \\ &=\frac{1}{2} \prod_{i=1}^{k-2} \frac{1}{2(i+1)} \times \frac{2k-1}{2k} =\frac{1}{2} \frac{1}{2^{k-2}(k-1)!} \times \frac{2k-1}{2k} \end{align*}$$
$$\boxed{P(A_{k})= \frac{2k-1}{2^{k}k!}}$$

On vérifie pour $k=1$
$P(A_{1})=\frac{2-1}{2}=\frac{1}{2}$ ça marche

8- Similairement que à la question précèdent, on trouve :
$$P(A_{0})=P(\overline{N_{1})} \times  \prod_{i=1}^{n-1} P_{\bigcap_{j=1}^{i} \overline{N_{j}}}(\overline{N_{i+1}})=\frac{1}{2} \times \prod_{i=1}^{n-1} \frac{1}{2(i+1)} = \frac{1}{2} \times \frac{1}{2^{n-1}n!}$$
$$\boxed{P(A_{0})=\frac{1}{n!2^{n}}}$$

9- Or $\{ A_{k} \} _{k \in [[0,n]]}$ est une système complete d'évenements, alors la somme des probabilités de tous les événements est egal à la probabilité de l'univers $\Omega$.
$$\begin{align*} \sum_{k=0}^{n}P(A_{k})=P(\Omega) \end{align*}$$
$$\Leftrightarrow \boxed{\sum_{k=1}^{n} \frac{2k-1}{2^{k}k!} + \frac{1}{n!2^{n}} =1 \quad CQFD}$$