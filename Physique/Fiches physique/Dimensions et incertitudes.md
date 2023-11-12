#chapitre0
## Dimensions et unités:
Une unité est nécessaire pour déterminer la valeur d'une grandeur physique.

| Longueur             | Mètre $(m)$       | Symbole : $L$      |
| -------------------- | ----------------- | ------------------ |
| Masse                | Kilogramme $(kg)$ | Symbole : $M$      |
| Temps                | Second $(s)$      | Symbole : $T$      |
| Intensité électrique | Ampère $(A)$      | Symbole : I        |
| Quantité de matière  | Mole $(mol)$      | Symbole : $N$      |
| Température          | Kelvin $(K)$      | symbole : $\theta$ |
| Intensité lumineuse  | Candela $(cd)$    | Symbole : $J$                   |
### Opérations possibles:
- $[a+b]\equiv [a]+[b]$
- $[a \times b]\equiv [a] \times [b]$ (division possible)
On cherche l'homonéite des fonctions
### Grandeurs fréquemment utilisées
#### Force : 
On la trouve en utilisant la [[Dynamique Newtonienne#2èm Loi Principe fondamental de la dynamique|deuxième loi de Newton]]. 
$[\overrightarrow{F}]=MLT^{-2}$
#### Energie : 
On la trouve en utilisant [[Etude énergétique#Théorème de l'énergie et de la puissance cinétique|l'énergie cinétique]]. 
- $[E_{c}]=ML^{2}T^{-2}$
#### Champ magnétique 
On utilise la [[Mouvement d'une particule chargée dans un champ électrique ou magnétique.#Force de Lorentz $ vec{F_{L}} = vec{F_{el}} + vec{F_{mag}}$|Force de Lorentz]] .
- $[B]=MT^{-2}I$ 
## Incertitude :
### Variabilité et incertitude-type:
Expérimentalement aucune mesure n'est parfait. On quantifié cette variabilité
- $\displaystyle \overline{X}=\frac{1}{N} \sum_{i=1}^{N} x_{i}u(x)=\sqrt{\frac{1}{N-1}\sum_{i=1}^{N}(x_{i}-\overline{X})^{2}}$
- Il y a moins de $5\%$ de chances que deux mesures soient distant de plus de $4u(x)$ 
### Comparaison de deux mesurages :
- $\displaystyle R_{n}=\frac{|\overline{x_{1}}-\overline{x_{2}}|}{\sqrt{u(x_{1})^{2}+u(x_{2})^{2}}}$
$\quad \quad E_{n}\leq 2$: compatible  
$\quad \quad E_{n}> 2$: compatible 
### Evaluation d'une incertitude type:
Statistique : possibilité de repetition
- $u(\overline{x})= \frac{u(x)}{\sqrt{N}}$
Autre que statistique : pas de possibilité de répétition
- $u(\overline{x})= \frac{\Delta}{\sqrt{3}}$
Résultat experimental 
- $x=(\overline{x}\pm u(x))$ unité
### Incertitude-type composé :
Somme : $u(q)=\sqrt{(\alpha u(x))^{2}+(\beta u(y))^{2}}$
Produit : $\frac{u(q)}{q}=\sqrt{(\alpha \frac{u(x)}{x})^{2}+(\beta \frac{u(y)}{y})^{2}}$
### Regression linéaire :
Déterminer les paramètres de $a$ et $b$ tels que la droite $y=ax+b$ passe au plus près de tous les points expérimentaux 