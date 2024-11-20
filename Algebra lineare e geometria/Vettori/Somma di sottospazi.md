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