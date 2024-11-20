---
Data: 24-11-2024
---


# Giorno 3
## Il valore assoluto
Il valore assoluto può essere utilizzato come operatore operazionale o operatore funzionale
Noi lo utilizzeremo come operatore funzionale

$|f(x)|$ ha due situazioni:
1. Se $f(x) \geq 0$ allora $|f(x)|=f(x)$
2. Se $f(x)\leq0$ allora $|f(x)| = -f(x)$

Prendiamo come esempio la funzione:
$f(x)=|\frac{x+2}{x-1}| +|x^2+4x=3|+1$
Innanzitutto vediamo dove il valore assoluto mostra il suo effetto studiando il segno:
$$
\begin{flalign}
&\frac{x+2}{x-1}\geq 0\\
&x+2\qquad x+2 \geq 0 \qquad &x\geq -2\\
&x-1 \qquad x-1>0 \qquad &x>1
\end{flalign}
$$

Ottenendo quindi:
![[Pasted image 20240924230413.png]]
Concludendo quindi che:
$$
\begin{flalign}
&\frac{x+2}{x-1}\geq 0\qquad \forall x\in ℝ:x\leq-2\ \cup\ x>1\\
&\frac{x+2}{x-1} < 0\qquad \forall x \in ℝ:-2\leq x<1
\end{flalign}
$$

Poi prendiamo l'altro polinomio messo sotto valore assoluto:
$x^2+4x+3$
> [!per sapere]
> Il professore qui ha fatto utilizzare una cosa chiamata "delta 4 ($\frac{\Delta}{4}$)” che si può utilizzare **solo** se il coefficiente della $x$ di primo grado è pari e serve nel caso in cui i numeri da calcolare nel delta sono troppo alti

$$
\begin{align}
&x^2+4x+3\geq 0\\
&\frac{\Delta}{4}=(\frac{b}{2})^2-ac=4-3 = 1\\
&x_{1,2} = \frac{-\frac{b}{2}\pm\sqrt{\frac{\Delta}{4}}}{a}=-2\pm1\\
&x_1 = -2-1=-3\\
&x_2 = -2 + 1 = -1
\end{align}
$$

Ottenendo quindi:
$x^2+4x+3\geq0\qquad \forall x\in ℝ:x\leq-3\ \cup\ x> -1$
$x^2+4x+3<0\qquad\forall x \in ℝ:-3<x< -1$

Otteniamo quindi unendo tutti e due i polinomi sotto valore assoluto:
![[Pasted image 20240924232052.png]]
si ottiene quindi in tutto $f(x)$ le cui condizioni di esistenza $\forall x\in ℝ:x\neq1$
$$
f(x)=\cases{
\begin{align}
\frac{x+2}{x-1} &+ (x^2+4x+3) +1\ se\ x\leq-3\ \cup\ x>1\\
\frac{x+2}{x-1} &- (x^2+4x+3) +1\ se\ -3<x\leq-2\\
-(\frac{x+2}{x-1}) &- (x^2+4x+3) +1\ se\ -2<x\leq -1\\
-(\frac{x+2}{x-1}) &+ (x^2+4x+3) +1\ se\ -1<x<1
\end{align}
}
$$

## Equazioni in valore assoluto
$|-f(x)|=k$ con $k\in ℝ$
- Impossibile se $k<0$
- Risolvibile se $k\geq 0$

$|f(x)|= k$ con $k\geq 0 \rightarrow \begin{cases}\begin{align}f(x)=k\ &se\ f(x)\geq 0\\ -f(x)=k\ &se\ f(x)<0\end{align}\end{cases}$

## Disequazioni irrazionali
Le radici hanno
$\sqrt[n]{radicando}$

Il cui risultato è: *quel numero che elevato a $n$ restituisce il $radicando$*
Per adesso però considereremo solo radici la cui $n=2$

Prendiamo quindi il caso in cui 
$\sqrt{f(x)}\geq g(x)$
Ma quello che stiamo scrivendo deve avere senso e per avere senso è necessario porre $f(x)\geq 0$ in quanto una radice quadrata non ha risultati nei numeri reali se il radicando è negativo
$$
\begin{cases}
f(x)\geq 0\\
g(x)\leq 0
\end{cases}\ \cup\ \begin{cases}
f(x)\geq 0\\
g(x)\geq 0\\
f(x)\geq [g(x)]^2
\end{cases}
$$
Se $g(x)\leq 0$ allora il sistema è sempre verificato in quanto $f(x)$ che è **sempre positivo** sarà sempre maggiore o uguale a $g(x)$ che è **sempre negativo**

Cambia invece nel caso in cui $g(x)\geq0$ qui entra il fatto che *elevare al quadrato due polinomi sempre positivi non cambia il risultato* permettendoci di **rimuovere la radice**

Ma se $f(x) \geq [g(x)]^2$ e $[g(x)]^2\geq0$ allora $f(x)\geq[g(x)]^2$ questo implica che $f(x)\geq 0$ e quindi non è necessario scriverlo nel sistema rimanendo con:
$$
\begin{cases}
f(x)\geq 0\\
g(x)\leq 0
\end{cases}\ 
\cup\ 
\begin{cases}
g(x)\geq 0\\
f(x)\geq [g(x)]^2
\end{cases}
$$

Nel caso in cui invece:
$\sqrt{f(x)}\leq g(x)$
otteniamo che:
$f(x)\geq 0$ deve essere maggiore o uguale a zero per dare senso alla radice
$g(x)\geq0$ deve essere maggiore di zero per permettere poi di fare
$f(x)\leq[g(x)]^2$
ottenendo quindi
$$
\begin{cases}
\begin{align}
f(x)&\geq0\\
g(x)&\geq 0\\
f(x)&\leq [g(x)]^2
\end{align}
\end{cases}
$$
