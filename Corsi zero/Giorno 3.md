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
> Il professore qui ha fatto utilizzare una cosa chiamata "delta 4" ($\frac{\Delta}{4}$) che si può utilizzare **solo** se il coefficiente della $x$ di primo grado è pari e serve nel caso in cui i numeri da calcolare nel delta sono troppo alti

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

## Disequazioni irrazionali
Le radici hanno
$\sqrt[n]{radicando}$

Il cui risultato è: *quel numero che elevato a $n$ restituisce il $radicando$*
Per adesso però considereremo solo radici la cui $n=2$

Prendiamo quindi di esempio 2