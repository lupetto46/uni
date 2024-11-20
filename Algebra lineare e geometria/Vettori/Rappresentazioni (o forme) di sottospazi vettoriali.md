### Forma cartesiana e parametrica
Per rappresentare i sottospazi vettoriali ci sono due modi. 
Ognuno di questi ha i suoi pro e i suoi contro di cui ne parleremo dopo

#### Forma cartesiana
$$
    V= \begin{cases}
        a_{11}x_1 + \dots + a_{1n}x_n = 0\\
        \vdots \\
        a_{m1}x_1 + \dots + a_{mn}x_n = 0
    \end{cases}= AX=0 =: ker(A)
$$

Di cui $A$:
$$
    A = \begin{pmatrix}
        a_{11} & \dots & a_{1n}\\
        \vdots & \ddots & \vdots\\
        a_{1m} & \dots & a_{mn}
    \end{pmatrix} \in M_{m,n}(K)
$$

E il kernel di $A$ ($ker(A)$) è l'insieme di tutti i vettori di $X$ tali che $AX=0$

#### Forma parametrica
Ci si riferisce invece alla forma parametrica come $<v_1, v_2, \dots, v_r>$
E viene definito come $row(B)$ ovvero una matrice formata da tutti i vettori all'interno dell'insieme coricati riga per riga
$$
    <v_1, v_2, \dots, v_r> =: row (B), B = \begin{pmatrix}
        V_1\\
        V_2\\
        \vdots\\
        V_r
    \end{pmatrix}
$$