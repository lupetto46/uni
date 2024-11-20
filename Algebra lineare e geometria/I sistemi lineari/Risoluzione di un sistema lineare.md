### Gauss-Jordan
Per trovare le soluzioni del sistema si devono affiancare la matrice $A$ con la matrice $B$ e applicare il metodo di Gauss-Jordan.

%% TODO: Aggiungere gli esempi del professore %%

### Teorema di Rouché-Capelli

Il teorema di Rouché-Capelli dice:

#### Teorema 
Un sistema lineare in forma matriciale $AX=B$ ammette soluzioni se e solo se $rk(A)=rk(A|B)$

Se il sistema ammette soluzioni con una matrice $A\in M_{m,n}(K)$ allora le soluzioni sono in numero infinito e dipendono da $n-rk(A)$ parametri.

Inoltre un sistema lineare se ammette soluzione ne ammette:
- Una sola
- Nessuna
- Infinite

### Teorema di Cramer
Gauss-Jordan, anche se riesce a dare le soluzioni, non da una formula chiusa che ci permette di dire esattamente quali sono le soluzioni
Per questo si utilizza il teorema di Cramer.
> [!success] Teorema
> Sia $AX=B$ sistema lineare, $A\in M_{n,n}(\mathbb{R})$
> Se $A$ è invertibile (quindi $rk(A)=n$) allora la soluzione ($x=\begin{pmatrix} x_1\\ \vdots\\ x_n \end{pmatrix}$) sono date dalla formula:
> $$
> x_i=\frac{|A_i|}{|A|}
> $$
> 
> Di cui $A_i$ è la matrice ottenuta sostituendo ad $A$ la colonna $i$-esima con la matrice $B=\begin{pmatrix} b_1\\ \vdots\\ b_n \end{pmatrix}$