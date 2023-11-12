#dimensionnement_de_liaisons_et_transmission_d_efforts 
## Liaison équivalentes
### En série 
$\big\{ V_{2 / 0} \big\}_{Q} = \big\{ V_{2 / 1} \big\}_{Q} + \big\{ V_{1 / 0} \big\}_{Q}$ 
### Parallèles 
$\big\{ T_{s} \big\}_{Q} = \big\{ T_{s} \big\}_{Q} + \big\{ T_{s} \big\}_{Q}$ 
$\big\{ V_{eq} \big\} = \big\{ V_{L1} \big\} = \big\{ V_{L2} \big\}$  (on prend les inconnues commun)
- Si on supprime plusieurs fois une liberté, on a une assemblage plus rigide mais plus couteux.
- Le choix du point de définition des torseurs est important pour observer la forme caractéristique de la liaison.

## Théorie des mécanismes 
- $i_{c}+i_{s}=6$ pour une même liaison.
### Nombre cyclomatique
$\gamma$ indique le nombre de boucles indépendantes 
- $\gamma = L-N+1$
- $L$ : nombre de liaisons
- $N$ : Nombre de pièces 
### Mobilité du mécanisme $m_{c}$ 
- Mobilité utile : $m_u$ 
- Mobilité interne : $m_{i}$ 
- $m_{c}=m_{u}+m_{i}$ 
### Hyperstatisme
$h$ est le degré d'hyperstatisme.
#### Approche statique 
Le système doit être en équilibre
$E_{s}=6 \times N$      ($N$ nombre de pièces isolables)
![[image matrice hyperstatisme statique.png]]
$I_{s}-r_{s}= h$
$E_{s}- r_{s}=m$
- $\boxed{E_{s}-I_{s}=m-h}$  
#### Approche cinématique 
$\gamma$ : nombre de boucles 
- $\gamma = L-N+1$      avec $L$ Le nombre de liaisons et $N$ nombre de pièces.
$E_{c}=6 \gamma$ 
![[image matrice hyperstatism cinetique.png]]
$I_{s}-r_{s}= h$
$E_{s}- r_{s}=m$
- $\boxed{I_{c}-E_{c} = m-h}$

## L'utilisation en conception
### Méthode statique
Plus utile pour deux pièces liés plusieurs fois. 
- Si on a une équation de tipe $0=f(X_{ext})$ alors on a une mobilité
	- La mobilité peut être une rotation ou une translation dépendent de si l'équation forme partie de la résultante ou du moment
### Méthode cinématique
Plus utile pour deux pièces liés plusieurs fois. 
- Si on a une équation de tipe $0=0$ alors on a un degré d'hyperstatique
	- Peut rotation ou une translation dépendent de si l'équation forme partie de la résultante ou du moment

