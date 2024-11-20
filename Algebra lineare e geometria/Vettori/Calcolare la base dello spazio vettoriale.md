#### Forma cartesiana
Preso il sistema lineare omogeneo si trova la matrice associata $A$:
$$
    V= \begin{cases}
        a_{11}x_1 + \dots + a_{1n}x_n = 0\\
        \vdots \\
        a_{m1}x_1 + \dots + a_{mn}x_n = 0
    \end{cases} \longrightarrow A=(a_{ij})
$$

Dopodiché si esegue Gauss-Jordan (\ref{subsubsec:Gaus-Jordan}) e si ottiene la matrice in forma
di Echelon ridotta.
Dopodiché si prendono tutti i pivot e si inserisce a sistema il valore della variabile a cui corrisponde e al secondo membro il valore delle variabili delle colonne dopo.

$$
    \begin{cases}
        x_1 = b_{11}x_{r+1} + \dots + b_{1,r-n}x_{n}\\
        \vdots\\
        x_r = b_{r1}x_{r+1} + \dots + b_{r,r-n}x_{n}
    \end{cases}
$$

Si mettono quindi in unico vettore tutte le variabili delle colonne (per nome)
$$
    \begin{cases}
        x_1 = b_{11}x_{r+1} + \dots + b_{1,r-n}x_{n}\\
        \vdots\\
        x_r = b_{r1}x_{r+1} + \dots + b_{r,r-n}x_{n}
    \end{cases}=
    \begin{pmatrix}
        x_1\\
        \vdots\\
        x_r\\
        x_{r+1}\\
        \vdots\\
        x_n
    \end{pmatrix}
$$

Poi si mette l'espressione che è stata messa dopo l'uguale
$$
    \begin{cases}
        x_1 = b_{11}x_{r+1} + \dots + b_{1,r-n}x_{n}\\
        \vdots\\
        x_r = b_{r1}x_{r+1} + \dots + b_{r,r-n}x_{n}
    \end{cases}=
    \begin{pmatrix}
        x_1\\
        \vdots\\
        x_r\\
        x_{r+1}\\
        \vdots\\
        x_n
    \end{pmatrix} =
    \begin{pmatrix}
        b_{11}x_{r+1} + \dots + b_{1,r-n}x_{n}\\
        \vdots\\
        b_{r1}x_{r+1} + \dots + b_{r,r-n}x_{n}\\
        x_{r+1}\\
        \vdots\\
        x_n
    \end{pmatrix}
$$

Prendo i coefficienti di una variabile e li inserisco in un vettore moltiplicato per quella variabile

$$
    \underbrace{\begin{pmatrix}
        b_{11}\\
        b_{21}\\
        \vdots\\
        b_{r1}\\
        1\\
        0\\
        \vdots\\
        0
    \end{pmatrix}, \begin{pmatrix}
        b_{12}\\
        b_{22}\\
        \vdots\\
        b_{r2}\\
        0\\
        1\\
        \vdots\\
        0
    \end{pmatrix}, \dots , \begin{pmatrix}
        b_{1,n-r}\\
        b_{2,n-r}\\
        \vdots\\
        b_{r,n-r}\\
        0\\
        0\\
        \vdots\\
        1
    \end{pmatrix}}_{n-r \text{ base di } V}
$$
Quest'ultima parte è quindi la base di $V$ di cui la lunghessa sarebbe $n-r$ di cui $r$ è uguale al rango della matrice associata $r=rk(A)$

