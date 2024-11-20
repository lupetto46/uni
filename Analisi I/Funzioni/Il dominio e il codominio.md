---
Data: 24-11-2024
---
Siano $X$ e $Y$ due insiemi non nulli. Una funzione $f$ definita in $X$ a valori in $Y$ è una corrispondenza che associa a ogni elemento di $x\in X$ uno e uno solo elemento $y\in Y$

L'insieme degli $x\in X$ a cui $f$ associa un elemento di $Y$ forma il ***dominio*** di $f$, questo viene indicato con $\text{dom }f$.

Invece l'insieme che include tutti i possibili valori che questa funzione può prendere si chiama ***codominio*** che indichiamo con $\text{cod } f$.

Quindi si scrive matematicamente
$$
f:X\to Y \implies f:\text{dom }f\to \text{cod }f
$$

L'elemento $y\in\text{cod }f$ associato a un elemento di $x\in\text{dom }f$ si dice *immagine di $x$ attraverso $f$*, che indichiamo con $y=f(x)$ che forma ***l'immagine*** di $f$, esso è dunque un sottoinsieme di: $\text{Im }f=\{y\in\text{cod }f\mid \exists n\in\text{dom }f:y=f(x)\}$

![[Pasted image 20241120223138.png|600]]
Il grafico di $f$ è il sottoinsieme $\varGamma(f)$ del prodotto cartesiano $X\times Y$ costituito dalle coppie $(x,f(x))$ al valore di $x$ nel dominio di $f$
$$
\varGamma(f)=\left\{(x,f(x))\\in X\times Y:x\in \text{dom }f\right\}
$$

Se $Y=ℝ,$ allora funzione si dice *reale*
Se $Y=ℝ^n,$ la funzione si dice *di $n$ variabili reali*

Si definisce *dominio naturale* il più grande sottoinsieme di $ℝ$ per il quale $f(x)$ ha senso esempio:
$$
y=\begin{cases}
&\ln x \qquad &(0;1)\\
&x^2+2x+1\qquad &[1;3]
\end{cases}
$$
È una funzione definita a tratti

