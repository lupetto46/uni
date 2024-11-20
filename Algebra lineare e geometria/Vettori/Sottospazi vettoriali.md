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