Inoltre $ker(A)= V$ quindi  il kernel della matrice associata è tutto lo spazio vettoriale 
> [!example] Esempio
> $$
> 	V=\begin{cases}
> 		x_1 + 2x_2 - 3x_3 = 0\\
> 		x_1 + x_2  - 4x_4 = 0\\
> 		x_2 - 3x_3 + 4x_4 = 0 
> 	\end{cases}
> $$
> $$
> 	A=\begin{pmatrix}
> 		1 & 2 &-3 & 0\\
> 		1 & 1 &0 & -4\\
> 		0 & 1 &-3 & 4\\
> 	\end{pmatrix} \xrightarrow{r_2 \rightarrow r_2-r_1} \begin{pmatrix}
> 		1 & 2 &-3 & 0\\
> 		0 & -1 &3 & -4\\
> 		0 & 1 &-3 & 4\\
> 	\end{pmatrix}
> $$
> $$
> 	\xrightarrow{r_2\rightarrow -1\cdot r_2}\begin{pmatrix}
> 		1 & 2 &-3 & 0\\
> 		0 & 1 &-3 & 4\\
> 		0 & 1 &-3 & 4\\
> 	\end{pmatrix} \xrightarrow{r_3 \rightarrow r_3 - r_2} \begin{pmatrix}
> 		1 & 2 & -3 & 0\\
> 		0 & 1 & -3 & 4\\
> 		0 & 0 & 0 & 0\\
> 	\end{pmatrix}
> $$
> $$
> 	\xrightarrow{r_1 \rightarrow r_1 - 2r_2}\begin{pmatrix}
> 		1 & 0 & 3 & -8\\
> 		0 & 1 & -3 & 4\\
> 		0 & 0 & 0 & 0\\
> 	\end{pmatrix} = \begin{cases}
> 		x_1 = -3x_3 + 8x_4\\
> 		x_2 = 3x_3 -4x_4
> 	\end{cases}
> $$
> $$
> 	=\begin{pmatrix}
> 		x_1\\
> 		x_2\\
> 		x_3\\
> 		x_4
> 	\end{pmatrix} = \begin{pmatrix}
> 		-3x_3 + 8x_4\\
> 		3x_3 - 4x_4\\
> 		x_3\\
> 		x_4
> 	\end{pmatrix} = \begin{pmatrix}
> 		-3\\
> 		3\\
> 		1\\
> 		0
> 	\end{pmatrix}x_3 + \begin{pmatrix}
> 		8\\
> 		-4\\
> 		0\\
> 		1
> 	\end{pmatrix} \implies 
> $$
> $$
> 	\implies V = <\begin{pmatrix}
> 		-3\\
> 		3\\
> 		1\\
> 		0
> 	\end{pmatrix},\begin{pmatrix}
> 		8\\
> 		-4\\
> 		0\\
> 		1
> 	\end{pmatrix}>
> $$

### Forma parametrica
Per calcolare la base invece tornando dalla forma parametrica è un po' più complicato.

Avendo $V \subseteq K^n$ e $V = <v_1, \dots, v_m>$ innanzitutto bisogna assicurarsi che siano linearmente indipendenti:
Per fare questo basta eseguire l'algoritmo di Gauss (non è necessaria la parte di Jordan) sulla matrice:

$$
    B = \begin{pmatrix}
        v_1\\
        \vdots\\
        v_m
    \end{pmatrix} \in M_{m,n}(K)
$$

Ottenendo quindi una matrice $A$ in forma di Echelon.
Con la matrice $A$ otteniamo quindi delle righe nulle e non nulle. Le righe non nulle formeranno la una base di $V$

Possiamo quindi giungere alla conclusione che la dimensione di $V$ è uguale al rango della matrice $B$ ($dim(V)=rk(B)$) e che per definizione $V = row(B)$ ovvero una matrice le cui righe sono i vettori scritti in orizzontale.
> [!example] Esempio
> $$
>         V=<\begin{pmatrix}
>             1\\
>             1\\
>             2
>         \end{pmatrix},\begin{pmatrix}
>             0\\
>             0\\
>             1
>         \end{pmatrix},\begin{pmatrix}
>             1\\
>             1\\
>             1
>         \end{pmatrix}>
> $$
> $$
>         B= \begin{pmatrix}
>             1 & 1 & 2\\
>             0 & 0 & 1\\
>             1 & 1 & 1\\
>         \end{pmatrix} \xrightarrow{r_3\rightarrow r_3 - r_1} \begin{pmatrix}
>             1 & 1 & 2\\
>             0 & 0 & 1\\
>             0 & 0 & -1\\
>         \end{pmatrix}\xrightarrow{r_3 \rightarrow r_3 - r_2} \begin{pmatrix}
>             1 & 1 & 2\\
>             0 & 0 & 1\\
>             0 & 0 & 0\\
>         \end{pmatrix}
> $$
> $$
>         rk(B)=2 = <\begin{pmatrix}
>             1\\
>             1\\
>             2
>         \end{pmatrix},\begin{pmatrix}
>             0\\
>             0\\
>             1
>         \end{pmatrix}> \text{ base di }V
> $$

