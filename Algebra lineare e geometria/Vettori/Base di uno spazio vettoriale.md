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