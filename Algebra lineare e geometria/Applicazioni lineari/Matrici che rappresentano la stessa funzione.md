Quando fissiamo una base stiamo facendo una scelta. Ovviamente proprio per questo motivo dipendentemente dalla base che scegliamo tutto cambia infatti quando scriviamo la forma di matrice di una funzione dobbiamo *specificare anche con che base sta venendo rappresentata*

Ma essendo che due matrici con due basi diverse stanno rappresentando la stessa funzione ci dovrà essere qualcosa che le **mettono in relazione**
### Cambio di base tra matrici
Abbiamo visto che $[f(v)]_{B_W}=[M(f)]^{B_V}_{B_W}\cdot [V]_{B_V}$ in [[#Forma matriciale di una funzione]]
E otteniamo anche che $[f(v)]_{B'_W}=[M(f)]^{B'_V}_{B'_W}\cdot [V]_{B'_V}$

Ma adesso consideriamo di avere una $b_j \in V$ con $j=1,\dots, n$
Se $\{v_1,\dots, v_n\}$ è una base di $V$ allora 
$\exists b_{1j},\dots,b_{nj}\in K$ tali che $b_j=b_{1j}v_1+\dots+b_{nj}v_n$
Questo si scrive quindi come $[b_j]_{B_V}=\begin{pmatrix} b_{1j}\\ \vdots\\ b_{nj} \end{pmatrix}$
Questo ci permette di creare la matrice $B=(b_{ij})\in M_{n,n}(K)$
$$
B=\begin{pmatrix}
	[b_1]_{B_V} & \dots & [b_n]_{B_V}
\end{pmatrix}
$$

Di cui $b_1,\dots, b_n$ sono i vettori di una base rappresentati attraverso un'altra base.
È quindi necessario per trovarli calcolare l'immagine del vettore della base.
### Rappresentazione di $V$ rispetto a $B'_V$
Avendo dei vettori $v\in V$ possiamo dopo aver segnato la base dire che questo vettore è: 
$v=\lambda_1 b_1+\dots + \lambda_nb_n$ e si scrive quindi $[v]_{B'_V}=\begin{pmatrix} \lambda_1\\ \vdots\\ \lambda_n \end{pmatrix}$ 
$\implies \lambda_1(b_{11}v_1 +\dots+b_{n1}v_n)+\lambda_2(b_{12}v_1+\dots+b_{n2}v_n+\dots+\lambda_n(b_{1n}v_1+\dots+b_{nn}v_n$
Cambiando l'ordine di come viene raggruppato il tutto si può ottenere quindi
$(\lambda_1b_{11}+\dots+\lambda_nb_{1n})v_1+\dots+(\lambda_1b_{n1}+\dots+\lambda_nb_{nn})v_n$
Otteniamo quindi che le coordinate di $v$ rispetto a $B_V$ sono:
$$
[v]_{B'_V}=\begin{pmatrix}
	\lambda_1b_{11}&+&\dots&+&\lambda_nb_{1n}\\
	\vdots&&\ddots&&\vdots\\
	\lambda_1b_{n1}&+&\dots&+&\lambda_nb_{nn}
\end{pmatrix}
$$
Ma se notiamo ogni singola riga è composta da un elemento del vettore moltiplicato per gli stessi lambda. Ottenendo che:
$$
[v]_{B'_V}=B\cdot\begin{pmatrix}
	\lambda_1\\
	\vdots\\
	\lambda_n
\end{pmatrix}
$$
Chiamandola la rappresentazione di $V$ rispetto a $B'_{V}$.

> [!tip] Analogamente
> Mentre $[w]_{B_W}=C\cdot [W]_{B'_W}, C=\begin{pmatrix} [c_1]_{B_W}&\dots&[c_m]_{B_W} \end{pmatrix}\in M_{m,m}(K)$
> Allora $[w]_{B'_W}=C^{-1}\cdot [w]_{B_W}$

Otteniamo quindi la formula 
$$
[M(f)]^{B'_V}_{B'_W}=C^{-1}\cdot[M(f)]^{B_V}_{B_W}\cdot B
$$
