---
tags:
  - meca_fluides
---
## Des systèmes fermés aux systèmes ouvertes 
### Schema à une entrée et une sortie 
#### Bilan sur les systèmes ouvertes (description eulérienne) 
On considère une surface fermée dit de contrôle fixe. Il y a échange de matière entre la surface de control et l'exterieur. 
#### Bilan sur un système fermée (description lagrangienne)
On considère une quantité déterminée de fluide délimitée par une surface fermée appelé surface particulière. Pas d'échange avec le milieu exterior. 
### [[Fluide en écoulement stationnaire dans une conduite#Conservation du débit massique|Conservation de la masse]] en régime stationnaire à  travers d'une machine 
$\displaystyle \sum _{entrée} D_{m,e} = \sum _{sortie} D_{m,s}$
 
## Relation de Bernoulli 
Il faut un [[Fluide en écoulement stationnaire dans une conduite#Fluide parfait|fluide parfait]], [[Fluide en écoulement stationnaire dans une conduite#Fluide incompressible|incompressible]] en [[Fluide en écoulement stationnaire dans une conduite#Régime stationnaire|régime stationnaire]]. 
$\displaystyle ( \frac{1}{2} v_{s}^{2} + gz_{s} + \frac{P_{s}}{\mu }) - (\frac{1}{2} v_{e}^{2} + gz_{e} + \frac{P_{e}}{\mu }) = w_{gen} + w_{reçu} + w_{d}$
- $w_{gen} < 0$ : [[Etude énergétique#Travail|Travail]] produit dans une turbine. 
- $w_{reçu} > 0$ : Travail reçue par compresseurs. 
- $w_{d} < 0$ : Travail dissipé (pertes de charge). 
On peut determiner le bilan de puissances en multipliant par $D_{m}$
## Pertes de charge 
Perte de pression dans une conduite. 
### Perte de charge singulière
Variation de la pression du à un rétrécissement, coude, bifurcation. 
- Diminution de pression : $\displaystyle P_{PC} = k \frac{1}{2}\mu v^{2}$
### Perte de charge régulière
Se font lors d'un écoulement visqueux dans une canalisation droite. 
- $P_{PC} = f \frac{L}{D} \frac{1}{2} \mu v^{2}$
### Expression de pertes de charge en pression ou altitude 
On peut exprimer la perte de charge dans une conduite comme perte de pression ou altitude.
- $w_{d} = -g \Delta z^{*} = \frac{\Delta P^{*}}{\mu }$
