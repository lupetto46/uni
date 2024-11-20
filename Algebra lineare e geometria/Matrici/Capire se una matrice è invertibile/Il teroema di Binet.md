$$
    A,B \in M_{n,n} (K), \quad det(A\cdot B) = det A \cdot det B
$$

### Dimostrazione
$A=(a_{ij}), \quad B = (b_{ij})$
$$
    \begin{align}
        A \cdot B &= \begin{pmatrix}
            a_{11}\cdot b_{11} + \dots + a_{1n}\cdot b_{n1} & \dots & a_{11}\cdot b_{1n} + \dots + a_{1n}\cdot b_{nn}\\
            \vdots & \ddots & \vdots\\
            a_{n1}\cdot b_{11} + \dots + a_{nn}\cdot b_{n1} & \dots & a_{n1}\cdot b_{1n} + \dots + a_{nn}\cdot b_{nn}\\
        \end{pmatrix}=\\
        &= \begin{pmatrix}
            a_{11}\cdot B^{(1)} + a_{12}\cdot B^{(2)} + \dots + a_{1n}\cdot B^{(n)}\\
            \vdots\\
            a_{n1}\cdot B^{(1)} + a_{n2}\cdot B^{(2)} + \dots + a_{nn}\cdot B^{(n)}\\
        \end{pmatrix}
    \end{align}
$$
Facendo lo stesso procedimento con le righe otteniamo che:
$$
        det A\cdot B = \sum_{j_1, \dots, j_n}^{n} a_1j_1\cdot \dots \cdot a_nj_n\cdot det \begin{pmatrix}
            B^{(j_1)}\\
            \vdots\\
            B^{(j_n)}\\
        \end{pmatrix}
$$
Ma visto che:
$$
        \Biggl(\underbrace{\sum_{\sigma \in \$} a_{\sigma(1)}\cdot \dots \cdot a_{\sigma(n)}}_{det A}\Biggr)\cdot det B= det A \cdot det B
$$

> [!success] Corollario
> $A\in M_{n,n}(K)$ invertibile $\Longrightarrow det A^{-1} = \frac{1}{det A}$
>
>$A^{-1}\cdot A = id_n,\qquad det(id_n) = 1$
>
> $det (id_n) = det A^{-1} \cdot det A$

> [!success] Corollario
> Se $A\in M_{n,n}(K)$ è invertibile $\Longrightarrow det A \neq 0$
> 
> Significa che se una matrice ha determinante 0 allora non è invertibile.