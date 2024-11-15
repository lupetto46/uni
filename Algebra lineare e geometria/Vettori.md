---
Data: 24-11-2024
tags: Algebra_lineare_e_geometria
---


# Vettori
## Spazio vettoriale
### Definizione
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

#### Esempi
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


## Sottospazi vettoriali
Avendo uno spazio vettoriale $V$ su $K$ e un sottoinsieme $W \subseteq V$ si dice che $W$ è un sottospazio vettoriale di $V$ se:
- $\forall  v, w \in W, \quad v+w \in W$ sommando qualsiasi elemento del sottoinsieme si ottiene un elemento del sottoinsieme
- $\forall v \in W, \quad -v \in W$ per ogni elemento del sottoinsieme esiste il suo opposto sempre dentro il sottoinsieme
- $0 \in W$ si ha l'elemento neutro
- $\forall \lambda \in K, \forall v \in W, \quad \lambda v \in W$ la moltiplicazione tra un elemento del campo e un elemento del sottoinsieme ha come risultato un elemento del sottoinsieme ^e1fe11

### Come vedere se un sottoinsieme è un sottospazio vettoriale
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

### Intersezioni e unioni di sottospazi
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

## Somma di sottospazi
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

### Somma al posto dell'unione
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

## Generatori di sottospazi
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

#### Sistema linearmente indipendente
Un sistema è detto linearmente indipendente se:
- $\forall v_1, v_2, \dots, v_n \in S, \forall \lambda_1, \lambda_2, \dots, \lambda_n \in K$ tutti i vettori appartengono al sistema di generatori $S$ e se tutti gli scalari appartengono al nostro campo
- $\lambda_1v_1+\lambda_2v_2+\dots+\lambda_nv_n=0 \implies \lambda_1=\lambda_2=\dots=\lambda_n=0$ se la somma di tutti i vettori moltiplicati per lambda è uguale a 0 allora tutti i lambda sono uguali a 0. Importante ricordare che se c'è anche solo una situazione in cui anche solo un lambda è diverso da 0 ma la somma è uguale a 0 allora il sistema è detto **linearmente dipendente**

## Base di uno spazio vettoriale

Sia $V$ uno spazio vettoriale su $K$. $B\subseteq V$ è una base di $V$ se:
- $<B>=V$ è un insieme di generatori di $V$
- $V$ linearmente indipendente

> [!success] Corollario 1
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

### Teorema di Steinitz

> [!success] Teorema
> $V$ uno spazio vettoriale su $K$. $\{v_1, v_2, \dots, v_n\}$ un insieme di generatori di $V$.
> 
> Se $\{w_1, w_2, \dots, w_r\}$ è un insieme di generatori di $V$ con $r<n$ allora esiste un insieme di generatori $\{w_1, w_2, \dots, w_r, v_{r+1}, \dots, v_n\}$ di $V$ con $r+1\leq n$

> [!success] Corollario 2
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

## rappresentazioni (o forme) di sottospazi vettoriali

### Forma cartesiana e parametrica
Per rappresentare i sottospazi vettoriali ci sono due modi. 
Ognuno di questi ha i suoi pro e i suoi contro di cui ne parleremo dopo

#### Forma cartesiana
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

#### Forma parametrica
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

## Calcolare la base dello spazio vettoriale
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

#### cartesiana $\rightarrow$ parametrica
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

## Pro e contro di queste forme 
### Somma di sottospazi (forma cartesiana)
La forma migliore da usare per fare una somma di sottospazio è la forma cartesiana.

$V,W \subseteq K^n \longrightarrow V=row A,\ W=row B$
$A\in M_{m_1,n}(K),\qquad B\in M_{m_2,n}$

$$
C= \left(\frac{A}{B}\right) \in M_{m_1+m_2, n} \implies V \oplus W = row(C)
$$

