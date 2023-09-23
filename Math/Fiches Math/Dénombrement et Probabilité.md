#probabilite 
$card(A \cup B) = card(A)+card(B)-card(A \cap B)$ 
## Listes et combinaisons

|            | Ordre : oui                                                                                             | Ordre : non                     |
| ---------- | ------------------------------------------------------------------------------------------------------- | ------------------------------- |
| Répétition | $\begin{align*} &\text{n-liste :  } card(E)^{n} \\ &card(\mathcal{F}(R,F)) = card(F^{E})  \end{align*}$ |                                 |
| Non-Rép    | $\begin{align*} &\text{p-liste d'éléments} \\ & \text{distincts :  } \frac{n!}{(n-p)!} \end{align*}$    | Combinaison : $\binom{n}{p}$ | 
- Permutation : n-liste d'éléments distincts $n!$ 

## Espaces probabilisés finis 
- $P(A \cup B) = P(A)+ P(B)- P(A \cap B)$ 
- $P(A \cup B \cup C) = P(A)+P(B)+P(C)-P(A \cap B)-P(A \cap C)-P(B \cap C) + P(A \cap B \cap C)$    
- $\displaystyle P(A)= \frac{\text{nombre de cas favorables}}{\text{nombre de cas}}$ 

## Probabilité conditionnelle
$\displaystyle P_{B}(A)= \frac{P(A \cap B)}{P(B)}$ 
### Formule de probabilité compose 
- $P(A \cap B)=P(B)P_{B}(A)$ 
- $P(A_{1} \cap A_{2} \cap \ldots \cap A_{n})= P(A_{1}) P_{A1}(A_{2})P_{A1\cap A2}(A_{3})P_{A1\cap \ldots An-1}(A_{n})$
### Formule de probabilité totales 
- $P(B)=P(A)P_{A}(B)+P(\overline{A})P_{\overline{A}}(B)$ 
- Soit $(A_{i})_{i \in I}$  une système complet d'événements 
	- $\displaystyle P(B)=\sum_{i} P(A_{i}\cap B)= \sum P(A_{i})P_{Ai}(B)$ 
### Formule de Bayes 
Soit $(A_{i})_{i \in I}$ un système complet d'événements
- $\displaystyle\forall j \in I,\quad P_{B}(A_{j})= \frac{P(B \cap A_{j})}{P(B)}= \frac{P(A_{j})P_{Aj}(B)}{\sum_{i \in J} P(A_{i})P_{Ai}(B)}$ 

## Indépendance des événements 
- $A$ et $B$ indépendantes si $P(A \cap B)=P(A)P(B)$ 
- Si $A$ et $B$ indépendantes, $A$ et $\overline{B}$ indépendantes.  