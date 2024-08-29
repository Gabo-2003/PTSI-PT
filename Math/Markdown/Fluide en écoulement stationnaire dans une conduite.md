---
tags:
  - meca_fluides
---
## Les outils de base
### Description du fluide

#### Point de vue lagrangien 
On suive une particule dans son mouvement. 
#### Point de vue eulérien 
On regarde l'évolution du flot en un point de vue fixe.
### Régime stationnaire 
Le champ de vitesse est figé et n'évolue pas dans le temps. 
- $\displaystyle \frac{\partial \overrightarrow{v}(M,t)}{\partial t}=0$
Cela est aussi vrai pour tout les autres grandeurs physiques.
- $\displaystyle \frac{\partial P(M,t)}{\partial t} = 0, \quad \frac{\partial \mu (M,t)}{\partial t} = 0, \quad \ldots$
### [[Champ]] de vitesse
#### Lignes de courant 
![[Champ#Lignes de champs]]

#### Tubes de courant 
![[Champ#Tube de champ]]
- Une conduite forme un tube de courante particulière. 
### Quelque définitions 
#### Écoulement uniforme
La vitesse (en norme) est la même en tout point du fluide. 
#### Écoulement unidirectionnel 
La vitesse de l'écoulement possède une seule composant spatial. 
#### Écoulement unidimensionnelle 
Écoulement décrit par un seul paramètre d'espace. 
#### Fluide incompressible
La masse volumique $\mu$ ne dépend pas de la pression.
#### Écoulement incompressible
Masse volumique $\mu$ constante en tout point de l'espace. On peut faire cette approximation pour les gaz si la vitesse de l'écoulement est $<<$ vitesse du son dans le gaz. 

## Débit d'un fluide et notion de flux
### Débit massique
Masse traversant une section de la conduite par unité de temps. 
On a $\delta m = \mu  \delta V = \mu \overrightarrow{v} \cdot \overrightarrow{dS} \cdot dt$
$\displaystyle \implies \frac{\delta m}{dt} = \mu \overrightarrow{v} \cdot \overrightarrow{dS}$            Soit $\overrightarrow{j} = \mu \overrightarrow{v}$

$\displaystyle D_{m} = \int \int_{(S)} \frac{\delta m}{dt} = \int \int_{(S)} \mu  \overrightarrow{v} \cdot \overrightarrow{dS} = \int \int_{(S)} \overrightarrow{j} \cdot \overrightarrow{dS}$ 

- Le débit massique est le flux de $\overrightarrow{j}$
- Si écoulement incompressible : $\displaystyle D_{m} = \mu \int \int_{(S)} \overrightarrow{v} \cdot \overrightarrow{dS}$ 
- Si en plus fluide parfait : $\displaystyle D_{m} = \mu v \cdot S$   ($S$ une section droite)
### Conservation du débit massique
Le long d'un tube de courant en régime stationnaire, le débit massique se conserve. 
### Débit volumique 
$\displaystyle D_{v} \int \int_{(S)} \frac{\delta V}{dt} = \int \int_{(S)} \overrightarrow{v} \cdot \overrightarrow{ds}$
- Si $\mu$ constante : $D_{m} = \mu D_{v}$

## Écoulement laminaires 
### Types de fluides et viscosité 
#### Fluide parfait
Pas de viscosité ni de frottement interne. Tout la section a la même vitesse d'écoulement. 
- A vitesse élevée dans une conduit l'eau peut être considérée parfait. 
#### Fluides newtoniens 
On ne néglige pas la viscosité et l'action dissipative de l'écoulement.
#### Viscosité 
Force surfacique de cisaillement : $\displaystyle \overrightarrow{f_{c}} = -S \eta \frac{\partial v_{x}}{\partial y} \overrightarrow{e_{x}}$ 
Viscosité dynamique $\eta$ : indépendant de la vitesse pour un fluide newtonien. 
Force volumique équivalente :  $\overrightarrow{f}_{v,visquex} = - \eta \Delta \overrightarrow{v}$ 
- Unité de $\eta$ : Poiseuille $(Pl)$ homogène à $Pa \cdot s$ 
### Condition aux limites sur un canalisation 
Pour un fluide parfait : il ne peut pas y avoir des vitesses orthogonales à la paroi : $\overrightarrow{v} \cdot \overrightarrow{n} = 0$
Pour un fluide visqueux : ils s adhèrent au paroi : $\overrightarrow{v}(paroi) = \overrightarrow{0}$ 
### Écoulements laminaires et turbulentes 
#### Écoulement laminaires
Écoulement ordonnée où les lignes de courant forment des lames qui ne se déforment pas dans le temps. 
#### Nombre de Reynolds 
Nombre sans unité qui permet de savoir si l'écoulement est laminaire, intermédiaire ou turbulente. 
$\displaystyle R_{e} = \frac{\mu l v}{\eta}$ avec $l$ le diamètre du tuyau. 
- $R_{e} < 2000$ : écoulement laminaire.
- $2000 < R_{e} < 4000$ : écoulement intermédiaire.
- $R_{e} > 4000$ : écoulement turbulente. 