$A\in M_{n,n} (K)$ il determinante di $A$ è definito come:
$$
    det (A) = |A|:= \sum_{\sigma \in \$_n} sign(\sigma) \cdot \prod_{i=1}^n a_{i,\sigma(i)}
$$

### Proprietà del determinante
Se una matrice è triangolare o diagonale allora il determinante è il prodotto degli elementi sulla diagonale.
$$
    A \in M_{n,n} (K) \text{ se } A \text{ è triangolare o diagonale allora } det A= \prod_{i=1}^n a_{i,i}
$$

> [!success] Lemma
> Il $det A^t= det A$
> > [!todo] Dimostrazione
> > Avendo $A\in M_{n,n} (K),\quad i \in \{1,2,\dots,n\}$\\
> > $A^{(i)}=(a_{1,i}\ a_{2,i}\ \dots\ a_{n,i})$ Quindi $A^{(i)}$ è la $i$-esima riga di $A$
> > $$
> >             det A = \alpha\cdot det \begin{pmatrix} A^{(1)}\\ \vdots\\ V\\ \vdots\\ A^{(n)}\end{pmatrix} + \alpha'\cdot det \begin{pmatrix} A^{(1)}\\ \vdots\\ V'\\ \vdots\\ A^{(n)} \end{pmatrix}
> > $$

> [!success] Lemma
> Se $A'$ è la matrice ottenuta scambiando $2$ righe di $A$ allora  $det A' = -det A$

> [!success] Corollario
> Se $A$ è la matrice ottenuta applicando la permutazione $\sigma$ alle righe di $A$ allora $det A' = sign(\sigma) \cdot det A$

> [!success] Proposizione
> - Se $A^{(i)}= (0\ \dots\ 0)$ allora $det A = 0$
> - $\text{Se } \exists i\neq j : A^{(i)}=A^{(j)} \text{ allora } det A = 0$
> - $$\det \begin{pmatrix} A^{(1)}\\ \vdots\\ A^{(i)} + \alpha\cdot A^{(j)}\\ \vdots\\ A^{(n)}\\ \end{pmatrix} = \det \begin{pmatrix} A^{(1)}\\ \vdots\\ A^{(i)}\\ \vdots\\ A^{(n)}\\ \end{pmatrix} + \alpha \cdot det \begin{pmatrix} A^{(1)}\\ \vdots\\ A^{(j)}\\ \vdots\\ A^{(n)}\\ \end{pmatrix} = det A $$
> - In quanto $$ \alpha \cdot det \begin{pmatrix} A^{(1)}\\ \vdots\\ A^{(j)}\\ \vdots\\ A^{(n)}\\ \end{pmatrix} = 0 $$ Siccome $A^{(j)}$ prende il posto di $A^{(i)}$ troviamo che $A^{(i)}=A^{(j)}$ ma visto che abbiamo due righe identiche in quanto seguendo l'equazione \eqref{det:due righe identiche} otteniamo che è uguale a $0$ e quindi solo il $\det A$
> - $$\det \begin{pmatrix} A^{(1)}\\ \vdots\\ \alpha\cdot A^{(i)}\\ \vdots\\ A^{(n)}\\ \end{pmatrix}=\alpha\cdot\det A$$

> [!important] Importante
> Importante:
Visto che $\det A^t= \det A$ allora tutte le proprietà del determinante valgono anche per le colonne.

## Usare il determinante per capire qual è il rango di una matrice
Il problema più grande è quello che il rango è calcolabile in tutte le matrici, ma il determinante solo in quelle quadrate.

Per questo motivo dobbiamo vedere una serie di proposizioni

> [!success] Proposizione
> Sia $A\in M_{m,n}(K), B\in M_{m,r}(K)$
> - $rk(AB)\leq min(rk(A), rk(B))$.
> - Se $m=n$ e $A$ è invertibile allora $rk(AB) = rk(B)$.
> - Se $n=r$ e $B$ è invertibile allora $rk(AB) = rk(A)$.

> [!success] Proposizione
> Se $B$ è una sottomatrice di $A$, allora $rk(B)\leq rk(A)$

> [!success] Teorema
> $A\in M_{m,n}(K)$ allora $rkA=$ guardando tutte le sottomatrici quadrate si prende il rango della sottomatrice quadrata più grande che non ha determinante nullo.