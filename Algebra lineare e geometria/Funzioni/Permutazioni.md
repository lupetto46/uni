Cos'è una permutazione.
$S$ un insieme finito $\#S=n, S=\{a_1,\cdots,a_n\}\rightarrow\{1,2,\cdots,n\}$

Quindi $S=\{1,2,3,\cdots,n\}$

Una permutazione è una funzione $\sigma:S\longrightarrow S$
Se questo sigma ($\sigma$)  è una permutazione $\Leftrightarrow$ è biiettiva

### Ma cosa fa?
Una permutazione è semplicemente una funzione che cambia l'ordine dell'insieme.
Si scrive $\sigma:(\sigma(1)\ \sigma(2)\ \sigma(3)\ \sigma(4)\cdots \sigma(n))$

Ricordare che nella funzione sigma non c'è scritto il valore di un posto ma il posto del valore di prima

$\sigma:(2\ 4\ 1\ 3)$ vuol dire:
- Il numero nella posizione $2$ va nella posizione $1$
- Il numero nella posizione $4$ va nella posizione $2$
- Il numero nella posizione $1$ va nella posizione $3$
- Il numero nella posizione $3$ va nella posizione $4$

Avendo $\sigma:(2\ 4\ 1\ 3)$
L'inverso di $\sigma$ è la funzione che rimette tutti i numeri al suo posto:
$\sigma^{-1}:(3\ 1\ 4\ 2)$ che significa:
- Il valore che deve stare alla posizione $1$ prendilo dalla posizione $3$
- Il valore che deve stare alla posizione $2$ prendilo dalla posizione $1$
- Il valore che deve stare alla posizione $3$ prendilo dalla posizione $4$
- Il valore che deve stare alla posizione $4$ prendilo dalla posizione $2$

> [!info] Dimostrazione
> Dimostrare che l'insieme delle possibili permutazioni di $S$ : $(\#\$_n)$ è $n!$
> Proposizione: $(\$_n, \circ)$ è un gruppo
> Dimostrazione: $\$_n=\{\text{permutazioni di }\{1,\dots,4\}\}$ 
> innanzitutto si sceglie la posizione di $\sigma(1)\in \{1,\dots,4\}$
> Poi si sceglie la posizione di $\sigma(2)\in\{\backslash\sigma(1)\}$ perché $\sigma(1)$ è *già stato scelto*
> E così via finché non scelgo il $\sigma(n-1)$ ottenendo che:
> $\#\$_n=n\cdot(n-1)\cdot(n-2)\cdotp ...\cdot (n-(n-1))=n!$

Abbiamo detto che avendo $S = \{1,2,\dots,n\}$ e $\$_n$ l'insieme di tutte le permutazioni di $S$ possiamo definire una permutazione come una funzione biiettiva da $S$ a $S$.
Quindi $\sigma \in \$_n$ è una funzione biiettiva da $S$ a $S$.

### Inversioni nella permutazione
Una inversione in una permutazione $\sigma \in \$_n$ è una coppia $(i,j)$ tale che $i<j$ e $\sigma(i)>\sigma(j)$ ed è indicato con $i(\sigma)$. Quindi:
$$
	S = \{1,2,3,4,5\},\qquad \sigma = (2\ 4\ 1\ 3\ 5),\qquad i(\sigma) = 3
$$

Questo perché il $2$ che si trova nella prima posizione è maggiore dell'$1$ che sta d'avanti a lui. Poi il $4$ è maggiore dell'$1$ e del $3$ che stanno davanti a lui.  Sommando le situazioni in cui un numero si trova dietro a un numero più piccolo di lui otteniamo che questa cosa succede $3$ volte.
### Il segno della permutazione
Il segno di una permutazione $\sigma \in \$_n$ è definito come: $sign(\sigma) := (-1)^{i(\sigma)}$
Sarà quindi:
$$
    sign(\sigma) = \begin{cases}
        1 & \text{se $i(\sigma)$ è pari}\\
        -1 & \text{se $i(\sigma)$ è dispari}
    \end{cases}
$$

> [!summary] Proposizione
> $\sigma, \tau \in \$ \text{ allora }  sign(\sigma \circ \tau) = sign(\sigma)\cdot sign(\tau)$
> 
> $sign(\sigma^{-1}) = sign(\sigma)$