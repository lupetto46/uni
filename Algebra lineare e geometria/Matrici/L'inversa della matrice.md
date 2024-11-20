Per ottenere l'inversa di una matrice è necessario prendere una matrice $A\in M_{n,n}(K)$ affiancarla all'$id_n$ e applicarci l'algoritmo di Gauss.

Se $(A|id_n)\in M_{n,2n}(K)$ dopo l'algoritmo Gauss-Jordan otteniamo $(id_n|B)$ e quindi $B=A^{-1}$

> [!done] Lemma
> Una matrice $A\in M_{n,n}(K)$ è invertibile se e solo se $rkA=n$
> Quindi il rango è massimale.