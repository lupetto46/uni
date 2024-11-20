Un sistema lineare omogeneo è un sistema lineare in cui tutti i termini noti sono uguali a zero.
$$
    \begin{cases}
        a_{11}x_1 + a_{12}x_2 + \dots + a_{1n}x_n = 0\\
        a_{21}x_1 + a_{22}x_2 + \dots + a_{2n}x_n = 0\\
        \vdots\\
        a_{m1}x_1 + a_{m2}x_2 + \dots + a_{mn}x_n = 0\\
    \end{cases} \iff AX=0
$$

in questo caso $A|B$ ammette sempre almeno una soluzione che è la soluzione con tutti zero ovvero $\begin{pmatrix} 0\\ \vdots\\ 0 \end{pmatrix}\in M_{n,1}$


> [!todo] Osservazione
> Avendo $Y,Y'$ soluzioni di $AX=0\iff AY'=0=AY$
>
> Considerando che $A(Y+Y')=AY+AY'=0+0=0$ e $A(-Y)=-(AY)=0$ per tutte le soluzioni $\Sigma_0\{\text{soluzioni di }AX=0\}$ allora $(AX, +, 0)$ è un \textbf{gruppo abeliano}
> 
> Anche se questo funziona solo per i sistemi omogenei.