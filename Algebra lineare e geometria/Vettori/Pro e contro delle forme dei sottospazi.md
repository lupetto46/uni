### Somma di sottospazi (forma cartesiana)
La forma migliore da usare per fare una somma di sottospazio è la forma cartesiana.

$V,W \subseteq K^n \longrightarrow V=row A,\ W=row B$
$A\in M_{m_1,n}(K),\qquad B\in M_{m_2,n}$

$$
C= \left(\frac{A}{B}\right) \in M_{m_1+m_2, n} \implies V \oplus W = row(C)
$$

##### Esercizio di esempio
$$
V = <\begin{pmatrix}
1\\1\\2
\end{pmatrix},\begin{pmatrix}
2\\2\\2
\end{pmatrix}>, \qquad W=<\begin{pmatrix}
0\\1\\0
\end{pmatrix}, \begin{pmatrix}
0\\0\\1
\end{pmatrix}> \subseteq ℝ^3
$$
$$
V= row\begin{pmatrix}
1 & 2& 1\\
2 & 2& 2
\end{pmatrix}, \qquad W=row\begin{pmatrix}
0 & 1 & 0\\
0 & 0 & 1
\end{pmatrix}
$$
$$
V\oplus B= row\begin{pmatrix}
1 & 2& 1\\
2 & 2& 2\\
0 & 1 & 0\\
0 & 0 & 1
\end{pmatrix} = \overbrace{<\begin{pmatrix}
1\\2\\1
\end{pmatrix},\begin{pmatrix}
2\\2\\2
\end{pmatrix},\begin{pmatrix}
0\\1\\0
\end{pmatrix},\begin{pmatrix}
0\\0\\1
\end{pmatrix}>}^4
$$
Il fatto che sia dimensione 4 significa che uno dei vettori non è necessario per creare la base. Per capire come rimuoverlo basta eseguire Gauss (non è necessario il passo Jordan) e verrà rimossa una riga che sarà la riga di troppo.

$$
\begin{pmatrix}
1 & 2& 1\\
2 & 2& 2\\
0 & 1& 0\\
0 & 0& 1
\end{pmatrix} \xrightarrow{r_2 \rightarrow \frac{r_2}{2}}\begin{pmatrix}
1 & 2& 1\\
1 & 1& 1\\
0 & 1& 0\\
0 & 0& 1
\end{pmatrix} \xrightarrow{r_2 \rightarrow r_2 - r_1}\begin{pmatrix}
1 & 2& 1\\
0 & -1& 0\\
0 & 1& 0\\
0 & 0& 1
\end{pmatrix} \xrightarrow{r_3 \rightarrow r_3 + r_2}
$$
$$
\begin{pmatrix}
1 & 2& 1\\
0 & -1& 0\\
0 & 0& 0\\
0 & 0& 1
\end{pmatrix} = \begin{pmatrix}
1 & 2& 1\\
0 & 1& 0\\
0 & 0& 1\\
0 & 0& 0
\end{pmatrix}
$$
Si prendono quindi solo le righe non nulle
$$
V= <\begin{pmatrix}
1\\2\\1
\end{pmatrix},\begin{pmatrix}
0\\1\\0
\end{pmatrix},\begin{pmatrix}
0\\0\\1
\end{pmatrix}>\implies \left\{\begin{pmatrix}
1\\2\\1
\end{pmatrix},\begin{pmatrix}
0\\1\\0
\end{pmatrix},\begin{pmatrix}
0\\0\\1
\end{pmatrix}\right\} \text{ base di }V
$$
$$
V= ℝ^3
$$

### Intersezione di sottospazio (forma parametrica)
Per calcolare la base di un'intersezione di sottospazi la forma migliore è la parametrica.

$$
V,W\subseteq K^n, V=\ker(A), w=\ker(B), C =(\frac{A}{B})
$$
$$
V\cap W = \ker(C)
$$

##### Esempio
$$
\begin{align*}
&V=<\begin{pmatrix}
1\\2\\1
\end{pmatrix}, \begin{pmatrix}
2\\2\\2
\end{pmatrix}>, W=<\begin{pmatrix}
0\\1\\0
\end{pmatrix}, \begin{pmatrix}
0\\0\\1
\end{pmatrix}>
\\
&V=row\begin{pmatrix}
1 & 2 & 1\\
2 & 2 & 2
\end{pmatrix} = row A \implies \ker A =\ker \begin{pmatrix}
1 & 2 & 1\\
2 & 2 & 2
\end{pmatrix}
\\
&\begin{pmatrix}
1 & 2&1\\
2&2&2
\end{pmatrix} \xrightarrow{r_2\rightarrow \frac{r_2}{2}} \begin{pmatrix}
1&2&1\\
1&1&1
\end{pmatrix}\xrightarrow{r_2\rightarrow -1\cdot(r_2-r_1)} \begin{pmatrix}
1&2&1\\
0&1&0
\end{pmatrix}
\\
&= \begin{pmatrix}
1&0&1\\
0&1&0
\end{pmatrix}
\end{align*}
$$

$$
\begin{align}
&W=row\begin{pmatrix}
0&1&0\\
0&0&1
\end{pmatrix} \implies \ker\begin{pmatrix}
0&1&0\\
0&0&1
\end{pmatrix}
\\
&\begin{cases}
x_2 = 0\\
x_3 = 0
\end{cases}\rightarrow \begin{pmatrix}
x_1\\
0\\
0
\end{pmatrix}=\begin{pmatrix}
1\\0\\0
\end{pmatrix}x_1\implies<\begin{pmatrix}
1\\0\\0
\end{pmatrix}> = row\begin{pmatrix}
1 & 0 & 0
\end{pmatrix}\implies
\\
&\implies W = ker\begin{pmatrix}
1&0&0
\end{pmatrix}= \{x_1=0
\end{align}
$$

$$
\begin{align*}
&V\cap W \begin{cases}
-x_1+x_3 = 0\\
x_1=0
\end{cases}= \ker\begin{pmatrix}
-1 & 0 & 1\\
1 & 0 & 0
\end{pmatrix}\xrightarrow{r_1 \rightarrow -1\cdot r_1}\\
&\ker\begin{pmatrix}
1 & 0 & -1\\
1 & 0 & 0
\end{pmatrix} \xrightarrow{r_2 \rightarrow r_2-r_1}\ker\begin{pmatrix}
1 & 0 &-1\\
0 & 0 & 1
\end{pmatrix}\xrightarrow{r_1\rightarrow r_1+r_2}\\
&\ker\begin{pmatrix}
1 & 0 &0\\
0 & 0 &1
\end{pmatrix} = \begin{cases}
x_1 = 0\\
x_3 = 0
\end{cases} = \begin{pmatrix}
0\\x_2\\0
\end{pmatrix}=\begin{pmatrix}
0\\1\\0
\end{pmatrix}x_2=<\begin{pmatrix}
0\\1\\0
\end{pmatrix}>
\end{align*}
$$