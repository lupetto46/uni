> [!success] Corollario 4
> $V,W$ spazi vettoriali su $K, dim\ V=n,dim\ W=m, f:V\to W$ omomorfismo
> 1. $f$ iniettiva $\iff n\leq m$
> 2. $f$ suriettiva $\iff n \geq m$
> 3. $f$ biiettiva $\iff n = m$

> [!success] Teorema (*dell'isomorfismo*)
> $V$ spazio vettoriale  su $K$, $dim\ V=n$, allora $V\simeq K^n$
> > [!summary] Dimostrazione
> > Avendo $B = \{b_1,\ldots, b_n\}$ base di $V$
> > $$
> > \begin{align}
> > \varphi: V &\to K^n\\
> > b_1 &\mapsto \varphi(b_1) = e_1 = (1\ 0\ \dots\ 0)
> > \end{align}
> > $$
> > Allora $\{\varphi(b_1), \dotsb, \varphi(b_n)\}= \varepsilon$ che seguendo il [[Proprietà degli omomorfismi#^7444b5|corollario 3]] è biiettiva 

Da qui già si può capire che la cosa più importante è stabilire una base. Infatti:

$V$ spazio vettoriale di $dim\ V=n, B=\{b_1,\dots, b_n\}$ base di $V$

Ma cosa significa che $B$ è una base?

Vuol dire che $v\in V\implies \exists!\lambda_1,\dots,\lambda_n\in K \text( t. c. ) v=\lambda_1b_1 + \dots + \lambda_nb_n \implies$
$\implies v\in V\rightsquigarrow \begin{pmatrix} \lambda_1\\ \lambda_2\\ \vdots\\ \lambda_n \end{pmatrix} \in K^n$

Quindi $\varphi(v) = \varphi(\lambda_1v_1+\dots+\lambda_nv_n)=\lambda_1\varphi(v_1)+\dots+\lambda_n\varphi(v_n)=$
$\lambda_1e_1+\dots+\lambda_ne_n=\lambda_1\begin{pmatrix} 1\\ 0\\ \vdots\\ 0 \end{pmatrix} +\dots+\lambda_n \begin{pmatrix} 0\\ 0\\ \vdots\\ 1 \end{pmatrix}= \begin{pmatrix} \lambda_1\\ \lambda_2 \\ \vdots \\ \lambda_n \end{pmatrix}$
### Con i polinomi
#### Esempio
$K[X]_{\leq 2}=\{a+bx+cx^2\mid a,b,c \in ℝ\}$
In questo caso la dimensione è $dim\ (K[x]_{\leq 2})= 3$ in quanto la base standard $B=\{1, x, x^2\}$

$$
\begin{align}
	\varphi: K[X]_{\leq 2} &\to K^3\\
	1&\mapsto \begin{pmatrix}
	1\\0\\0
	\end{pmatrix}\\
	x& \mapsto \begin{pmatrix}
	0\\1\\0
	\end{pmatrix}\\
	x^2&\mapsto \begin{pmatrix}
	0\\0\\1
	\end{pmatrix}
\end{align}
$$
Ottenendo quindi qualcosa come $a+bx+cx^2 = \begin{pmatrix} a\\b\\c \end{pmatrix}$

Ma questo se si sceglie la "*base standard*". È possibile anche cambiare base ed è come se si stesse cambiando **sistema di rappresentazione del vettore**:
Usando la base $C = \{1+x, x+x^2, 1+x^2\}$
$$
\begin{align}
	\tau:K[X]_{\leq 2}&\to K^3\\
	1 + x &\mapsto \begin{pmatrix}
	1\\0\\0
	\end{pmatrix}\\
	x + x^2 & \mapsto \begin{pmatrix}
	0\\1\\0
	\end{pmatrix}\\
	1 + x^2 &\mapsto \begin{pmatrix}
	0\\0\\1
	\end{pmatrix}
\end{align}
$$