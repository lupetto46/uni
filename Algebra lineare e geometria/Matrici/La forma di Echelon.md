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