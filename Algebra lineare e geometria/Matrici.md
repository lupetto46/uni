---
Data: 24-11-2024
---


# Matrici
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

## Insiemi di matrici con operazioni
Nel gruppo l'identità di ordine $n$ prende la forma di elemento neutro della moltiplicazione tra matrici.
$$
    A\cdot id_n=\left( \sum_{k=1}^{n}a_{ik}\cdot b_{kj} \right) =(a_{ij})=id_n\cdot A = A
$$
Ne segue quindi che
- $(M_{n,n},\cdotp,id_n)$ è un gruppo non abeliano.
- $(M_{n,n},+,\cdotp)$ è un anello non abeliano.

# L'inversa di una matrice
Per poter parlare di inversa di una matrice è necessario parlare dell'algoritmo di Gauss-Jordan.
## La forma di Echelon
Una matrice è in forma di Echelon se:
- Tutte le righe nulle si trovano in fondo alla matrice
- In ogni riga non nulla il primo elemento non nullo è da sinistra (chiamato pivot) è alla destra di tutti gli altri pivot delle righe precedenti.
- Tutte le entrate al di sotto di un pivot sono nulle.

Ottenendo quindi matrici in forma di Echelon:
$$
\begin{pmatrix}
	(1) & 0 & 3 & 2\\
	0 & (1) & 4 & 5\\
	0 & 0 & 0 & 7\\
	0 & 0 & 0 & (2)\\
\end{pmatrix}
$$
I numeri cerchiati sono i cosiddetti **pivot**

###  Forma di Echelon ridotta
Una matrice è in forma di Echelon ridotta se:
- La matrice è in forma di Echelon
- Ogni pivot è uguale a 1
- Ogni pivot è l'unico elemento non nullo della sua colonna

Ottenendo quindi matrici in forma di Echelon ridotta
$$
\begin{pmatrix}
	(1) & 0 & 3 & 0\\
	0 & (1) & 4 & 0\\
	0 & 0 & 0 & 0\\
	0 & 0 & 0 & (1)\\
\end{pmatrix}
$$

## Algoritmo di Gauss-Jordan
L'algoritmo di Gauss-Jordan è un algoritmo che permette di trasformare una matrice qualsiasi in forma di Echelon ridotta.

Questo algoritmo permette di utilizzare le operazioni elementari per trasformare una matrice in forma di Echelon ridotta. Queste operazioni elementari sono:

- Scambiare le righe
- Moltiplicare una riga per uno scalare non nullo
- Sostituire una riga con la somma tra se stessa e un'altra riga moltiplicata per uno scalare. $r_i+\alpha r_j, \alpha \in K, j\neq i$

Questo è diviso in 2 parti: La parte di Gauss e la parte di Jordan
### Gauss
- Trovare il primo elemento non nullo della prima colonna
- Scambiare la riga con il primo elemento non nullo con la prima riga della matrice
- Dividere tutta la prima riga per il valore del suo primo valore
- Controllare tutte le altre entrate della prima colonna e se si trova un elemento non nullo sottrarre quella riga con la prima riga moltiplicata per l'elemento non nullo
- Ottenere una matrice in questa forma:
$$
\begin{pmatrix}
	(1) & a_{12} & \dots & a_{1n}\\
	0 & b_{22} & \dots & b_{2n}\\
	\vdots &\vdots & \ddots & \vdots\\
	0 & b_{n2} & \dots & b_{nn}            
\end{pmatrix}
$$
- Prendere solo la matrice $B$:
$$
B=\begin{pmatrix}
	b_{22} & \dots & b_{2n}\\
	\vdots & \ddots & \vdots\\
	b_{n2} & \dots & b_{nn}                
\end{pmatrix}
$$
- Ripetere il procedimento con la matrice $B$
### Jordan
Una volta finito otteniamo un matrice in forma di Echelon.
Per trasformarla in forma di Echelon ridotta è necessario utilizzare l'algoritmo di Jordan sulla matrice.
- Prendere l'ultimo pivot che abbiamo trovato
- Prendere tutti i valori non nulli sopra il pivot e sottrarre le rispettive righe per la riga del pivot moltiplicata per l'elemento non nullo
- Eseguire la stessa cosa per ogni pivot dal basso verso l'alto

