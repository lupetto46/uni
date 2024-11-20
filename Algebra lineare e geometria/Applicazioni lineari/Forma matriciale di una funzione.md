Abbiamo quindi ottenuto $[f(V)]_{B_{W}}=A\cdot [V]_{B_{V}}$
Sapendo che $A=[M]^{^{B_{V}}}_{_{B_W}}$
Otteniamo la relazione: $[f(V)]_{B_{W}}=[M]^{^{B_{V}}}_{_{B_W}}\cdot [V]_{B_{V}}$
Di cui $[M]^{^{B_{V}}}_{_{B_W}}$ è la matrice che rappresenta l'applicazione lineare ed è creata mettendo tutti i vettori della base $B_W$ in verticale:
$$
[M]^{^{B_{V}}}_{_{B_W}}=\begin{pmatrix}
	f(v_1)_{B_W}&\dotsb&f(v_n)_{B_W}
\end{pmatrix}
$$

### Esempio trovare la matrice rappresentante
$$
\begin{align}
	g:ℝ^2&\to ℝ^3\\
	\begin{pmatrix}
	x\\y
	\end{pmatrix}&\mapsto \begin{pmatrix}
	2x\\ x+y\\ 2y
	\end{pmatrix}
\end{align}
$$
Poi si devono definire le due basi di $ℝ^3$ e $ℝ^2$:
$$
\begin{align}
	&\varepsilon_2=\left\{\begin{pmatrix}
	1\\0
	\end{pmatrix},\begin{pmatrix}
		0\\1
	\end{pmatrix}\right\}\\
	&\varepsilon_3=\left\{\begin{pmatrix}
	1\\0\\0
	\end{pmatrix},\begin{pmatrix}
	0\\1\\0
	\end{pmatrix},\begin{pmatrix}
	0\\0\\1
	\end{pmatrix}\right\}
\end{align}
$$
Poi si calcola utilizzando le due basi a cosa risulta $f(v)$
$$
g\begin{pmatrix}
	1\\0
\end{pmatrix}=\begin{pmatrix}
	2\\1\\0
\end{pmatrix},g\begin{pmatrix}
	0\\1
\end{pmatrix}=\begin{pmatrix}
	0\\1\\2
\end{pmatrix}
$$

Prendiamo quindi i due vettori e mettiamoli in colonna:
$$
[M]^{\varepsilon_2}_{\varepsilon_3}=\begin{pmatrix}
	2 & 0\\
	1 & 1\\
	0 & 2
\end{pmatrix}\in M_{3,2}(ℝ)
$$

### Esempio da matrice ad applicazione lineare
Avendo quindi la matrice:
$$
\begin{pmatrix}
	2 & 1& 0 &4 \\
	2&3&2&6
\end{pmatrix}
$$
Essendoci $4$ colonne sappiamo che ci sono $4$ variabili e sappiamo che:
$$
\begin{pmatrix}
	x\\ y\\ z\\ w
\end{pmatrix}=xe_1+ye_2+ze_3+we_4
$$

Si scrive quindi così:
$$
\begin{align}
	f:ℝ^4&\to ℝ^2\\
	e_1&\mapsto\begin{pmatrix}
		2\\2
	\end{pmatrix}\\
	e_2&\mapsto\begin{pmatrix}
		1\\3
	\end{pmatrix}\\
	e_3&\mapsto\begin{pmatrix}
		0\\2
	\end{pmatrix}\\
	e_4&\mapsto\begin{pmatrix}
		4\\6
	\end{pmatrix}
\end{align}
$$

> [!success] Teorema
> $V,W$ spazi vettoriali su $K$. $dim\ V=n,dim\ W=m$
> $Hom(V,W)\simeq M_{m,n}(K)$
> L'isomorfismo dipende dalla scelta delle basi di $V$ e $W$

$Hom(V,V)$ quindi un $End(V)\simeq M_{n,n}(K)$
$\varepsilon$ basi di $V$ nel dominio e codominio 

Sappiamo che
$id\ n\in M_{n,n}(K) \longleftrightarrow id\ v\in End(V)$

E che lo zero è:
$0\in M_{n,n}(K) \longleftrightarrow 0 \in End(V)$

> [!success] Proposizione
> $V,W,U$ spazi vettoriali di dimensioni $n,m,p$ rispettivamente
> *fissiamo le basi (**importante**)*, $f:V\to W\quad g:W\to U$ applicazioni lineari
> $M(g\circ f)=M(g)\cdot M(f)$
> Di cui:
> - $M(g\circ f) \in M_{p,n}$
> - $M(g) \in M_{p,m}$
> - $M(f)\in M_{m,n}$

> [!success] Corollario
> $f:V\to V$ endomorfismo biiettivo
> *fissiamo le basi di $V$*
> $M(f^{-1})=M(f)^{-1}$