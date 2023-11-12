#dimensionnement_de_liaisons_et_transmission_d_efforts 
### Actions mécaniques
Toute cause susceptible de : maintenir un corps en repos, créer ou modifier un mouvement, déformer un corps.
#### Force 
Modélise une action mécanique appliquée à un point. Il est modélise par un glisseur. 
#### Moment
$M_{a}(\overrightarrow{F})=\overrightarrow{AM} \wedge \overrightarrow{F}$ 
- Intensité : $\| \overrightarrow{M_{A}(\overrightarrow{F})} \| = \| \overrightarrow{F} \| \times |d|$        $d=d(A,\Delta)$ 

## Modélisation des actions mécaniques 
### Pesanteur 
$\{ P \} = \begin{Bmatrix} m \overrightarrow{g} \\ \overrightarrow{0} \end{Bmatrix}_{G}$ 
#### Centre de gravité $G$
$\displaystyle m \cdot \overrightarrow{OG}= \int_{M \in S} \overrightarrow{OM} \cdot dm$ 
- Si $(S)$ est homogène :  $\displaystyle \overrightarrow{OM}= \frac{1}{m} \sum_{i=1}^{n}m_{i} \overrightarrow{OG_{1}}$ 
### Liaison parfait 
Pas de frottement.
- Pour la liaison hélicoïdale $L_{12}=-pX_{12}$       $p= \frac{pas}{2\pi}$  
### Contacts réels 
- $\overrightarrow{f_{p}}(S_{1}\rightarrow S_{2})$ : densité surfacique en $N / mm^{2}$.
- $\overrightarrow{n_{p}}(S_{1} \rightarrow S_{2})$ : densité surfacique normale. 
- $\overrightarrow{t_{p}}(S_{1} \rightarrow S_{2})$ : densité surfacique tangentielle.
- $\displaystyle \Big \{ T(S_{1}\rightarrow S_{2}) \Big \} = \begin{Bmatrix} \displaystyle \overrightarrow{R}(1\rightarrow2)= \int_{P \in S}\overrightarrow{f_{p}}(1 \rightarrow 2) dS \\ \displaystyle \overrightarrow{M_{A}}(1 \rightarrow 2) = \int_{P \in S} \overrightarrow{AP} \wedge \overrightarrow{f_{p}}(1 \rightarrow 2) dS \end{Bmatrix}$  
![[image contact reel.png|350]]
#### Lois de Coulomb
$f=\tan(\varphi)$
##### 1èr cas : $\overrightarrow{V}(P,S_{2} / S_{1}) \neq \overrightarrow{0}$ 
![[image lois de coulomb 1.png|300]]
- $\overrightarrow{f_{p}}$ sur le bord du cône de frottement.
- $\overrightarrow{t_{p}}(1 \rightarrow 2)$  opposé à la vitesse de glissement $\overrightarrow{V}(P \in S_{2} / S_{1})$ 
- $\overrightarrow{t_{p}}(1 \rightarrow 2) \wedge \overrightarrow{V}(P, 2 / 1) = \overrightarrow{0}$   (direction)
- $\overrightarrow{t_{p}}(1 \rightarrow 2) \cdot \overrightarrow{V}(P, 2 / 1) = \overrightarrow{0}$   (sens)
- $\| \overrightarrow{t_{p}}(S_{1} \rightarrow S_{2}) \| = f \cdot \| \overrightarrow{n_{p}}(1 \rightarrow 2) \|$   (module) 
$\quad \quad \Leftrightarrow \overrightarrow{T} = f \cdot \overrightarrow{N}$ 
##### 2èm cas : $\overrightarrow{V}(P,S_{2} / S_{1}) = \overrightarrow{0}$ 
- $\overrightarrow{f_{p}}$  à l'intérieur du cône.
