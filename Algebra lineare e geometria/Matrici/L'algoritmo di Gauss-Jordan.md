L'algoritmo di Gauss-Jordan è un algoritmo che permette di trasformare una matrice qualsiasi in forma di Echelon ridotta.

Questo algoritmo permette di utilizzare le operazioni elementari per trasformare una matrice in forma di Echelon ridotta. Queste operazioni elementari sono:

- Scambiare le righe
- Moltiplicare una riga per uno scalare non nullo
- Sostituire una riga con la somma tra se stessa e un'altra riga moltiplicata per uno scalare. $r_i+\alpha r_j, \alpha \in K, j\neq i$

Questo è diviso in 2 parti: La parte di Gauss e la parte di Jordan
### Gauss
- Trovare il primo elemento non nullo della prima colonna
- Scambiare la riga con il primo elemento non nullo con la prima riga della matrice
- Dividere tutta la prima riga per il valore del suo primo valore
- Controllare tutte le altre entrate della prima colonna e se si trova un elemento non nullo sottrarre quella riga con la prima riga moltiplicata per l'elemento non nullo
- Ottenere una matrice in questa forma:
$$
\begin{pmatrix}
	(1) & a_{12} & \dots & a_{1n}\\
	0 & b_{22} & \dots & b_{2n}\\
	\vdots &\vdots & \ddots & \vdots\\
	0 & b_{n2} & \dots & b_{nn}            
\end{pmatrix}
$$
- Prendere solo la matrice $B$:
$$
B=\begin{pmatrix}
	b_{22} & \dots & b_{2n}\\
	\vdots & \ddots & \vdots\\
	b_{n2} & \dots & b_{nn}                
\end{pmatrix}
$$
- Ripetere il procedimento con la matrice $B$
### Jordan
Una volta finito otteniamo un matrice in forma di Echelon.
Per trasformarla in forma di Echelon ridotta è necessario utilizzare l'algoritmo di Jordan sulla matrice.
- Prendere l'ultimo pivot che abbiamo trovato
- Prendere tutti i valori non nulli sopra il pivot e sottrarre le rispettive righe per la riga del pivot moltiplicata per l'elemento non nullo
- Eseguire la stessa cosa per ogni pivot dal basso verso l'alto

Finiti tutte queste operazioni otteniamo la matrice in forma di Echelon ridotta.