##### Esercizio di esempio
$$
V = <\begin{pmatrix}
1\\1\\2
\end{pmatrix},\begin{pmatrix}
2\\2\\2
\end{pmatrix}>, \qquad W=<\begin{pmatrix}
0\\1\\0
\end{pmatrix}, \begin{pmatrix}
0\\0\\1
\end{pmatrix}> \subseteq ℝ^3
$$
$$
V= row\begin{pmatrix}
1 & 2& 1\\
2 & 2& 2
\end{pmatrix}, \qquad W=row\begin{pmatrix}
0 & 1 & 0\\
0 & 0 & 1
\end{pmatrix}
$$
$$
V\oplus B= row\begin{pmatrix}
1 & 2& 1\\
2 & 2& 2\\
0 & 1 & 0\\
0 & 0 & 1
\end{pmatrix} = \overbrace{<\begin{pmatrix}
1\\2\\1
\end{pmatrix},\begin{pmatrix}
2\\2\\2
\end{pmatrix},\begin{pmatrix}
0\\1\\0
\end{pmatrix},\begin{pmatrix}
0\\0\\1
\end{pmatrix}>}^4
$$
Il fatto che sia dimensione 4 significa che uno dei vettori non è necessario per creare la base. Per capire come rimuoverlo basta eseguire Gauss (non è necessario il passo Jordan) e verrà rimossa una riga che sarà la riga di troppo.

$$
\begin{pmatrix}
1 & 2& 1\\
2 & 2& 2\\
0 & 1& 0\\
0 & 0& 1
\end{pmatrix} \xrightarrow{r_2 \rightarrow \frac{r_2}{2}}\begin{pmatrix}
1 & 2& 1\\
1 & 1& 1\\
0 & 1& 0\\
0 & 0& 1
\end{pmatrix} \xrightarrow{r_2 \rightarrow r_2 - r_1}\begin{pmatrix}
1 & 2& 1\\
0 & -1& 0\\
0 & 1& 0\\
0 & 0& 1
\end{pmatrix} \xrightarrow{r_3 \rightarrow r_3 + r_2}
$$
$$
\begin{pmatrix}
1 & 2& 1\\
0 & -1& 0\\
0 & 0& 0\\
0 & 0& 1
\end{pmatrix} = \begin{pmatrix}
1 & 2& 1\\
0 & 1& 0\\
0 & 0& 1\\
0 & 0& 0
\end{pmatrix}
$$
Si prendono quindi solo le righe non nulle
$$
V= <\begin{pmatrix}
1\\2\\1
\end{pmatrix},\begin{pmatrix}
0\\1\\0
\end{pmatrix},\begin{pmatrix}
0\\0\\1
\end{pmatrix}>\implies \left\{\begin{pmatrix}
1\\2\\1
\end{pmatrix},\begin{pmatrix}
0\\1\\0
\end{pmatrix},\begin{pmatrix}
0\\0\\1
\end{pmatrix}\right\} \text{ base di }V
$$
$$
V= ℝ^3
$$

### Intersezione di sottospazio (forma parametrica)
Per calcolare la base di un'intersezione di sottospazi la forma migliore è la parametrica.

$$
V,W\subseteq K^n, V=\ker(A), w=\ker(B), C =(\frac{A}{B})
$$
$$
V\cap W = \ker(C)
$$

##### Esempio
$$
\begin{align*}
&V=<\begin{pmatrix}
1\\2\\1
\end{pmatrix}, \begin{pmatrix}
2\\2\\2
\end{pmatrix}>, W=<\begin{pmatrix}
0\\1\\0
\end{pmatrix}, \begin{pmatrix}
0\\0\\1
\end{pmatrix}>
\\
&V=row\begin{pmatrix}
1 & 2 & 1\\
2 & 2 & 2
\end{pmatrix} = row A \implies \ker A =\ker \begin{pmatrix}
1 & 2 & 1\\
2 & 2 & 2
\end{pmatrix}
\\
&\begin{pmatrix}
1 & 2&1\\
2&2&2
\end{pmatrix} \xrightarrow{r_2\rightarrow \frac{r_2}{2}} \begin{pmatrix}
1&2&1\\
1&1&1
\end{pmatrix}\xrightarrow{r_2\rightarrow -1\cdot(r_2-r_1)} \begin{pmatrix}
1&2&1\\
0&1&0
\end{pmatrix}
\\
&= \begin{pmatrix}
1&0&1\\
0&1&0
\end{pmatrix}
\end{align*}
$$

