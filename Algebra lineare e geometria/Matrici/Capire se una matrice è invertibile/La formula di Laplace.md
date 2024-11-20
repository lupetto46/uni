Sia $A\in M_{n,n}(K),\quad i,j \in \{1, 2, \dots, n\}$

$A_{ij}\in M{n-1, n-1}(K)$ è la sottomatrice di $A$ ottenute eliminando la riga $i$-esima e la colonna $j$-esima.

Allora posiamo considerare $m_{ij}:=det A_{ij} =: |A_{ij}|$ minore di $A$ rispetto agli indici $(i,j)$

---
$$
    \text{Sia }A\in M_{n,n}(K).\quad \forall i \in \{1,2,\dots,n\}, \quad det A = \sum_{j=1}^n (-1)^{i+j}\cdot a_{ij}\cdot |A_{ij}|
$$
Analogamente per le colonne:
$$
    \forall j \in \{1, 2, \dots, n\}, \quad det A = \sum_{i=1}^n (-1)^{i+j}\cdot a_{ij}\cdot |A_{ij}|
$$
### Definizione generale
$A = (a_{ij})\in M_{n,n}(K). \quad \forall i,j\in\{1,2,,\dots,n\}$ definiamo $a_{ij}^* := (-1)^{i+j}\cdot |A_{ij}|$ il coefficiente di $a_{ij}$

Di conseguenza $A^* := adj(A) :=(a_{ij}^*)^t\in M_{n,n} (K)$

> [!success] Proposizione
> $$
> 	A\cdot A^* = det A \cdot id_n
> $$

> [!success] Corollario
> $$
> 	A^{-1} = \frac{A^*}{det A}
> $$


> [!success] Corollario
> Sia $A\in M_{n,n} (K)$
> $$
> 	A \text{ invertibile} \iff det A \neq 0 \iff rkA = n
> $$