#transformation_de_mouvement
Permettent remplacer un système de vecteur liés par un seul être mathématique.
## Définition
### Résultante $\vec{R}$ :
Ce vecteur est le même pour tout point.
### Moment $\vec{M_{A}}$ :
Ce vecteur dépende du point de réduction.
#### Formule de Varignon 
$\overrightarrow{M_{B}}= \overrightarrow{M_{A}}+ \overrightarrow{BA} \wedge \overrightarrow{R} \quad \forall A \text{  et  } B$ 

## Notation
$\{ T \} = \begin{Bmatrix} \overrightarrow{R}  \\ \overrightarrow{M_{A}} \end{Bmatrix} = \begin{Bmatrix} X & L \\ Y & M \\ Z & N \end{Bmatrix}_{A,R}$
avec $\overrightarrow{R}= \begin{pmatrix} X \\ Y \\ Z \end{pmatrix}$ et $\overrightarrow{M_{A}}= \begin{pmatrix} L \\ M \\ N \end{pmatrix}$

## Changement de centre de réduction
$\{ T \} = \begin{Bmatrix} \overrightarrow{R}  \\ \overrightarrow{M_{A}} \end{Bmatrix}_{A} = \begin{Bmatrix} \overrightarrow{R}  \\ \overrightarrow{M_{B}}= \overrightarrow{M_{A}}+ \overrightarrow{BA} \wedge \overrightarrow{R} \end{Bmatrix}_{B}$

## Somme 
Doivent être définies au même point. 
$\{ T_{1} \} + \{ T_{1} \} = \begin{Bmatrix} \overrightarrow{R_{1}} + \overrightarrow{R_{2}}  \\ \overrightarrow{M1_{A}} + \overrightarrow{M2_{A}}  \end{Bmatrix}_{A}$ 

## Axe central 
Ensemble des points où la résultante du torseur est colinéaire.
$\overrightarrow{M_{P}}=k \overrightarrow{R}$ 

## Torseurs particulières 
### Torseurs couple
Résultant nulle :  $\{ T \} = \begin{Bmatrix} \overrightarrow{0}  \\ \overrightarrow{M} \end{Bmatrix}_{A}= \begin{Bmatrix} \overrightarrow{0}  \\ \overrightarrow{M} \end{Bmatrix}_{B}$
### Glisseurs 
On a un glisseur s'il existe au moins un point $A$ tel que :
- $\overrightarrow{M_{A}}=\overrightarrow{0}$ donc   $\{ T \} = \begin{Bmatrix} \overrightarrow{R}  \\ \overrightarrow{0} \end{Bmatrix}_{A}$ 
- Ou si $\overrightarrow{R} \cdot \overrightarrow{M_{A}}=0$ 


