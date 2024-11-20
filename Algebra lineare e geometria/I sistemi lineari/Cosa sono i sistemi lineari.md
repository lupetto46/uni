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