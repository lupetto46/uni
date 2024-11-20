### Somma tra matrici
La somma tra matrici è un’operazione che consiste nell’aggiungere le entrate corrispondenti di due matrici. Per esempio prendiamo due matrici della stessa dimensione: $A = (a_{ij})\in M_{m,n}(K)$ e $B = (b_{ij})\in M_{m,n}(K)$ quindi le matrici devono essere di stesse dimensioni.
$$
A+B = (a_{ij} + b_{ij})\in M_{m,n}, A+B = B+A
$$
La somma tra matrici è inoltre commutativa.

### Moltiplicazione tra una matrice e uno scalare

La moltiplicazione di una matrice e uno scalare è un'operazione che consiste nel moltiplicare ogni entrata della matrice per uno scalare. $A=(a_{ij})\in M_{m,n}(K), c \in K$
$$
c\cdot A = (c\cdot a_{ij})\in M_{m,n}(K)
$$
Quindi si moltiplica qualsiasi valore all'interno della matrice per quello scalare.

### Moltiplicazione tra matrici.
Per poter eseguire una moltiplicazione tra matrici è necessario che il numero delle colonne della prima matrice sia uguale al numero delle righe della seconda matrice.
Avendo le due matrici $A=(a_{ij})\in M_{m,n} (K)$ e $B=(b_{ij})\in M_{n,p} (K)$ per poter fare la moltiplicazione tra queste due matrici dobbiamo fare attenzione che la $n$ sia nelle colonne della matrice $A$ e nelle righe della matrice $B$.

La moltiplicazione viene definita come:
$$
A\cdot B = \left(\sum_{k=1}^{n}a_{ik}\cdot b_{ik}\right)_{\overset{1\leq j\leq p}{1\leq i \leq m}} \in M_{m,p}(K)
$$
E non è commutativa.