> [!success] Teorema
> Teorema (del rango)
> Avendo una matrice $A\in M_{m,n}(K)$:
> - $rk(A) =: r$
> - $\dim(\ker(A)) = n - r$ e viene anche definito come nullità di $A$ quindi $\dim(\ker(A))=: null(A)$
> 
> Otteniamo quindi che $null(A)+rk(A)=n$

^a5f396

### Passaggio di forma
#### Parametrica $\rightarrow$ cartesiana
$V \subseteq K^n$ spazio vettoriale.
Per passare dalla forma cartesiana alla forma parametrica è necessario innanzitutto prendere il vettore $V$ che è uguale al $\ker(A)$ di cui $A\in M_{m,n}$ trovare la base $\{b_1, \dots, b_r\}$ di $V$

Otteniamo quindi che $V=<v_1, \dots, v_r> = row(B)$ di cui $B$ è la matrice contenente tutti i vettori coricati $B=\begin{pmatrix} b_1\\ \vdots\\ b_r \end{pmatrix}$

#### Cartesiana $\rightarrow$ parametrica
$V \subseteq K^n,\quad V=<v_1, \dots, v_n> = row(A), A = \begin{pmatrix} v_1\\ \vdots\\ v_n \end{pmatrix}\in M_{m,n}(K)$

Per poter fare questa cosa è necessaria una proposizione:
> [!success] Proposizione
> Siano $A,B$ due matrici, $\ker(A)=row(B) \iff \ker(B) = row(A)$
> 
> $W = \ker(A \rightarrow \{b_1,\dots,b_r\}$ base di $W \implies W=\ker(A) = row(B),\ B=$
> $= \begin{pmatrix}b_1\\\vdots\\b_r\end{pmatrix} \implies row(A)=\ker(B) \implies V = \ker(B)$

##### Esercizio di esempio
$$
V=<\begin{pmatrix}
-1\\1\\2
\end{pmatrix},\begin{pmatrix}
0\\1\\0
\end{pmatrix}> = row\begin{pmatrix}
-1 & 1 & 2\\
0 & 1& 0
\end{pmatrix} = A
$$
$$
W:= \ker A
$$
$$
\begin{pmatrix}
-1 & 1 & 2\\
0 & 1& 0
\end{pmatrix} \xrightarrow{r_1 \rightarrow -1\cdot r_1} \begin{pmatrix}
1 & -1 & -2\\
0 & 1& 0
\end{pmatrix} \xrightarrow{r_1 \rightarrow r_1 + r_2} \begin{pmatrix}
1 & 0 & -2\\
0 & 1& 0
\end{pmatrix}
$$
$$
\begin{cases}
x_1 = 2x_3\\
x_2 = 0
\end{cases} \implies \begin{pmatrix}
x_1\\ x_2\\ x_3
\end{pmatrix}= \begin{pmatrix}
2x_3\\ 0 \\ x_3
\end{pmatrix} = \begin{pmatrix}
2 \\ 0 \\ 1
\end{pmatrix} x_3 \implies
$$
$$
\implies W = \ker A,\ A = <\begin{pmatrix}
2\\ 0\\ 1
\end{pmatrix}>
$$