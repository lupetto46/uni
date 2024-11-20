$K^3=\left\{\begin{pmatrix} a\\b\\c \end{pmatrix}\mid a,b,c\in K\right\}$

$v=\begin{pmatrix} 1\\2\\1 \end{pmatrix} = 1\cdot\begin{pmatrix} 1\\0\\0 \end{pmatrix}+2\begin{pmatrix} 0\\1\\0 \end{pmatrix}+1\begin{pmatrix} 0\\0\\1 \end{pmatrix}$

Tutto questo però si può fare seguendo anche un'altra base ad esempio
$B =\{(1,1,0),(0,1,1),(1,0,1)\}$ base di $K^3$

$v=\begin{pmatrix} 1\\2\\1 \end{pmatrix} =$ *$1$* $\cdot\begin{pmatrix} 1\\1\\0 \end{pmatrix}+$*$1$* $\begin{pmatrix} 0\\1\\1 \end{pmatrix}+$ *$0$*$\begin{pmatrix} 1\\0\\1 \end{pmatrix}=[V]_B=\begin{pmatrix} 1\\1\\0 \end{pmatrix}$
Di cui il vettore finale sono i vettori evidenziati.

$[V]_B$ coordinate di $V$ rispetto a $B$

---
$V,W$ spazi vettoriali. $dim\ V=n,dim\ W=m, B_V=\{v_1,\dots, v_n\}\text{ base di }V,\ B_W=\{w_1,\dots, w_m\}\text{ base di }B$
$$
f:V\to W\text{ omomorfismo},\quad \{f(v_1),\dots, f(v_n)\}\subset W
$$
$$
f(v_j)=a_{1\ j}\cdot w_1 +\dots + a_{m\ j}\cdot w_m\forall j=1,\dots,n
$$
$v\in V$ si scrive $f(v)$ 
Di cui $V=\lambda_1v_1+\dots + \lambda_nv_n\implies f(v)=f(\lambda_1v_1 +\dots + \lambda_nv_n)= \lambda_1 f(v_1)+\dots+\lambda_nf(v_n)=$$=\lambda_1(a_{11}w_1+\dots+a_{m1}w_m)+\dots+\lambda_n(a_{1n}w_1+\dots+a_{mn}w_m)$
$=(\lambda_1a_{11}+\dots+\lambda_na_{1n})w_1+\dots+(\lambda_1a_{m1}+\dots+\lambda_na_{mn})w_m$
Di cui:
$w_1 = \begin{pmatrix} 1\\0\\\vdots\\0 \end{pmatrix}, w_m+\begin{pmatrix} 0\\0\\\vdots\\1 \end{pmatrix}$

Otteniamo quindi che:
- $W\simeq K^n$
- $B_W$
- $V\simeq K^n$
- $B_V$
$$
=\begin{pmatrix}
	\lambda_1a_{11}&+&\dots&+&\lambda_na_{1n}\\
	\vdots &&\ddots&& \vdots\\
	\lambda_1a_{m1}&+&\dots&+&\lambda_na_{mn}\\
\end{pmatrix}=[f(v)]_{B_{_W}}
$$
$$
A=(a_{ij})_{\underset{1\leq j\leq n}{1\leq i\leq m}}\in M_{m,n}(K)
$$
$$
[V]_{B_{_V}}=\begin{pmatrix}
	\lambda_1\\
	\vdots\\
	\lambda_n
\end{pmatrix}
$$