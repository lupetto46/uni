$B, W$ spazi vettoriali su $K$, avendo una funzione $f:V\longrightarrow W$ 

$f$ è un'applicazione lineare se:
- $\forall v_1,v_2 \in V\qquad f(v_1 + v_2)=f(v_1)+f(v_2)$
- $\forall v \in V, \forall \lambda \in K\quad f(\lambda \cdot v) = \lambda \cdot f(v)$

> [!example] Esempio 1
> $\begin{align}f: ℝ^2 &\longrightarrow ℝ^3\\ \begin{pmatrix}x\\y\end{pmatrix}&\longmapsto \begin{pmatrix}2x\\x+y\\2y\end{pmatrix}\end{align}$
> 
> In questo caso controlliamo se soddisfa il primo punto:
> $$
> \begin{align}
> &f(\begin{pmatrix}
> x_1\\ y_1
\end{pmatrix}+\begin{pmatrix}
> x_2\\ y_2
\end{pmatrix}) = \begin{pmatrix}
> 2(x_1+x_2)\\ x_1 + x_2 + y_1+y_2\\2(y_1+y_2)
\end{pmatrix}=\\
> =&\begin{pmatrix}
> 2x_1\\ x_1+y_1\\ 2y_1\end{pmatrix} + \begin{pmatrix}2x_2\\ x_2+y_2\\ 2y_2
\end{pmatrix}=f\begin{pmatrix}
> x_1\\ y_1
\end{pmatrix} +f\begin{pmatrix}
> x_2\\ y_2
\end{pmatrix}
\end{align}
> $$
> 
> Poi controlliamo se soddisfa la seconda proprietà
> $$
> \begin{align}
> &f\left(\lambda \begin{pmatrix}
> x\\ y
\end{pmatrix}\right) = f\begin{pmatrix}
> \lambda x\\ \lambda y
\end{pmatrix}=\begin{pmatrix}
> 2\lambda x\\ \lambda x+\lambda y\\ 2\lambda y
\end{pmatrix} = \lambda\begin{pmatrix}
> 2x \\ x+y \\ 2y
\end{pmatrix}=\\
> =&\lambda f\begin{pmatrix}
> x\\ y
\end{pmatrix}
\end{align}
> $$
> Essendo tutte e due questo è un omomorfismo

> [!example] Esempio 2:
> $$
> \begin{align}
> f:V&\longrightarrow W\\
> v&\longmapsto 0
> \end{align}\qquad \text{ si chiama omomorfismo nulllo}
> $$

> [!example] Esempio 3
> $$
> \begin{align}
> f:ℝ^3 &\longrightarrow ℝ^2\\
> \begin{pmatrix}
> x\\ y\\ z
\end{pmatrix} &\longmapsto \begin{pmatrix}
> x^2 +y \\ z
\end{pmatrix}
\end{align}
> $$
> In questo caso non è un omomorfismo in quanto un polinomio elevato a 2 da un valore particolare 

> [!example] Esempio 4
> $$
> \begin{align}
> f:ℝ^2 &\longrightarrow ℝ^2\\
> \begin{pmatrix}
> x\\ y
\end{pmatrix}& \longmapsto \begin{pmatrix}
> y- 1 \\ y + x
\end{pmatrix}
\end{align}
> $$
> Non è un omomorfismo in quanto non soddisfa la seconda proprietà:
> $$
> f\begin{pmatrix}
> 0 \\ 0
\end{pmatrix} = \begin{pmatrix}
> -1 \\ 0
\end{pmatrix}
> $$
> Ma
> $$
> \begin{align}
> f\begin{pmatrix}
> 0 \\ 0
\end{pmatrix}= f \left(0 \begin{pmatrix}
> 0 \\ 0
\end{pmatrix}\right)= 0 f\begin{pmatrix}
> 0 \\ 0
\end{pmatrix} =\begin{pmatrix}
> 0 \\ 0 
\end{pmatrix} \neq \begin{pmatrix}
> -1 \\ 0
\end{pmatrix}
\end{align}
> $$


In base le coordinate devono essere monomi di primo grado

> [!success] Lemma 
> $f: V\longrightarrow W$ è un monomorfismo, allora $f(0)=0$