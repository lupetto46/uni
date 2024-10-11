#algebra_lineare_e_geometria
Considerando che $a\in S$ è invertibile, dimostrare che il suo inverso è unico

$\exists b\in S:b*a=e=a*b$
Supponiamo per assurdo che : 
$\exists c\in S: c*a=e=a*c$
Ma allora:
$c*a=a*c=e$
$b*a=a*b=e$ 
Di conseguenza
$b*a=e=c*a$
quindi $c=b$

## Dimostrare che in generale $(\$_n, \circ)$ non è commutativo

$\$_n$
$(\$_n, \circ)$ non commutativo:
Commutativo $\Rightarrow \forall a,b \in S \quad a \circ b = b\circ a$

Ci sono due casi $n\geq 3$ e $n<3$
Nel caso in cui $S_n\quad n=1$ allora di permutazioni ce ne sarebbero solo una che lascia l'elemento invariato. Rendendo quindi $\sigma=id_1$ 

Perché una funzione che manda l'unico valore di $S$ a se stesso 

Il caso in cui $S_n\quad n=2$ questo insieme $S_2=\{1,2\}$ ha invece ha due permutazioni:
il caso in cui non ha cambiato nulla quindi l'identità e il caso in cui i due valori sono stati scambiati
Componendo queste due operazioni otteniamo:
- $id \circ \{2,1\}$
Visto che l'identità si comporta come l'elemento neutro $id \circ \{2,1\}=\{2,1\}$

Nel caso in cui invece $n\geq3$
dobbiamo vedere se:
$\sigma\circ\tau=\tau\circ\sigma$
prendiamo di esempio $\$_3=\{1,2,3\}$
$\sigma(3\ 1\ 2)$
$\tau(1\ 3\ 2)$

$\sigma\circ\tau=(1\ 2\ 3)\rightarrow(1\ 3\ 2)\rightarrow (2\ 1\ 3)$
$\tau \circ\sigma= (1\ 2\ 3)\rightarrow(3\ 1\ 2)\rightarrow(3\ 2\ 1)$

possiamo quindi notare che:
$\sigma\circ\tau=(2\ 1\ 3) \neq \tau\circ\sigma=(3\ 2\ 1)$
