$f:V\to W\rightsquigarrow \ker f \subseteq V,Im\ f\subseteq W$

> [!success] Proposizione
> $f:V\to W$ omomorfismo
> fissiamo le basi sia di $V$ che di $W$ e sia $M$ la matrice rappresentante $f$
> Otteniamo che:
> - $\ker f \simeq \ker M$
> - $\text{Im}\ f \simeq \text{col } M=\text{ spazio generato dalle colonne di }M$

### Esempio
$$
\begin{align}
	f:ℝ^3 &\to ℝ^2\\
	\begin{pmatrix}
	x\\ y\\ z
	\end{pmatrix}&\mapsto \begin{pmatrix}
	x + y \\ y + z
	\end{pmatrix}
\end{align}
$$

$$
f\begin{pmatrix}
	1\\0\\0
\end{pmatrix}=\begin{pmatrix}
	1\\0\\
\end{pmatrix}, f\begin{pmatrix}
	0\\1\\0
\end{pmatrix}=\begin{pmatrix}
	1\\1
\end{pmatrix},f\begin{pmatrix}
	0\\0\\1
\end{pmatrix}=\begin{pmatrix}
	0\\1
\end{pmatrix}
$$ Per trovare il kernel di:
$$
\left\{\begin{pmatrix}
	1\\0
\end{pmatrix},\begin{pmatrix}
	1\\1
\end{pmatrix},\begin{pmatrix}
	0\\1
\end{pmatrix}\right\}
$$
Di cui la matrice rappresentate è:
$$
M(f)=\begin{pmatrix}
	1&1&0\\
	0&1&1\\
\end{pmatrix}
$$
Sapendo che $\ker f \simeq \ker M$ dobbiamo trovare il kernel. Quindi si fa la forma di Echelon ridotta:
$$
\begin{pmatrix}
	1&0&-1\\
	0&1&1
\end{pmatrix} \begin{cases}
	x = z\\
	y = -z
\end{cases} \implies \begin{pmatrix}
	x\\
	y\\
	z
\end{pmatrix}=\begin{pmatrix}
	z\\
	-z\\
	z
\end{pmatrix}=
$$
$$
=z\begin{pmatrix}
	1\\
	-1\\
	1
\end{pmatrix}= <\begin{pmatrix}
	1\\-1\\1
\end{pmatrix}>
$$

Ottenendo quindi il kernel

Ora dobbiamo trovare l'immagine 
$$
Im(f) \simeq <\begin{pmatrix}
	1\\0
\end{pmatrix},\begin{pmatrix}
	1\\1
\end{pmatrix},\begin{pmatrix}
	0\\1
\end{pmatrix}>= \underbrace{<\begin{pmatrix}
	1\\0
\end{pmatrix}
\begin{pmatrix} 0\\1 \end{pmatrix}>}_{\text{base di } ℝ} = ℝ^2
$$

Otteniamo quindi che $f$ è suriettiva ma non iniettiva.

> [!success] Corollario
> Se $f$ è un omomorfismo e $M$ la matrice che lo rappresenta
> $\text{null}(f)=\text{null}(M), \text{rk}(f)=\text{rk}(M)$
> 
> E che $\text{null}(f)=\text{dim}(\ker f)$

Ricordare anche che $f\text{ iniettiva }\iff \ker M = \left\{\begin{pmatrix} 0\\0\\\vdots\\0 \end{pmatrix}\right\}$