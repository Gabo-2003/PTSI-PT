#transformation_de_mouvement
## Changement de base
![[image changement de base.png|300]]
Considérons la base $B(\overrightarrow{i}, \overrightarrow{j}, \overrightarrow{k})$ et la base $B_{1}(\overrightarrow{u}, \overrightarrow{v}, \overrightarrow{k})$

| $\displaystyle\cos(\alpha)= \frac{l_{1}}{\| \overrightarrow{u} \|}=l_{1}$ | $\displaystyle\sin(\alpha)= \frac{l_{2}}{\| \overrightarrow{u} \|}=l_{2}$ |
| ------------------------------------------------------------------------- | ------------------------------------------------------------------------- |
|                                                                           $\displaystyle\cos(\alpha)= \frac{d_{1}}{\| \overrightarrow{u} \|}=d_{1}$ | $\displaystyle\sin(\alpha)= \frac{d_{2}}{\| \overrightarrow{u} \|}=d_{2}$                                                                           |
Donc :
- $\overrightarrow{u}= \cos(\alpha) \overrightarrow{i} + \sin(\alpha)\overrightarrow{j}$
- $\overrightarrow{v} = -\sin(\alpha)\overrightarrow{i}+ \cos(\alpha)\overrightarrow{j}$ 

## [[Géométrie de l'espace#Produit vectoriel|Produit vectoriel]] de 2 vecteurs 
$\overrightarrow{w}=\overrightarrow{v_{1}}\wedge \overrightarrow{v_{2}}$ 
### Direction 
Perpendiculaire au plan $(A, \overrightarrow{v_{1}}, \overrightarrow{v_{2}})$.
### Sens
Tel que $(\overrightarrow{v_{1}}, \overrightarrow{v_{2}}, \overrightarrow{w})$ forme une base directe. 
### Norme
$\| \overrightarrow{w} \| = \| \overrightarrow{v_{1}} \| \cdot \| \overrightarrow{v_{2}} \|  \cdot | \sin(\alpha) |$ 
### Propriétés 
- Antisymétrique : $\overrightarrow{v_{1}}\wedge \overrightarrow{v_{2}}=-\overrightarrow{v_{2}}\wedge \overrightarrow{v_{1}}$ 
- Produit vectoriel nul : $\overrightarrow{v_{1}}\wedge \overrightarrow{v_{2}}=\overrightarrow{0} \Leftrightarrow \begin{cases} \overrightarrow{v_{1}}= \overrightarrow{0} \\ \overrightarrow{v_{2}}= \overrightarrow{0} \\ \overrightarrow{v_{1}} \text{  et  }\overrightarrow{v_{2}} \text{  colinéaires} \end{cases}$
### Expression en fonction des composantes 
$\overrightarrow{w}= \overrightarrow{v_{1}} \wedge \overrightarrow{v_{2}}= \begin{cases} X_{1} \quad X_{2} \\ Y_{1} \wedge Y_{2} \\ Z_{1} \quad Z_{2} \end{cases} = \begin{cases} Y_{1}Z_{2} - Z_{1}Y_{2} \\ X_{2}Z_{1}-Z_{2}X_{1} \\ X_{1}Y_{2}-Y_{1}X_{2} \end{cases}$ 
### Calcul direct du produit vectoriel
Le produit entre deux vecteurs d'une même base est égal au troisième vecteur.
![[image calcule direct produit vetoriel.png|300]] 

## [[Géométrie de l'espace#Produit mixte|Produit mixte]] de trois vecteurs 
$V=(\overrightarrow{V_{1}}, \overrightarrow{V_{2}}, \overrightarrow{V_{3}}) = (\overrightarrow{V_{1}} \wedge \overrightarrow{V_{2}})\cdot \overrightarrow{V_{3}}$  
- $(\overrightarrow{V_{1}}, \overrightarrow{V_{2}}, \overrightarrow{V_{3}})=(\overrightarrow{V_{3}}, \overrightarrow{V_{1}}, \overrightarrow{V_{2}}) = (\overrightarrow{V_{2}}, \overrightarrow{V_{3}}, \overrightarrow{V_{1}})$ 
- $(\overrightarrow{V_{1}}, \overrightarrow{V_{2}}, \overrightarrow{V_{3}}) = -(\overrightarrow{V_{2}}, \overrightarrow{V_{1}}, \overrightarrow{V_{3}}) = -(\overrightarrow{V_{1}}, \overrightarrow{V_{3}}, \overrightarrow{V_{2}})= -(\overrightarrow{V_{3}}, \overrightarrow{V_{2}}, \overrightarrow{V_{1}})$ !