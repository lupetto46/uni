# Spazio vettoriale
## Definizione
Prendiamo un insieme $V$ e due operazioni $(V, +, 0)$ un gruppo abeliano questo è considerabile spazio vettoriale se:
- $\forall v,w,u\in V, (v+w)+u=v+(w+u)$ l'addizione è associativa
- $\forall v \in V ,\quad v+0=v \qquad 0+v = v$  esiste un elemento neutro dell'addizione
- $\forall v \in V, \exists v' \in V : v+v'=0\qquad  v'+v=0 \qquad (v' := -v)$ esiste un elemento inverso
- $\forall v, v' \in V, \quad v+v'=v'+v$ l'addizione è commutativa

Inoltre assumiamo di avere una moltiplicazione sul campo $K$:

$$
\begin{align*}
    K &\longrightarrow V \\
    (\lambda, v) &\longmapsto \lambda \cdot v
\end{align*}
$$

E vogliamo che $\forall \lambda \in K, \forall v \in V, \lambda V\in V$
- $\forall \lambda\in K, \forall v, v' \in V,\qquad \lambda \cdot (v+v')=\lambda \cdot v + \lambda \cdot v'$ la moltiplicazione è distributiva rispetto alla somma da sinistra
- $\forall \lambda, \lambda' \in K, \forall v \in V, \qquad (\lambda + \lambda') \cdot v = \lambda \cdot v + \lambda' \cdot v$ la moltiplicazione è distributiva rispetto alla somma anche da destra
- $\forall \lambda, \lambda' \in K, \forall v \in V, \qquad (\lambda \cdot \lambda') \cdot v = \lambda \cdot (\lambda' \cdot v)$ 
- $\forall v \in V \quad 1 \cdot v = v$ esiste l'elemento neutro della moltiplicazione

Un insieme V con queste proprietà su un campo $K$ è detto spazio vettoriale su $K$ di cui:
- Gli elementi di $V$ sono detti vettori
- Gli elementi di $K$ sono detti scalari

### Esempi
L'esempio più base che si può fare con ciò di cui abbiamo già parlato sono le matrici. 

Infatti se consideriamo solo le matrici quadrate di ordine $n$ con le operazioni di somma e prodotto per uno scalare, queste formano uno spazio vettoriale.
$$(M_{n,n}, +, 0)$$
è un gruppo abeliano e quindi uno spazio vettoriale su $K$.

Altri esempi di spazi vettoriali su $K$ sono:
- $\{0\}$ chiamato spazio vettoriale nullo
- $K^n = \{(x_1, \dots, x_n) \mid x_i \in K\}$
	In quanto a questo spazio vettoriale si può dire che:
	- $(x_1, \dots, x_n) + (y_1, \dots, y_n) = (x_1 + y_1, \dots, x_n + y_n)$ e quindi si fa una somma componente per componente
	- $\lambda \cdot (x_1, \dots, x_n) = (\lambda x_1, \dots, \lambda x_n)$ e quindi si moltiplica ogni componente per lo scalare

Possiamo quindi notare come si somiglino: $K^n \cong M_{n,1}\cong M_{1,n}$

---
Un esempio un po' più complesso invece è:
Avendo $AX=0 \text{ sistema lineare omogeneo}, A\in M_{n,n}(K)$

$\Sigma_0 = \{\text{soluzioni di } AX=0\}$

avendo $\lambda \in K\qquad A(\lambda X) = \lambda (AX) = \lambda 0 = 0 \implies \lambda X \in \Sigma_0 \iff \Sigma_0$ è uno spazio vettoriale su $K$

---
Un altro esempio è:
$K[x]_n =$ polinomi su $K$ in una variabile $x$ di grado al più $n$

Avendo $f: \sum_{i=0}^n a_i x^i$ se si moltiplica la $f$ per uno scalare $\lambda \in K$ si ottiene: $\lambda f: \sum_{i=0}^n \lambda a_i x^i$


# Sottospazi vettoriali
Avendo uno spazio vettoriale $V$ su $K$ e un sottoinsieme $W \subseteq V$ si dice che $W$ è un sottospazio vettoriale di $V$ se:
- $\forall  v, w \in W, \quad v+w \in W$ sommando qualsiasi elemento del sottoinsieme si ottiene un elemento del sottoinsieme
- $\forall v \in W, \quad -v \in W$ per ogni elemento del sottoinsieme esiste il suo opposto sempre dentro il sottoinsieme
- $0 \in W$ si ha l'elemento neutro
- $\forall \lambda \in K, \forall v \in W, \quad \lambda v \in W$ la moltiplicazione tra un elemento del campo e un elemento del sottoinsieme ha come risultato un elemento del sottoinsieme ^e1fe11

## Come vedere se un sottoinsieme è un sottospazio vettoriale
Prendiamo di esempio:
- $\mathbb{R}=\mathbb{R}^1$ ed è quindi uno spazio vettoriale su $\mathbb{R}$.

	$\{0\}\subseteq \mathbb{R}$ è un sottospazio vettoriale di $\mathbb{R}$
- $\mathbb{Z} \subseteq \mathbb{R}$ non è un sottospazio vettoriale di $\mathbb{R}$
	In quanto se prendiamo di esempio $\sqrt{2}\cdot 1 = \sqrt{2} \notin \mathbb{Z}$ non rispettando il punto [[#^e1fe11|4]] per diventare uno spazio vettoriale.
- Nell'insieme $\mathbb{R}_{\geq 0}$ 
	
	$\{(0, \mu)\mid \mu \in \mathbb{R}\}$ è un sottospazio vettoriale di $\mathbb{R}^2$ in quanto se moltiplicato per uno scalare $\lambda \in \mathbb{R}$ si ottiene: $\lambda(0, \mu) = (0, \lambda \mu) \in \mathbb{R}_{\geq 0}$

> [!success] Proposizione
> Sia $V$ uno spazio vettoriale su $K, W \subseteq V$
>
> $W$ un sottospazio $\iff \forall \lambda, \lambda' \in K, \forall v, v' \in W$ si ha che $\lambda'v'+\lambda v \in W$

## Intersezioni e unioni di sottospazi
Avendo $V$ uno spazio vettoriale e $W_1,W_2\subseteq V$ sottospazi vettoriali di $V$. Possiamo farci due cose con questi insiemi:
- Intersecarli: $W_1 \cap W_2$
- Unirli: $W_1 \cup W_2$

Ma la domanda adesso è: $W_1 \cap W_2$ e $W_1 \cup W_2$ sono sottospazi vettoriali?

Provare che $W_1 \cap W_2$ è un sottospazio vettoriale di $V$

Il fatto che $W_1 \cap W_2$ è un sottospazio vettoriale di $V$ è equivalente a dire che:
$\forall \lambda, \lambda' \in K, \forall v, v' \in W_1 \cap W_2$ si ha che $\lambda'v'+\lambda v \in W_1 \cap W_2$

Sappiamo quindi che $v, v'$ appartengono sia a $W_1$ che a $W_2$ e che quindi $\lambda'v'+\lambda v \in W_1$ e $\lambda'v'+\lambda v \in W_2$ giungendo alla proposizione:

> [!success] Proposizione
> Avendo una famiglia di sottospazi vettoriali
> 
> $$
> 	\{W_i\}_{i\in I}
> $$
> Si ha che $\bigcap_{i\in I} W_i$ è un sottospazio vettoriale di $V$

> [!todo] Dimostrazione
> Provare che $W_1 \cup W_2$ è un sottospazio vettoriale di $V$
> 
> Proviamo a fare un esempio:
> 
> Prendiamo $V=\mathbb{R}^2,\quad W_1=\{(\lambda,0)\mid \lambda\in \mathbb{R}\},\quad W_2=\{(0,\mu)\mid \mu\in \mathbb{R}\}$
> 
> L'unione dei due sarebbe $W_1 \cup W_2=\{(\lambda,0), (0,\mu)\mid \lambda, \mu\in \mathbb{R}\}$ ma se facciamo l'unione prendendo come esempio $(1,0)\cup(0,1)$ otteniamo $(1,1)$ ma la coppia $(1,1)$ non si trova all'interno dell'unione in quanto in essa se c'è un valore a sinistra non c'è un valore a destra e viceversa.

# Somma di sottospazi
Ma per far funzionare l'unione si è deciso di utilizzare la somma di sottospazi. Ma prima di parlare di somma di sottospazi è necessario parlare di insiemi di combinazioni lineari di elementari $S$.

$$
    <S> = \left\{\sum_{i=1}^{n}\lambda_i \cdot v_i\mid m\in \mathbb{N}, \lambda_i \in K, v_i\in S\right\}
$$

> [!success] Notazione
> $S=\{v_1, v_2, \dots, v_n\},\quad <S>=<v_1, v_2, \dots, v_n>$

In poche parole una combinazione lineare non è altro che un valore raggiungibile tramite la somma di vettori moltiplicati per degli scalari.

> [!hint] Esempio
> Avendo il vettore $v_1=(1, 0, 3)$ e $v_2=(2, 0, 1)$ una combinazione lineare di questi due vettori è: $(3, 0, 4)$ in quanto si può ottenere attraverso $(1,0,3) + (2, 0, 1)$
> 
> Mentre invece $(1, 1, 4)$ non è una combinazione lineare di $v_1$ e $v_2$ in quanto non è possibile ottenere questo vettore sommando $v_1$ e $v_2$. Questo perché entrambi i vettori hanno il secondo valore  uguale a $0$ mentre $(1, 1, 4)$ ha il secondo valore diverso da $0$ non permettendo quindi di trovare uno scalare che moltiplicato per $0$ da un numero che permette di raggiungere $1$.

## Somma al posto dell'unione
Avendo $V$ uno spazio vettoriale e $W_1,W_2\subseteq V$ sottospazi vettoriali di $V$.

Identifichiamo la somma $W_1 + W_2$ con l'unione $<W_1 \cup W_2>$

> [!success] Lemma
> $$
> 	W_1 + W_2 = \left\{w_1 + w_2\mid w_1\in W_1, w_2\in W_2\right\}
> $$
> 
> Questo lemma definisce la somma di due sottospazi vettoriali $W_1$ e $W_2$ come l'insieme di tutti i vettori che si possono ottenere sommando un vettore di $W_1$ con un vettore di $W_2$. In altre parole, è l'insieme di tutte le possibili combinazioni di un elemento preso da $W_1$ e un elemento preso da $W_2$.

Possiamo quindi estendere la definizione di famiglia di sottospazi vettoriali:
$$
    \left\{W_i\right\}_{i\in I} \text{ sottospazi di } V
$$

$$
+_{i\in I}\ W_i = \left\{\sum_{i\in I} w_i\mid w_i\in W_i\right\}=\left\{<\bigcup_{i\in I}>W_i\right\}
$$


> [!success] Esempio
> $W_1=\{(\lambda, 0)\mid \lambda\in \mathbb{R}\}, w_2=\{(0,\mu)\mid \mu\in \mathbb{R}\}\subseteq \mathbb{R}^2$
> 
> $<W_1 \cup W_2>=W_1 + W_2 \subseteq \mathbb{R}^2 \iff \mathbb{R}^2=W_1 + W_2$
> 
> Di cui $W_1 + W_2 = (\lambda, \mu)$

# Generatori di sottospazi
Sia $V \text{ uno spazio vettoriale su } K,\quad S\subseteq V$ si diche che 

$S \text{ genera } V \text{ se } <S>=V$
In questo caso $S$ è chiamato generatore di $V$

Quindi $<S>$ è un insieme di generatori di $V$ se:
- $S=\{v_1, v_2, \dots, v_n\}$ e $<S>=V$ quindi se tutti i vettori di $V$ sono generato dai vettori contenuti in $S$.
- $\forall v \in V \exists \lambda_1, \lambda_2, \dots, \lambda_n \in K \text{ tali che } v=\lambda_1v_1+\lambda_2v_2+\dots+\lambda_nv_n$ Quindi esistono degli scalari che permettono di ottenere qualsiasi vettore di $V$ attraverso la somma dei vettori di $S$

> [!example] Esempio
> $<(0,1), (1,0)>=\mathbb{R}^2$
>
> Considerando che \{(0,1), (1,0)\} genera $\mathbb{R}^2$ in quanto moltiplicando $(0,1)$ e $(1,0)$ per due lambda diversi sono in grado di ottenere qualsiasi valore di $\mathbb{R}^2$

### Sistema linearmente indipendente
Un sistema è detto linearmente indipendente se:
- $\forall v_1, v_2, \dots, v_n \in S, \forall \lambda_1, \lambda_2, \dots, \lambda_n \in K$ tutti i vettori appartengono al sistema di generatori $S$ e se tutti gli scalari appartengono al nostro campo
- $\lambda_1v_1+\lambda_2v_2+\dots+\lambda_nv_n=0 \implies \lambda_1=\lambda_2=\dots=\lambda_n=0$ se la somma di tutti i vettori moltiplicati per lambda è uguale a 0 allora tutti i lambda sono uguali a 0. Importante ricordare che se c'è anche solo una situazione in cui anche solo un lambda è diverso da 0 ma la somma è uguale a 0 allora il sistema è detto **linearmente dipendente**

# Base di uno spazio vettoriale

Sia $V$ uno spazio vettoriale su $K$. $B\subseteq V$ è una base di $V$ se:
- $<B>=V$ è un insieme di generatori di $V$
- $V$ linearmente indipendente

> [!success] Corollario
> $B\subseteq V$ è una base di $V$ se e solo se:
> $$
> v\in V \exists! \lambda_1, \lambda_2, \dots, \lambda_n \in K : v = \sum_{i=1}^{n} \lambda_i \cdot v_i
> $$
> 
> Se prendendo un vettore di $V$ esiste una sola combinazione di scalari che permette di ottenere quel vettore attraverso la somma dei vettori di $B$.

> [!success] Proposizione
> Sia $V$ uno spazio vettoriale ed $S=\{v_1, v_2, \dots, v_n\}$ un insieme di generatori di $V$. Allora $S$ contiene $r\leq n$ vettori che formano una base di $V$.
> - Nel caso in cui si rispetta l'eguaglianza $r=n$ allora $S$ è una base di $V$.
> - Nel caso in cui si rispetta la diseguaglianza $r<n$ allora $S$ non è una base di $V$.

## Teorema di Steinitz

> [!success] Teorema
> $V$ uno spazio vettoriale su $K$. $\{v_1, v_2, \dots, v_n\}$ un insieme di generatori di $V$.
> 
> Se $\{w_1, w_2, \dots, w_r\}$ è un insieme di generatori di $V$ con $r<n$ allora esiste un insieme di generatori $\{w_1, w_2, \dots, w_r, v_{r+1}, \dots, v_n\}$ di $V$ con $r+1\leq n$

> [!success] Corollario
> $V=K^n=\{(x_1,, x_2, \dots, x_n)\mid x_i\in K\}$
> $$
> 	\left\{\begin{pmatrix} 1 \\ 0 \\ \vdots \\ 0 \end{pmatrix}, \begin{pmatrix} 0 \\ 1 \\ \vdots \\ 0 \end{pmatrix}, \begin{pmatrix} 0 \\ 0 \\ \vdots \\ 1 \end{pmatrix}\right\}
> $$
> La dimensione della base anche chiamata $\dim$ è uguale a $n$.
> Quindi:
> $$
> 	\dim K^n = n
> $$
> ovvero il numero di elementi che c'è all'interno di un vettore

Un esempio con le matrici può essere:

$$
	M_{2,2} (K)=\left\{\begin{pmatrix}
		a, b \\
		c, d
	\end{pmatrix} \mid a,b,c,d \in K\right\}
$$
La sua base sarebbe:
$$
        \left\{\begin{pmatrix} 1, 0 \\
            0, 0
        \end{pmatrix},\begin{pmatrix}
            0, 1 \\
            0, 0
        \end{pmatrix}, \begin{pmatrix}
            0, 0 \\
            1, 0
        \end{pmatrix}, \begin{pmatrix}
            0, 0 \\
            0, 1
        \end{pmatrix}\right\}
$$
Quindi la dimensione della base è uguale al numero di elementi all'interno della matrice quindi $\dim(M_{2,2}(K))=2\cdot2 = 4$.
Giungendo alla conclusione che: $\dim M_{m,n}(K)=m\cdot n$

> [!success] Proposizione
> $V$ spazio vettoriale, $W\subseteq V$ sottospazio vettoriale $\exists U\subseteq V$ sottospazio tale che $U\oplus W = V$
> 
> In poche parole se si ha un sottospazio vettoriale si avrà un secondo sottospazio vettoriale che se sommato al primo restituisce l'intero spazio vettoriale (simile al complementare)
> > [!todo] Dimostrazione
> > Avendo una $W=\{w_1, w_2,\dots,w_r\}\subseteq V$ linearmente indipendente
> > 
> > Allora $\exists n-r$ vettori $U=\{u_{1}, \dots, u_{n-r}\}$ tali che $\{w_1,\dots, w_r,u_1,\dots, u_{n-r}\}$
> > 
> > $\implies <u_1, u_2, \dots, u_{n-r}>=: U \implies U\oplus W = V$

# rappresentazioni (o forme) di sottospazi vettoriali

## Forma cartesiana e parametrica
Per rappresentare i sottospazi vettoriali ci sono due modi. 
Ognuno di questi ha i suoi pro e i suoi contro di cui ne parleremo dopo

### Forma cartesiana
$$
    V= \begin{cases}
        a_{11}x_1 + \dots + a_{1n}x_n = 0\\
        \vdots \\
        a_{m1}x_1 + \dots + a_{mn}x_n = 0
    \end{cases}= AX=0 =: ker(A)
$$

Di cui $A$:
$$
    A = \begin{pmatrix}
        a_{11} & \dots & a_{1n}\\
        \vdots & \ddots & \vdots\\
        a_{1m} & \dots & a_{mn}
    \end{pmatrix} \in M_{m,n}(K)
$$

E il kernel di $A$ ($ker(A)$) è l'insieme di tutti i vettori di $X$ tali che $AX=0$

### Forma parametrica
Ci si riferisce invece alla forma parametrica come $<v_1, v_2, \dots, v_r>$
E viene definito come $row(B)$ ovvero una matrice formata da tutti i vettori all'interno dell'insieme coricati riga per riga
$$
    <v_1, v_2, \dots, v_r> =: row (B), B = \begin{pmatrix}
        V_1\\
        V_2\\
        \vdots\\
        V_r
    \end{pmatrix}
$$

# Calcolare la base dello spazio vettoriale
## Forma cartesiana
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

## Forma parametrica
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

## Passaggio di forma
### Parametrica $\rightarrow$ cartesiana
$V \subseteq K^n$ spazio vettoriale.
Per passare dalla forma cartesiana alla forma parametrica è necessario innanzitutto prendere il vettore $V$ che è uguale al $\ker(A)$ di cui $A\in M_{m,n}$ trovare la base $\{b_1, \dots, b_r\}$ di $V$

Otteniamo quindi che $V=<v_1, \dots, v_r> = row(B)$ di cui $B$ è la matrice contenente tutti i vettori coricati $B=\begin{pmatrix} b_1\\ \vdots\\ b_r \end{pmatrix}$

### cartesiana $\rightarrow$ parametrica
$V \subseteq K^n,\quad V=<v_1, \dots, v_n> = row(A), A = \begin{pmatrix} v_1\\ \vdots\\ v_n \end{pmatrix}\in M_{m,n}(K)$

Per poter fare questa cosa è necessaria una proposizione:
> [!success] Proposizione
> Siano $A,B$ due matrici $\ker(A)=row(B)\iff \ker(B) = row(A)$

# Pro e contro di queste forme 
## Somma di sottospazi (forma cartesiana)
