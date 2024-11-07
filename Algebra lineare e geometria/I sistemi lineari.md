## Cosa sono i sistemi lineari
I sistemi lineari sono un insieme di equazioni di primo grado a più variabili, e le matrici sono utilizzate per poter svolgere tutte queste equazioni contemporaneamente.

$$
\begin{cases}
	a_{11}x_1 + a_{12}x_2 + \dots + a_{1n}x_n = b_1\\
	a_{21}x_1 + a_{22}x_2 + \dots + a_{2n}x_n = b_2\\
	\vdots\\
	a_{m1}x_1 + a_{m2}x_2 + \dots + a_{mn}x_n = b_m\\
\end{cases}
$$

In questo caso la matrice $A$ che contiene i coefficienti delle incognite sarà:
$$
    \begin{pmatrix}
        a_{11} & a_{12} & \dots & a_{1n}\\
        a_{21} & a_{22} & \dots & a_{2n}\\
        \vdots & \vdots & \ddots & \vdots\\
        a_{m1} & a_{m2} & \dots & a_{mn}\\
    \end{pmatrix}
$$

La matrice $X$ che contiene le incognite sarà:
$$
    X=\begin{pmatrix}
      x_1\\
      x_2\\
      \vdots\\
      x_n  
    \end{pmatrix} \in M_{n,1}(K)
$$

E la matrice $B$ che contiene i termini noti sarà:
$$
    B=\begin{pmatrix}
        b_1\\
        b_2\\
        \vdots\\
        b_m\\
    \end{pmatrix} \in M_{m,1}(K)
$$
Chiamiamo **matrice completa** del sistema invece la matrice:
$$
(A|B)
$$

Si scrive avendo tutte queste matrici la **forma matriciale del sistema lineare**:
$$
    AX=B
$$

## Risoluzione di un sistema lineare
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

## Sistemi lineare con coefficienti variabili
Nel caso in cui i coefficiente delle equazioni siano variabili quindi $\alpha \in K$ bisogna svolgerlo normalmente eseguendo [[Matrici#Algoritmo di Gauss-Jordan|l'algoritmo di Gauss-Jordan]] a meno che il valore di $\alpha$ non si trovi come pivot. In quel caso è necessario, prima di dividere $\alpha$ per se stesso in modo da ottenere il pivot uguale a uno, analizzarlo per poter specificare che valori non può prendere $\alpha$ in modo tale da non risultare $\frac{0}{0}$ ponendo quindi $\alpha \neq 0$

## Sistema lineare omogeneo
Un sistema lineare omogeneo è un sistema lineare in cui tutti i termini noti sono uguali a zero.
$$
    \begin{cases}
        a_{11}x_1 + a_{12}x_2 + \dots + a_{1n}x_n = 0\\
        a_{21}x_1 + a_{22}x_2 + \dots + a_{2n}x_n = 0\\
        \vdots\\
        a_{m1}x_1 + a_{m2}x_2 + \dots + a_{mn}x_n = 0\\
    \end{cases} \iff AX=0
$$

in questo caso $A|B$ ammette sempre almeno una soluzione che è la soluzione con tutti zero ovvero $\begin{pmatrix} 0\\ \vdots\\ 0 \end{pmatrix}\in M_{n,1}$


> [!todo] Osservazione
> Avendo $Y,Y'$ soluzioni di $AX=0\iff AY'=0=AY$
>
> Considerando che $A(Y+Y')=AY+AY'=0+0=0$ e $A(-Y)=-(AY)=0$ per tutte le soluzioni $\Sigma_0\{\text{soluzioni di }AX=0\}$ allora $(AX, +, 0)$ è un \textbf{gruppo abeliano}
> 
> Anche se questo funziona solo per i sistemi omogenei.

## Associare un sistema lineare a un sistema lineare omogeneo

Dato un sistema lineare $AX=B$ si può associare un sistema lineare omogeneo $AX=0$.

> [!success] Proposizione
> Se $Z$ è una soluzione di $AX=B$ e $H$ è una soluzione di $AX=0$ allora l'insieme delle soluzioni di $AX=B\quad \Sigma=\{Z+H|H\in \Sigma_0\}$ ricordando che $\Sigma_0$ è l'insieme delle soluzioni di $AX=0$
> Quindi basta una soluzione di $AX=B$ e tutte le soluzioni di $AX=0$ per avere tutte le soluzioni di $AX=B$
> > [!summary] Dimostrazione
> > Avendo 
> >
> > $\Sigma = \{\text{soluzioni di } AX=B\}$ e $\Sigma_0=\{\text{soluzioni di } AX=0\}$ 
> > 
> > Dimostrare che $\Sigma_0 \subseteq \Sigma$ e $\Sigma_0 \supseteq \Sigma$