$$
\begin{align}
&W=row\begin{pmatrix}
0&1&0\\
0&0&1
\end{pmatrix} \implies \ker\begin{pmatrix}
0&1&0\\
0&0&1
\end{pmatrix}
\\
&\begin{cases}
x_2 = 0\\
x_3 = 0
\end{cases}\rightarrow \begin{pmatrix}
x_1\\
0\\
0
\end{pmatrix}=\begin{pmatrix}
1\\0\\0
\end{pmatrix}x_1\implies<\begin{pmatrix}
1\\0\\0
\end{pmatrix}> = row\begin{pmatrix}
1 & 0 & 0
\end{pmatrix}\implies
\\
&\implies W = ker\begin{pmatrix}
1&0&0
\end{pmatrix}= \{x_1=0
\end{align}
$$

$$
\begin{align*}
&V\cap W \begin{cases}
-x_1+x_3 = 0\\
x_1=0
\end{cases}= \ker\begin{pmatrix}
-1 & 0 & 1\\
1 & 0 & 0
\end{pmatrix}\xrightarrow{r_1 \rightarrow -1\cdot r_1}\\
&\ker\begin{pmatrix}
1 & 0 & -1\\
1 & 0 & 0
\end{pmatrix} \xrightarrow{r_2 \rightarrow r_2-r_1}\ker\begin{pmatrix}
1 & 0 &-1\\
0 & 0 & 1
\end{pmatrix}\xrightarrow{r_1\rightarrow r_1+r_2}\\
&\ker\begin{pmatrix}
1 & 0 &0\\
0 & 0 &1
\end{pmatrix} = \begin{cases}
x_1 = 0\\
x_3 = 0
\end{cases} = \begin{pmatrix}
0\\x_2\\0
\end{pmatrix}=\begin{pmatrix}
0\\1\\0
\end{pmatrix}x_2=<\begin{pmatrix}
0\\1\\0
\end{pmatrix}>
\end{align*}
$$

### [[Omomorfismo|Omomorfismi]] tra spazi vettoriali (o applicazioni lineari)
$B, W$ spazi vettoriali su $K$, avendo una funzione $f:V\longrightarrow W$ 

$f$ è un'applicazione lineare se:
- $\forall v_1,v_2 \in V\qquad f(v_1 + v_2)=f(v_1)+f(v_2)$
- $\forall v \in V, \forall \lambda \in K\quad f(\lambda \cdot v) = \lambda \cdot f(v)$

> [!example] Esempio 1
> $\begin{align}f: ℝ^2 &\longrightarrow ℝ^3\\ \begin{pmatrix}x\\y\end{pmatrix}&\longmapsto \begin{pmatrix}2x\\x+y\\2y\end{pmatrix}\end{align}$
> 
> In questo caso controlliamo se soddisfa il primo punto:
> $$
> \begin{align}
> &f(\begin{pmatrix}
> x_1\\ y_1
\end{pmatrix}+\begin{pmatrix}
> x_2\\ y_2
\end{pmatrix}) = \begin{pmatrix}
> 2(x_1+x_2)\\ x_1 + x_2 + y_1+y_2\\2(y_1+y_2)
\end{pmatrix}=\\
> =&\begin{pmatrix}
> 2x_1\\ x_1+y_1\\ 2y_1\end{pmatrix} + \begin{pmatrix}2x_2\\ x_2+y_2\\ 2y_2
\end{pmatrix}=f\begin{pmatrix}
> x_1\\ y_1
\end{pmatrix} +f\begin{pmatrix}
> x_2\\ y_2
\end{pmatrix}
\end{align}
> $$
> 
> Poi controlliamo se soddisfa la seconda proprietà
> $$
> \begin{align}
> &f\left(\lambda \begin{pmatrix}
> x\\ y
\end{pmatrix}\right) = f\begin{pmatrix}
> \lambda x\\ \lambda y
\end{pmatrix}=\begin{pmatrix}
> 2\lambda x\\ \lambda x+\lambda y\\ 2\lambda y
\end{pmatrix} = \lambda\begin{pmatrix}
> 2x \\ x+y \\ 2y
\end{pmatrix}=\\
> =&\lambda f\begin{pmatrix}
> x\\ y
\end{pmatrix}
\end{align}
> $$
> Essendo tutte e due questo è un [[Omomorfismo|omomorfismo]]

> [!example] Esempio 2:
> $$
> \begin{align}
> f:V&\longrightarrow W\\
> v&\longmapsto 0
> \end{align}\qquad \text{ si chiama [[Omomorfismo|omomorfismo]] nulllo}
> $$

> [!example] Esempio 3
> $$
> \begin{align}
> f:ℝ^3 &\longrightarrow ℝ^2\\
> \begin{pmatrix}
> x\\ y\\ z
\end{pmatrix} &\longmapsto \begin{pmatrix}
> x^2 +y \\ z
\end{pmatrix}
\end{align}
> $$
> In questo caso non è un [[Omomorfismo|omomorfismo]] in quanto un polinomio elevato a 2 da un valore particolare 

> [!example] Esempio 4
> $$
> \begin{align}
> f:ℝ^2 &\longrightarrow ℝ^2\\
> \begin{pmatrix}
> x\\ y
\end{pmatrix}& \longmapsto \begin{pmatrix}
> y- 1 \\ y + x
\end{pmatrix}
\end{align}
> $$
> Non è un [[Omomorfismo|omomorfismo]] in quanto non soddisfa la seconda proprietà:
> $$
> f\begin{pmatrix}
> 0 \\ 0
\end{pmatrix} = \begin{pmatrix}
> -1 \\ 0
\end{pmatrix}
> $$
> Ma
> $$
> \begin{align}
> f\begin{pmatrix}
> 0 \\ 0
\end{pmatrix}= f \left(0 \begin{pmatrix}
> 0 \\ 0
\end{pmatrix}\right)= 0 f\begin{pmatrix}
> 0 \\ 0
\end{pmatrix} =\begin{pmatrix}
> 0 \\ 0 
\end{pmatrix} \neq \begin{pmatrix}
> -1 \\ 0
\end{pmatrix}
\end{align}
> $$


In base le coordinate devono essere monomi di primo grado

> [!success] Lemma 
> $f: V\longrightarrow W$ è un monomorfismo, allora $f(0)=0$

### Applicazione lineare
$\ker (f) =\left\{v\in V\mid f(v) = 0\right\} \subseteq V$
Quindi il kernel di $f$ è l'insieme di tutte le $v\in V$ tali che $f(v) = 0$

$Im\ f= \left\{w\in W \mid \exists v \in V:f(v) = w\right\} \subseteq W$
Quindi l'immagine di $f$ è l'insieme di tutte le $w$ immagini di $f$

> [!success] Proposizione 1
> $$
> f:V\longrightarrow W \text{ [[Omomorfismo|omomorfismo}]]
> $$
> $\ker f$ è un sottospazio di $V$
> $Im\ f\subseteq W$ è un sottospazio di $W$

> [!success] Proposizione 2
> $$
> f: V\longrightarrow W \text{ [[Omomorfismo|omomorfismo}]]
> $$
> $V = <v_1,\ldots,v_m>$
> Allora
> $Im\ f=<f(v_1), \ldots, f(v_m)>$
> %%Inserire la dimostrazione scritta negli appunti%%

> [!success] Osservazione
> Se $\{v_1, \ldots, v_m\}$ base di $V \centernot{\implies}\{f(v_1), \ldots, f(v_m)\}$ base di $Im(f)$

Similmente al [[#^a5f396|teorema del rango]]:
$dim(\ker(f)) =: null(f)$
$dim(Im(f)) =: rk(f)$

> [!success] Teorema
> $null(f) + rk(f) = dim(v)$

$$
\begin{align}
&U,V,W\text{ tre spazi vettoriali su }K\\
& f:U \longrightarrow V, \qquad g: V\longrightarrow W\\
\end{align}
$$

$$
\begin{align}
g\circ f: U &\longrightarrow W\\
u& \longmapsto g(f(u))
\end{align}
$$


> [!success] Lemma
> Se $f,g$ sono applicazioni lineari allora $g\circ f$ è un'applicazione lineare

$V$ uno spazio vettoriale
$f:V\longrightarrow V$ è un applicazione lineare e un endomorfismo

Sia $V,W$ spazi vettoriali

$L(V,W)=\{V\longrightarrow W\text{ applicazioni lineari}\}$
Che è allo stesso momento uguale a
$Mor(V,W)$ e $Hom(V,W)$

$L(V,V)= End(V)$

### Aggiungere le operazioni

#### Addizione
$f,g \in L(V,W)$
$$
\begin{align}
f+g: V &\longrightarrow W\\
v &\longmapsto f(v)+g(v)
\end{align}
$$

#### Moltiplicazione
$f,g \in L(V,W), \lambda \in \lambda$

$$
\begin{aligned}
\lambda \cdot f: V&\longrightarrow W\\
v&\longmapsto \lambda\cdot f(v)=f(\lambda \cdot v)
\end{aligned}
$$

> [!success] Lemma
> $L(V,W)$ è uno spazio vettoriale su $K$
> > [!warning] Lo $0$ è una funzione
> > $$
> > \begin{align}
> > 0:V&\longrightarrow W\\
> > v &\longmapsto 0
\end{align}
> > $$

### Proprietà degli [[Omomorfismo|omomorfismi]]

$f: V\longrightarrow W$ combinazione lineare allora:
1. $f$ è [[Iniettività|iniettiva]] $\iff\forall v_1\neq v_2\in V, f(v_1)\neq f(v_2)$
2. $f$ è [[Suriettività|suriettiva]] $\iff \forall v\in V, \exists f(v)=w$
3. $f$ è [[Biiettività|biiettiva]] $\iff f$ [[Iniettività|iniettiva]] e [[Suriettività|suriettiva]] $\iff$ invertibile

> [!success] lemma
> Se $f:V\longrightarrow W$ invertibile. Allora la sua inversa è un'applicazione lineare.
> $V,W$ apazi vettoriali. Isomorfi ($V\simeq W$) se $\exists f:V\longrightarrow W$ che è un [[Isomorfismo]] 

> [!success] Proposizione
> $f: V\longrightarrow W$ applicazione lineare
> $f$ è [[Iniettività|iniettiva]] $\iff\ker(f)=\{0\}$

> [!success] Proposizione
> $f: V\longrightarrow W$ [[Omomorfismo|omomorfismo,]] $B = \{B_i\}_{i=1,\ldots,n}$ base di $B$
> 1. $f$ è determinata da $f(b_1), \ldots, f(b_n)$
> 2. Dati $m$ vettori in $W$ allora $\exists!g:V\longrightarrow W\text{ t. c } g(b_i) = w_i \{w_1, \ldots, w_m\}$

> [!success] Corollario 3
> $f:V\longrightarrow W$ [[Omomorfismo|omomorfismo]]
> $B = \{B_i\}_{i=1,\ldots,n}$ base di $V$
> 1. $f$ [[Iniettività|iniettiva]] $\iff\{f(b_1),\ldots f(b_m)\}$ sono linearmente indipendenti
> 2. $f$ [[Suriettività|suriettiva]] $\iff\{f(b_1),\ldots f(b_m)\}$ sono generatori di $W$
> 3. $f$ [[Biiettività|biiettiva]] $\iff\{f(b_1),\ldots f(b_m)\}$ sono una base di $W$

^7444b5

> [!warning] attenzione
> Ci sono un sacco di dimostrazioni che non ho scritto in questi appunti. Riguardarsele

# Lezione del 15-11-2024

## Iniettività suriettività e biiettività delle funzioni

> [!success] Corollario 4
> $V,W$ spazi vettoriali su $K, dim\ V=n,dim\ W=m, f:V\to W$ omomorfismo
> 1. $f$ iniettiva $\iff n\leq m$
> 2. $f$ suriettiva $\iff n \geq m$
> 3. $f$ biiettiva $\iff n = m$

> [!success] Teorema (*dell'isomorfismo*)
> $V$ spazio vettoriale  su $K$, $dim\ V=n$, allora $V\simeq K^n$
> > [!summary] Dimostrazione
> > Avendo $B = \{b_1,\ldots, b_n\}$ base di $V$
> > $$
> > \begin{align}
> > \varphi: V &\to K^n\\
> > b_1 &\mapsto \varphi(b_1) = e_1 = (1\ 0\ \dots\ 0)
> > \end{align}
> > $$
> > Allora $\{\varphi(b_1), \dotsb, \varphi(b_n)\}= \varepsilon$ che seguendo il [[#^7444b5|corollario 3]] è [[Biiettività|biiettiva]] 

Da qui già si può capire che la cosa più importante è stabilire una base. Infatti:

$V$ spazio vettoriale di $dim\ V=n, B=\{b_1,\dots, b_n\}$ base di $V$

Ma cosa significa che $B$ è una base?

Vuol dire che $v\in V\implies \exists!\lambda_1,\dots,\lambda_n\in K \text( t. c. ) v=\lambda_1b_1 + \dots + \lambda_nb_n \implies$
$\implies v\in V\rightsquigarrow \begin{pmatrix} \lambda_1\\ \lambda_2\\ \vdots\\ \lambda_n \end{pmatrix} \in K^n$

Quindi $\varphi(v) = \varphi(\lambda_1v_1+\dots+\lambda_nv_n)=\lambda_1\varphi(v_1)+\dots+\lambda_n\varphi(v_n)=$
$\lambda_1e_1+\dots+\lambda_ne_n=\lambda_1\begin{pmatrix} 1\\ 0\\ \vdots\\ 0 \end{pmatrix} +\dots+\lambda_n \begin{pmatrix} 0\\ 0\\ \vdots\\ 1 \end{pmatrix}= \begin{pmatrix} \lambda_1\\ \lambda_2 \\ \vdots \\ \lambda_n \end{pmatrix}$
### Con i polinomi
#### Esempio
$K[X]_{\leq 2}=\{a+bx+cx^2\mid a,b,c \in ℝ\}$
In questo caso la dimensione è $dim\ (K[x]_{\leq 2})= 3$ in quanto la base standard $B=\{1, x, x^2\}$

$$
\begin{align}
	\varphi: K[X]_{\leq 2} &\to K^3\\
	1&\mapsto \begin{pmatrix}
	1\\0\\0
	\end{pmatrix}\\
	x& \mapsto \begin{pmatrix}
	0\\1\\0
	\end{pmatrix}\\
	x^2&\mapsto \begin{pmatrix}
	0\\0\\1
	\end{pmatrix}
\end{align}
$$
Ottenendo quindi qualcosa come $a+bx+cx^2 = \begin{pmatrix} a\\b\\c \end{pmatrix}$

Ma questo se si sceglie la "*base standard*". È possibile anche cambiare base ed è come se si stesse cambiando **sistema di rappresentazione del vettore**:
Usando la base $C = \{1+x, x+x^2, 1+x^2\}$
$$
\begin{align}
	\tau:K[X]_{\leq 2}&\to K^3\\
	1 + x &\mapsto \begin{pmatrix}
	1\\0\\0
	\end{pmatrix}\\
	x + x^2 & \mapsto \begin{pmatrix}
	0\\1\\0
	\end{pmatrix}\\
	1 + x^2 &\mapsto \begin{pmatrix}
	0\\0\\1
	\end{pmatrix}
\end{align}
$$

## La base standard
$K^3=\left\{\begin{pmatrix} a\\b\\c \end{pmatrix}\mid a,b,c\in K\right\}$

$v=\begin{pmatrix} 1\\2\\1 \end{pmatrix} = 1\cdot\begin{pmatrix} 1\\0\\0 \end{pmatrix}+2\begin{pmatrix} 0\\1\\0 \end{pmatrix}+1\begin{pmatrix} 0\\0\\1 \end{pmatrix}$

Tutto questo però si può fare seguendo anche un'altra base ad esempio
$B =\{(1,1,0),(0,1,1),(1,0,1)\}$ base di $K^3$

$v=\begin{pmatrix} 1\\2\\1 \end{pmatrix} =$ *$1$* $\cdot\begin{pmatrix} 1\\1\\0 \end{pmatrix}+$*$1$* $\begin{pmatrix} 0\\1\\1 \end{pmatrix}+$ *$0$*$\begin{pmatrix} 1\\0\\1 \end{pmatrix}=[V]_B=\begin{pmatrix} 1\\1\\0 \end{pmatrix}$
Di cui il vettore finale sono i vettori evidenziati.

$[V]_B$ coordinate di $V$ rispetto a $B$

---
$V,W$ spazi vettoriali. $dim\ V=n,dim\ W=m, B_V=\{v_1,\dots, v_n\}\text{ base di }V,\ B_W=\{w_1,\dots, w_m\}\text{ base di }B$
$$
f:V\to W\text{ omomorfismo},\quad \{f(v_1),\dots, f(v_n)\}\subset W
$$
$$
f(v_j)=a_{1\ j}\cdot w_1 +\dots + a_{m\ j}\cdot w_m\forall j=1,\dots,n
$$
$v\in V$ si scrive $f(v)$ 
Di cui $V=\lambda_1v_1+\dots + \lambda_nv_n\implies f(v)=f(\lambda_1v_1 +\dots + \lambda_nv_n)= \lambda_1 f(v_1)+\dots+\lambda_nf(v_n)=$$=\lambda_1(a_{11}w_1+\dots+a_{m1}w_m)+\dots+\lambda_n(a_{1n}w_1+\dots+a_{mn}w_m)$
$=(\lambda_1a_{11}+\dots+\lambda_na_{1n})w_1+\dots+(\lambda_1a_{m1}+\dots+\lambda_na_{mn})w_m$
Di cui:
$w_1 = \begin{pmatrix} 1\\0\\\vdots\\0 \end{pmatrix}, w_m+\begin{pmatrix} 0\\0\\\vdots\\1 \end{pmatrix}$

Otteniamo quindi che:
- $W\simeq K^n$
- $B_W$
- $V\simeq K^n$
- $B_V$
$$
=\begin{pmatrix}
	\lambda_1a_{11}&+&\dots&+&\lambda_na_{1n}\\
	\vdots &&\ddots&& \vdots\\
	\lambda_1a_{m1}&+&\dots&+&\lambda_na_{mn}\\
\end{pmatrix}=[f(v)]_{B_{_W}}
$$
$$
A=(a_{ij})_{\underset{1\leq j\leq n}{1\leq i\leq m}}\in M_{m,n}(K)
$$
$$
[V]_{B_{_V}}=\begin{pmatrix}
	\lambda_1\\
	\vdots\\
	\lambda_n
\end{pmatrix}
$$

## Matrice rappresentate un'applicazione lineare
Abbiamo quindi ottenuto $[f(V)]_{B_{W}}=A\cdot [V]_{B_{V}}$
Sapendo che $A=[M]^{^{B_{V}}}_{_{B_W}}$
Otteniamo la relazione: $[f(V)]_{B_{W}}=[M]^{^{B_{V}}}_{_{B_W}}\cdot [V]_{B_{V}}$
Di cui $[M]^{^{B_{V}}}_{_{B_W}}$ è la matrice che rappresenta l'applicazione lineare ed è creata mettendo tutti i vettori della base $B_W$ in verticale:
$$
[M]^{^{B_{V}}}_{_{B_W}}=\begin{pmatrix}
	f(v_1)_{B_W}&\dotsb&f(v_n)_{B_W}
\end{pmatrix}
$$

### Esempio trovare la matrice rappresentante
$$
\begin{align}
	g:ℝ^2&\to ℝ^3\\
	\begin{pmatrix}
	x\\y
	\end{pmatrix}&\mapsto \begin{pmatrix}
	2x\\ x+y\\ 2y
	\end{pmatrix}
\end{align}
$$
Poi si devono definire le due basi di $ℝ^3$ e $ℝ^2$:
$$
\begin{align}
	&\varepsilon_2=\left\{\begin{pmatrix}
	1\\0
	\end{pmatrix},\begin{pmatrix}
		0\\1
	\end{pmatrix}\right\}\\
	&\varepsilon_3=\left\{\begin{pmatrix}
	1\\0\\0
	\end{pmatrix},\begin{pmatrix}
	0\\1\\0
	\end{pmatrix},\begin{pmatrix}
	0\\0\\1
	\end{pmatrix}\right\}
\end{align}
$$
Poi si calcola utilizzando le due basi a cosa risulta $f(v)$
$$
g\begin{pmatrix}
	1\\0
\end{pmatrix}=\begin{pmatrix}
	2\\1\\0
\end{pmatrix},g\begin{pmatrix}
	0\\1
\end{pmatrix}=\begin{pmatrix}
	0\\1\\2
\end{pmatrix}
$$

Prendiamo quindi i due vettori e mettiamoli in colonna:
$$
[M]^{\varepsilon_2}_{\varepsilon_3}=\begin{pmatrix}
	2 & 0\\
	1 & 1\\
	0 & 2
\end{pmatrix}\in M_{3,2}(ℝ)
$$

### Esempio da matrice ad applicazione lineare
Avendo quindi la matrice:
$$
\begin{pmatrix}
	2 & 1& 0 &4 \\
	2&3&2&6
\end{pmatrix}
$$
Essendoci $4$ colonne sappiamo che ci sono $4$ variabili e sappiamo che:
$$
\begin{pmatrix}
	x\\ y\\ z\\ w
\end{pmatrix}=xe_1+ye_2+ze_3+we_4
$$

Si scrive quindi così:
$$
\begin{align}
	f:ℝ^4&\to ℝ^2\\
	e_1&\mapsto\begin{pmatrix}
		2\\2
	\end{pmatrix}\\
	e_2&\mapsto\begin{pmatrix}
		1\\3
	\end{pmatrix}\\
	e_3&\mapsto\begin{pmatrix}
		0\\2
	\end{pmatrix}\\
	e_4&\mapsto\begin{pmatrix}
		4\\6
	\end{pmatrix}
\end{align}
$$

> [!success] Teorema
> $V,W$ spazi vettoriali su $K$. $dim\ V=n,dim\ W=m$
> $Hom(V,W)\simeq M_{m,n}(K)$
> L'isomorfismo dipende dalla scelta delle basi di $V$ e $W$

$Hom(V,V)$ quindi un $End(V)\simeq M_{n,n}(K)$
$\varepsilon$ basi di $V$ nel dominio e codominio 

Sappiamo che
$id\ n\in M_{n,n}(K) \longleftrightarrow id\ v\in End(V)$

E che lo zero è:
$0\in M_{n,n}(K) \longleftrightarrow 0 \in End(V)$

> [!success] Proposizione
> $V,W,U$ spazi vettoriali di dimensioni $n,m,p$ rispettivamente
> *fissiamo le basi (**importante**)*, $f:V\to W\quad g:W\to U$ applicazioni lineari
> $M(g\circ f)=M(g)\cdot M(f)$
> Di cui:
> - $M(g\circ f) \in M_{p,n}$
> - $M(g) \in M_{p,m}$
> - $M(f)\in M_{m,n}$

> [!success] Corollario
> $f:V\to V$ endomorfismo biiettivo
> *fissiamo le base di $V$*
> $M(f^{-1})=M(f)^{-1}$

## Kernel e immagine di $f$
$f:V\to W\rightsquigarrow \ker f \subseteq V,Im\ f\subseteq W$

> [!success] Proposizione
> $f:V\to W$ omomorfismo
> fissiamo le basi sia di $V$ che di $W$ e sia $M$ la matrice rappresentante $f$
> Otteniamo che:
> - $\ker f \simeq \ker M$
> - $\text{Im}\ f \simeq \text{col } M=\text{ spazio generato dalle colonne di }M$

### Esempio
$$
\begin{align}
	f:ℝ^3 &\to ℝ^2\\
	\begin{pmatrix}
	x\\ y\\ z
	\end{pmatrix}&\mapsto \begin{pmatrix}
	x + y \\ y + z
	\end{pmatrix}
\end{align}
$$

$$
f\begin{pmatrix}
	1\\0\\0
\end{pmatrix}=\begin{pmatrix}
	1\\0\\
\end{pmatrix}, f\begin{pmatrix}
	0\\1\\0
\end{pmatrix}=\begin{pmatrix}
	1\\1
\end{pmatrix},f\begin{pmatrix}
	0\\0\\1
\end{pmatrix}=\begin{pmatrix}
	0\\1
\end{pmatrix}
$$ Per trovare il kernel di:
$$
\left\{\begin{pmatrix}
	1\\0
\end{pmatrix},\begin{pmatrix}
	1\\1
\end{pmatrix},\begin{pmatrix}
	0\\1
\end{pmatrix}\right\}
$$
Di cui la matrice rappresentate è:
$$
M(f)=\begin{pmatrix}
	1&1&0\\
	0&1&1\\
\end{pmatrix}
$$
Sapendo che $\ker f \simeq \ker M$ dobbiamo trovare il kernel. Quindi si fa la forma di Echelon ridotta:
$$
\begin{pmatrix}
	1&0&-1\\
	0&1&1
\end{pmatrix} \begin{cases}
	x = z\\
	y = -z
\end{cases} \implies \begin{pmatrix}
	x\\
	y\\
	z
\end{pmatrix}=\begin{pmatrix}
	z\\
	-z\\
	z
\end{pmatrix}=
$$
$$
=z\begin{pmatrix}
	1\\
	-1\\
	1
\end{pmatrix}= <\begin{pmatrix}
	1\\-1\\1
\end{pmatrix}>
$$

Ottenendo quindi il kernel

Ora dobbiamo trovare l'immagine 
$$
Im(f) \simeq <\begin{pmatrix}
	1\\0
\end{pmatrix},\begin{pmatrix}
	1\\1
\end{pmatrix},\begin{pmatrix}
	0\\1
\end{pmatrix}>= \underbrace{<\begin{pmatrix}
	1\\0
\end{pmatrix}
\begin{pmatrix} 0\\1 \end{pmatrix}>}_{\text{base di } ℝ} = ℝ^2
$$

Otteniamo quindi che $f$ è suriettiva ma non iniettiva.

> [!success] Corollario
> Se $f$ è un omomorfismo e $M$ la matrice che lo rappresenta
> $\text{null}(f)=\text{null}(M), \text{rk}(f)=\text{rk}(M)$
> 
> E che $\text{null}(f)=\text{dim}(\ker f)$

Ricordare anche che $f\text{ iniettiva }\iff \ker M = \left\{\begin{pmatrix} 0\\0\\\vdots\\0 \end{pmatrix}\right\}$
