---
Time: 2024-11-21 10:52
---
Se una funzione è biiettiva, allora è invertibile. 
Se il $\text{cod } f=f(x)$ allora basta che sia iniettiva.
Se una funzione $f$ è iniettiva, possiamo associare a ogni elemento di $y$ dell'immagine l'unico elemento $x$ del dominio tale che $f(x)=y$.

Tale corrispondenza determina una funzione definita in $Y$ a valori in $X$, che viene detta *funzione inversa* di $f$, indicata come $f^{-1}$
$$
x=f^{-1}(y) \iff y = f(x)
$$
$$
f^{-1}:\text{Im }f \to \text{dom }f
$$

Una funzione biiettiva (o iniettiva) è dunque invertibile. Il grafico della funzione inversa si ottiene  scambiando tra loro le componenti di ciascuna coppia.
$$
\begin{align}
&\varGamma(f^{-1})=\{(y,f^{-1}(y))\in Y\times X :y \in \text{dom } f^{-1}\}=\\
&=\{(f(x), x) \in Y\times Y: x \in \text{dom }f\}
\end{align}
$$

Nel caso di una funzione reale in variabile, tale scambio corrisponde al "riflesso" rispetto alla retta $y=x$

> [!attention] Attenzione
> Spesso, qualora sia possibile determinare la funzione inversa nella forma $x=f^{-1} (y)$, si preferisce tornare ad indicare la variabile indipendente ($f^{-1}(y)$) con $x$ e la variabile dipendente ($x$) con $y$, per essere in grado di tracciarne il grafico. Otteniamo così:
> $$
> x= f^{-1}(y) \implies y=f^{-1}(x)
> $$