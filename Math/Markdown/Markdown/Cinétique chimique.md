Soit la réaction $|\alpha|A+|\beta|B=|\gamma|C+|\delta|D$ 
## Différents vitesses
### Vitesse de formation/disparition
$\displaystyle v_{C}= \frac{dn_{C}}{dt}$             $\displaystyle v_{A}= - \frac{dn_{A}}{dt}$   en $mol\cdot s^{-1}$ 
### Vitesse molaire 
$\displaystyle v_{mol} = \frac{d \xi}{dt} = - \frac{1}{\alpha} \frac{dn_{A}}{dt} = \frac{1}{\gamma} \frac{dn_{C}}{dt}$ en $mol \cdot s^{-1}$
### Vitesse de réaction 
$\displaystyle v_{re}= \frac{d}{dt} \left(\frac{\xi}{V}\right) =  - \frac{1}{\alpha} \frac{d[A]}{dt} = \frac{1}{\gamma} \frac{d[C]}{dt}$  en $mol \cdot L^{-1} \cdot s^{-1}$
### Temps de demi-réaction 
$\displaystyle \xi(t_{\frac{1}{2}})= \frac{\xi(t_{f})}{2}$   avec  $\displaystyle  t_{\frac{1}{2}} \neq \frac{t_{f}}{2}$  

## Facteurs cinétiques 
### Facteur cinétique
1- Concentration des réactifs
- Augment la probabilité que les réactives se rencontrent.
2- Température
- Augmente la probabilité qu'un choc soit efficace.
3- Présence d'un catalyseur
### Loi de vitesse et ordre de réaction 
#### Loi de vitesse 
Relation qui relie la vitesse de réaction $v$ aux concentrations.
$v_{re}=k[A]^{mA}[B]^{mB}$ 
- $mA$ : ordre partielle par rapport à $A$.
- $mB$ : ordre partielle par rapport à $B$.
- $k$ : constante de vitesse de la reaction. 
##### Ordre initial
Ordre aux instants proches de le moment initial pour les réaction sans ordre.
#### Loi d'Arrhenius 
$\displaystyle \frac{d \ln(k)}{dT}= \frac{E_{A}}{RT^{2}} \quad \quad \Rightarrow k(T)=A e^{-\frac{E_{A}}{RT}}$
- $E_{A}$ : Energie d'activation en $J \cdot mol^{-1}$.

## Etude d'ordres simples 

| Ordre | Loi de vitesse                            | Loi integrée                         | Temps de demi-réaction                                  |
| ----- | ----------------------------------------- | ------------------------------------ | ------------------------------------------------------- |
| 0     | $\frac{d[A]}{dt}=-\mid \alpha \mid k$     | $[A]=[A_{0}]-\mid\alpha\mid kt$      | $t_{\frac{1}{2}}= \frac{[A_{0}]}{2 \mid \alpha \mid k}$ |
| 1     | $\frac{d[A]}{dt}=-\mid \alpha \mid k [A]$ | $[A]=[A_{0}] e^{-\mid\alpha\mid kt}$ | $t_{\frac{1}{2}}= \frac{\ln(2)}{ \mid \alpha \mid k}$   |
| 2     |          $\frac{d[A]}{dt}=-\mid \alpha \mid k [A]^{2}$ |$\frac{1}{[A]}= \frac{1}{A_{0}}+ \mid\alpha\mid kt$                                      |$t_{\frac{1}{2}} = \frac{1}{\mid \alpha\mid k [A]_{0}}$                                                         |

## Détermination expérimentale de l'ordre d'une réaction 
Se ramener à une vitesse de la forme $v=k_{app}[A]^{p}$ par un choix approprié des conditions expérimentales 
### Choix des conditions 
Soit la réaction $|\alpha|A+|\beta|B=|\gamma|C+|\delta|D$ 
$v=k[A]^{m}[B]^{n}$ 
#### Mélange stœchiométrique
$\displaystyle\frac{n_{A}}{\alpha} = \frac{n_{B}}{\beta}$ 
$v= k_{app} \times [A]^{p}$  avec  $\begin{cases} k_{app} = k \times (\frac{\beta}{\alpha})^{n}  \\ p = m+n\end{cases}$
- Cette méthode permet donc d'accéder à l'ordre global de la réaction.
#### Dégénérescence de l'ordre 
On met un des réactifs en excès et on suppose que sa concentration ne varie pas lors de la réaction. 
$[A](t) = [A]_{0}$ 
- $v= k_{app} \times [B]^{n}$       avec $k_{app}=k[A]_{0}^{m}$
- Cette permet de déterminer l'ordre partiel par rapport à un réactif largement limitant par rapport aux autres. 
