## Cos'è una radice?
Una radice è una tabella rettangolare di elementi ordinati
Si rappresenta come:
$$
m
\underbrace{
\cases{\begin{matrix}
a_{11} &a_{12} &a_{13} &a_{14}&...&a_{1n}\\
a_{21} &a_{22} &a_{23} &a_{24}&...&a_{2n}\\
.&.&.&.&.&.\\
.&.&.&.&.&.\\
.&.&.&.&.&.\\
a_{m1}&a_{m2}&a_{m3}&a_{m4}&a_{m5}&a_{mn}
\end{matrix}
}
}_n
$$

Oppure $(a_{ij})_{\begin{align}1\leq i\leq n\\1\leq j\leq m\end{align}}$ ricordare che bisogna dire prima le righe e poi le colonne (*prima y poi x*)

Oppure $A\in M_{m,n}(S)={matrice\ m\times n \ con\ entrate\ in\ S\brace}, \text{ un insieme}$

Per noi $S=K$ quindi un campo

Per esempio una matrice:
$$
M_{2,2}(ℝ)={\begin{Bmatrix}\begin{pmatrix}
a,b\\ c,d
\end{pmatrix} a,b,c,d\inℝ\end{Bmatrix}}
$$

> [!important] Importante
> Le dimensioni di una matrice sono attributi fondamentali e quindi si *devono scrivere sempre* e sono quasi sempre la *prima cosa da guardare*

Una matrice si dice quadrata quando il numero di righe è uguale a quello delle colonne $m=n$
Quindi : $A=(a_{i,j})\in M{n,n} (ℝ)$

- $A$ viene chiamata triangolare superiore se $\forall i>j\qquad a_{i,j}=0$
$$
\begin{Bmatrix}
&a_{11} &n &n &n\\
&0 &\ddots &n &n\\
&0 &0 &\ddots &n\\
&0 &0 &0 &a_{nn}\\
\end{Bmatrix}
$$
- $A$ viene chiamata triangolare inferiore se $\forall i<j\qquad a_{i,j}=0$
$$
\begin{Bmatrix}
&a_{11} &0 &0 &0\\
&n &\ddots &0 &0\\
&n &n &\ddots &0\\
&n &n &n &a_{nn}\\
\end{Bmatrix}
$$
- $A$ viene chiama diagonale se $\forall i\neq j\qquad a_{i,j}=0$
$$
\begin{Bmatrix}
&a_{11} &0 &0 &0\\
&0 &\ddots &0 &0\\
&0 &0 &\ddots &0\\
&0 &0 &0 &a_{nn}\\
\end{Bmatrix}
$$

- Una matrice di cui tutte le entrato sono 0 si dice matrice nulla
- Una matrice diagonale di cui tutte le entrate della diagonale sono 1 si chiama identità di ordine n
$$
id_n=\begin{Bmatrix}
&1&0&0&\dots&0\\
&0&1&0&\dots&0\\
&0&0&1&\dots&0\\
&\vdots&\vdots&\vdots&\ddots&0\\
&0&0&0&\dots&1
\end{Bmatrix}
$$

## La trasposta di una matrice
Presa una matrice $A=(a_{i,j})\in M_{m,n}\in (K)$
Si può definire la trasposta $A^t=(a_{j,i})_{\eqalign{1\leq j\leq n\\1\leq i\leq m}}\in M_{n,m}$
> [!question] Quando due matrici sono uguali?
> Avendo due matrici $A\in M_{m,n}(K),\quad A'\in M_{l,h}(K)$
> $A=B\Longleftrightarrow m=l, h=n$ e $\forall i,j\ a_{ij}=b_{ij}$

Dalla trasposta si ottiene il concetto di simmetrica
$A$ è simmetrica se $A^t=A$ capendo anche che una matrice simmetrica è sicuramente quadrata

> [!success] Lemma
> $A\in M_{m,n}(K)$ simmetrica allora $m=n$ $\forall i,j\in \{1,\dots,n\}\ a_{ij}=a{ij}$


## Operazioni tra matrici
### Somma tra matrici