Finiti tutte queste operazioni otteniamo la matrice in forma di Echelon ridotta.

## Il rango di una matrice
Il rango di una matrice è il numero di pivot che ci sono all'interno di una matrice che è almeno in forma di Echelon.  Si identifica come: avendo $A\in M_{m,n}(K)$ il rango di $A$ è $rkA$

Il rango massimo di una matrice è il minimo tra $m$ e $n$ quindi $rkA\leq min\{m,n\}$

## L'inversa della matrice
Per ottenere l'inversa di una matrice è necessario prendere una matrice $A\in M_{n,n}(K)$ affiancarla all'$id_n$ e applicarci l'algoritmo di Gauss.

Se $(A|id_n)\in M_{n,2n}(K)$ dopo l'algoritmo Gauss-Jordan otteniamo $(id_n|B)$ e quindi $B=A^{-1}$

> [!done] Lemma
> Una matrice $A\in M_{n,n}(K)$ è invertibile se e solo se $rkA=n$
> Quindi il rango è massimale.

# Come capire se una matrice è invertibile a priori
## Permutazioni
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

## Il determinante
$A\in M_{n,n} (K)$ il determinante di $A$ è definito come:
$$
    det (A) = |A|:= \sum_{\sigma \in \$_n} sign(\sigma) \cdot \prod_{i=1}^n a_{i,\sigma(i)}
$$

### Proprietà del determinante
Se una matrice è triangolare o diagonale allora il determinante è il prodotto degli elementi sulla diagonale.
$$
    A \in M_{n,n} (K) \text{ se } A \text{ è triangolare o diagonale allora } det A= \prod_{i=1}^n a_{i,i}
$$

> [!success] Lemma
> Il $det A^t= det A$
> > [!todo] Dimostrazione
> > Avendo $A\in M_{n,n} (K),\quad i \in \{1,2,\dots,n\}$\\
> > $A^{(i)}=(a_{1,i}\ a_{2,i}\ \dots\ a_{n,i})$ Quindi $A^{(i)}$ è la $i$-esima riga di $A$
> > $$
> >             det A = \alpha\cdot det \begin{pmatrix} A^{(1)}\\ \vdots\\ V\\ \vdots\\ A^{(n)}\end{pmatrix} + \alpha'\cdot det \begin{pmatrix} A^{(1)}\\ \vdots\\ V'\\ \vdots\\ A^{(n)} \end{pmatrix}
> > $$

> [!success] Lemma
> Se $A'$ è la matrice ottenuta scambiando $2$ righe di $A$ allora  $det A' = -det A$

> [!success] Corollario
> Se $A$ è la matrice ottenuta applicando la permutazione $\sigma$ alle righe di $A$ allora $det A' = sign(\sigma) \cdot det A$

> [!success] Proposizione
> - Se $A^{(i)}= (0\ \dots\ 0)$ allora $det A = 0$
> - $\text{Se } \exists i\neq j : A^{(i)}=A^{(j)} \text{ allora } det A = 0$
> - $$\det \begin{pmatrix} A^{(1)}\\ \vdots\\ A^{(i)} + \alpha\cdot A^{(j)}\\ \vdots\\ A^{(n)}\\ \end{pmatrix} = \det \begin{pmatrix} A^{(1)}\\ \vdots\\ A^{(i)}\\ \vdots\\ A^{(n)}\\ \end{pmatrix} + \alpha \cdot det \begin{pmatrix} A^{(1)}\\ \vdots\\ A^{(j)}\\ \vdots\\ A^{(n)}\\ \end{pmatrix} = det A $$
> - In quanto $$ \alpha \cdot det \begin{pmatrix} A^{(1)}\\ \vdots\\ A^{(j)}\\ \vdots\\ A^{(n)}\\ \end{pmatrix} = 0 $$ Siccome $A^{(j)}$ prende il posto di $A^{(i)}$ troviamo che $A^{(i)}=A^{(j)}$ ma visto che abbiamo due righe identiche in quanto seguendo l'equazione \eqref{det:due righe identiche} otteniamo che è uguale a $0$ e quindi solo il $\det A$
> - $$\det \begin{pmatrix} A^{(1)}\\ \vdots\\ \alpha\cdot A^{(i)}\\ \vdots\\ A^{(n)}\\ \end{pmatrix}=\alpha\cdot\det A$$

