---
tags:
  - electronique
---
## Nature
### Nature du composant électronique 
![[image nature ALI.png|300]]

- $+V_{CC}$ et $-V_{CC}$ : ils reprenant les alimentations continues du composant 
- $V_{-}$ : Entrée inverseuse 
- $V_{+}$ : Entrée non-inverseuse
- L'ALI amplifie la différence $\epsilon = V_{+} - V_{-}$
- $V_{s}$ : sortie
### Représentations conventionnelles 
![[image representation conventionnelles.png]]
### Comportement réel
On a le comportement d'un filtre passe bas (absence de saturation).
$\displaystyle \underline{\mu } = \frac{\underline{V_{S}} }{\underline{V_{+}} - \underline{V_{-}} } = \frac{\underline{V_{S}} }{\underline{\epsilon} } = \frac{\mu _{0}}{1+j \frac{\omega }{\omega _{0}}}$   avec $\epsilon = V_{+} - V_{-}$.
- Gain statique : $\mu _{0} > 10^{5}$ 
- Temps caractéristique : $\tau \approx 100 \;ms$
- Fréquence de coupure : $3 \sim 4 \; Hz$ 

## Modélisation 
![[image modele ALI.png|300]]
On considère le modèle suivant :
- Impédance d'entrée infinie sur $V_{+}$ et $V_{-}$ donc : $i_{+} = i_{-} = 0$.
- Impédance de sortie nulle, donc quelque soit le courant de sortie, la tension de sortie $V_{s}$ est inchangée.
- La tension de sortie est limitée : $\pm V_{sat}$
### Rétroaction stabilisant 
Un montage à ALI nécessite une rétroaction sur l'entrée inverseuse pour que la stabilité soit assurée.
### Limites du modèle 
#### Vitesse de balayage 
C'est la vitesse de réponse à une excitation donnée 
- Slew rate : pente de sortie maximale : entre $0,5$ et $20 \; V / \mu s$
![[image slew rate.png|400]]
#### Intensité de saturation 
L'intensité de sortie ne peut dépasser les valeurs de saturation caractéristiques : $\pm i_{sat}$ qui est vers $20 \;mA$
#### Saturation en tension
Pareil que pour l'intensité mais vers  $\pm 14 \; V$

## Regimes
### ALI idéal de gain infinie en régime linéaire 
On va considérer que $\mu _{0} = + \infty$. Cela permet d'établir des relations entrée - sortie fiables.
Le régime linéaire correspondra à $\epsilon =0$ et $V_{S} \in ]- V_{sat}, + V_{sat}[ \implies V_{+} = V_{-}$
### ALI idéal de gain infinie en régime saturé 
On a:
- $\epsilon > 0 \Leftrightarrow V_{S} = + V_{sat}$ 
- $\epsilon < 0 \Leftrightarrow V_{S} = - V_{sat}$

## Montages 
### Amplificateur non-inverseur 
![[image amplificateur non inverseur.png|400]]
#### Régime linéaire 
##### ALI réel
On trouve $\displaystyle \frac{V_{s}}{V_{-}} = G$  et d'après  $\underline{\mu } = \frac{\underline{V_{S}} }{\underline{V_{+}}  - \underline{V_{-}} } = \frac{\mu _{0}}{1+j \frac{\omega}{\omega _{0}}}$
Alors $\displaystyle \underline{H}  = \frac{V_{s}}{V_{e}} = \frac{\mu _{0}}{1+ \frac{\mu _{0}}{G} +j \frac{\omega }{\omega _{0}}}$
Et donc on a comme pulsation de coupure $\displaystyle \omega'_{0} = \omega _{0}(\underbrace{1}_{\text{négligeable}} + \frac{\omega _{0}}{G})$
Alors le produit gain - bande est constante 
![[image amplificateur non inverseur regime lineaire ALI reel.png|300]]
##### ALI idéal
On trouve $\displaystyle \frac{V_{S}}{V_{e}} = \frac{R_{1}+R_{2}}{R_{1}} = G$ 
On a une impédance d'entrée infinie et de sortie nulle. Alors les montages en amont et en aval ne sont pas perturbes. 
### Montage inverseur 
![[image montage inverseur.png|400]]
#### Régime linéaire
##### ALI idéal de gain infinie 
On trouve $\displaystyle \frac{V_{S}}{V_{E}} = - \frac{R_{2}}{R_{1}}$ 
### Comparateur à hystérésis 
![[image comparateur a hysteresis.png|400]]
#### Régime linéaire 
##### Ali réel
On trouve $\displaystyle\underline{H} = \frac{-\mu _{0}}{1- \frac{\mu _{0}}{G} + j \frac{\omega }{\omega _{0}}}$
C'est un montage instable alors il fonctionne en saturation.
#### Régime saturé 
##### ALI idéal  
Pour trouver les conditions de saturation, on fait l'hypothèse d'être en saturation 
![[image regime saturee.png|300]]
Ce montage réalise une fonction mémoire binaire.
### Montage suiveur 
![[image montage suiveur.png|400]]
#### Régime linéaire 
##### ALI ideal
$V_{+} = V_{E} = V_{-}$ et $V_{-} = V_{S}$ 
$\implies V_{S} = V_{E}$ 
On prélève un signal pour la dupliquer sans l'altérer : on ne prélève aucune puissance. 
### Montage intégrateur 
![[image montage integrateur.png|400]]
#### Régime linéaire 
##### Ali ideal
$\displaystyle \frac{V_{S}}{V_{E}} = - \frac{1}{jRC \omega }$
Problème : les signales en continue sont amplifies ce qui conduit à la saturation. 
### Comparateur simple 
![[image comparateur simple.png|400]]
$\epsilon = V_{+} - V_{-} = V_{E} - V_{0}$ 
- Si $V_{E}> V_{0} \implies V_{S} = + V_{sat}$
- Si $V_{E} < V_{0} \implies V_{S} = - V_{sat}$