> [!important] Importante
> Importante:
Visto che $\det A^t= \det A$ allora tutte le proprietà del determinante valgono anche per le colonne.

## Il teroema di Binet
$$
    A,B \in M_{n,n} (K), \quad det(A\cdot B) = det A \cdot det B
$$

### Dimostrazione
$A=(a_{ij}), \quad B = (b_{ij})$
$$
    \begin{align}
        A \cdot B &= \begin{pmatrix}
            a_{11}\cdot b_{11} + \dots + a_{1n}\cdot b_{n1} & \dots & a_{11}\cdot b_{1n} + \dots + a_{1n}\cdot b_{nn}\\
            \vdots & \ddots & \vdots\\
            a_{n1}\cdot b_{11} + \dots + a_{nn}\cdot b_{n1} & \dots & a_{n1}\cdot b_{1n} + \dots + a_{nn}\cdot b_{nn}\\
        \end{pmatrix}=\\
        &= \begin{pmatrix}
            a_{11}\cdot B^{(1)} + a_{12}\cdot B^{(2)} + \dots + a_{1n}\cdot B^{(n)}\\
            \vdots\\
            a_{n1}\cdot B^{(1)} + a_{n2}\cdot B^{(2)} + \dots + a_{nn}\cdot B^{(n)}\\
        \end{pmatrix}
    \end{align}
$$
Facendo lo stesso procedimento con le righe otteniamo che:
$$
        det A\cdot B = \sum_{j_1, \dots, j_n}^{n} a_1j_1\cdot \dots \cdot a_nj_n\cdot det \begin{pmatrix}
            B^{(j_1)}\\
            \vdots\\
            B^{(j_n)}\\
        \end{pmatrix}
$$
Ma visto che:
$$
        \Biggl(\underbrace{\sum_{\sigma \in \$} a_{\sigma(1)}\cdot \dots \cdot a_{\sigma(n)}}_{det A}\Biggr)\cdot det B= det A \cdot det B
$$

> [!success] Corollario
> $A\in M_{n,n}(K)$ invertibile $\Longrightarrow det A^{-1} = \frac{1}{det A}$
>
>$A^{-1}\cdot A = id_n,\qquad det(id_n) = 1$
>
> $det (id_n) = det A^{-1} \cdot det A$

> [!success] Corollario
> Se $A\in M_{n,n}(K)$ è invertibile $\Longrightarrow det A \neq 0$
> 
> Significa che se una matrice ha determinante 0 allora non è invertibile.

## La formula di Laplace
Sia $A\in M_{n,n}(K),\quad i,j \in \{1, 2, \dots, n\}$

$A_{ij}\in M{n-1, n-1}(K)$ è la sottomatrice di $A$ ottenute eliminando la riga $i$-esima e la colonna $j$-esima.

Allora posiamo considerare $m_{ij}:=det A_{ij} =: |A_{ij}|$ minore di $A$ rispetto agli indici $(i,j)$

## Teorema di Laplace
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

## Usare il determinante per capire qual è il rango di una matrice
Il problema più grande è quello che il rango è calcolabile in tutte le matrici, ma il determinante solo in quelle quadrate.

Per questo motivo dobbiamo vedere una serie di proposizioni

> [!success] Proposizione
> Sia $A\in M_{m,n}(K), B\in M_{m,r}(K)$
> - $rk(AB)\leq min(rk(A), rk(B))$.
> - Se $m=n$ e $A$ è invertibile allora $rk(AB) = rk(B)$.
> - Se $n=r$ e $B$ è invertibile allora $rk(AB) = rk(A)$.

> [!success] Proposizione
> Se $B$ è una sottomatrice di $A$, allora $rk(B)\leq rk(A)$

> [!success] Teorema
> $A\in M_{m,n}(K)$ allora $rkA=$ guardando tutte le sottomatrici quadrate si prende il rango della sottomatrice quadrata più grande che non ha determinante nullo.

