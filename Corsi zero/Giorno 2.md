## La scrittura in generale di un polinomio
Un polinomio è uguale a:
$P(x)=a_nx^n+a_{n-1}x^{n-1}+a_{n-2}x^{n-2}+...+a_{2}x^{2}+
a_{1}x^{1}+a_{0}$

In questo caso per poterlo scrivere in modo compatto si può scrivere
$P(x)=\sum^{n}_{i=0}a_ix^i$

## Lo studio del segno

Il polinomio lo posso anche scrivere come prodotto i cui termini sono vari polinomi:
$P(x)= (x-1)(x-\frac{1}{2})^2(x+5)(7-x)^2(x^2+x+1)(x^2+x+3)^2$

Questa tipologia di scrittura si chiama **fattorizzazione**

E ci permette di semplificare e fare molte cose:
Per esempio come posso sapere il grado del polinomio?
$x-1$ ammette $1$ zeri
$(x-\frac{1}{2})^2$ ammette $2$ zeri
$x+5$ ammette $1$ zero
$(7-x)^2$ ammette $2$ zeri
Gli altri due hanno $\Delta < 0$ ma stiamo comunque lavorando nel campo dei numeri reali se dobbiamo solo capirne il numero di zeri
$x^2+x+1$ ammette $2$ zeri
$(x^2+x+3)^2$ ammette $4$ zeri

Quindi il polinomio da cui solo risultati tutti questi polinomi è di grado
$1+2+1+2+2+4=12$

## Divisioni tra Polinomi
Come prima cosa è importante sapere lo studio del segno come funziona

Innanzitutto prendere il nostro polinomio fattorizzato e studiare singolarmente il segno dei singoli termini

Esempio.
$P(x)=(x-1)(x-\frac{1}{2})^2(x+5)(7-x)^2$

$$
\begin{align}
x-1\qquad x-1\geq 0\qquad x\geq1\\
(x-\frac{1}{2})^2\qquad (x-\frac{1}{2})^2\geq0\qquad x\geq\frac{1}{2}\\
x+5\qquad x+5\geq0\qquad x\geq-5\\
(7-x)^2\qquad (7-x)^2\geq0\qquad \forall x \in ℝ
\end{align}
$$

![[Pasted image 20240924090744.png]]

### Cosa si intende dire per maggiore di 0?
Considerando che un polinomio può essere una retta in quanto l'equazione della retta è

$a,b,c \in ℝ\qquad ax+by+c=0$ questa equazione racchiude al cambiare di $a$ e $b$ TUTTE le rette
Ma questa forma della retta si chiama **forma implicita** che non ha molto valore a causa della presenza di **due variabili *indipendenti*** 

Per ovviare a questo problema dobbiamo trovare il modo di rendere una delle due variabili **dipendenti** e quindi si ottiene
$$
\begin{flalign}
by&=-ax-c\\
y&=-\frac{ax}{b}-\frac{c}{b}
\end{flalign}
$$
Si ottiene quindi l'equazione di tutte le rette tranne quelle in cui non esiste $y$
è quindi importante porre $b\neq 0$

Per semplicità si scrive quindi che
$$
\begin{flalign}
m&=-\frac{a}{b}\\
q&=-\frac{c}{b}\\
y&=mx+q
\end{flalign}
$$
Di cui 
- $m$ è il coefficiente angolare 
- $q$ è l'ordinata all'origine

Qualche altro dettaglio da dire su $m$ è:
![[Pasted image 20240924092430.png]]
$m$ sarebbe la tangente dell'angolo $(\alpha)$ che fa la retta con l'asse delle ascisse 

Quindi quando si pone un polinomio > 0 si sta cercando il momento in cui la retta o il grafico va nei quadranti in basso

## Disequazioni razionali fratte
È importante ricordare che quando si scrive una disequazione razionale fratta bisogna specificarne le condizioni di esistenza
Quindi:
$$
\frac{N(x)}{D(x)}=\frac{3x^3+2x^2-x+2}{4x^5+6x^2-\frac{7}{2}x+\frac{1}{2}}
$$
La cui condizione di esistenza è: $\forall x \in ℝ:4x^5+6x^2-\frac{7}{2}x+\frac{1}{2}\neq0$

Ma conviene dividere per gradi più bassi e per farlo si può usare la regola di Ruffini la cui unica esigenza é quella di avere gli eventuali zeri **razionali**

Lo scopo è quindi diminuire il grado dei polinomi al più basso possibile mantenendo il $\Delta$ maggiore di 0

L'esempio é quindi:
$$
\frac{(x-1)(5-x)(x^2-x+2)(x+3)}{(x+3)(\frac{1}{2}-x)(x^2+x-2)} \geq 0
$$

In questo caso si potrebbero semplificare i due $(x+3)$ ma é necessario evitare l'annullamento del valore che stiamo semplificando
$$
\begin{cases}
\frac{(x-1)(5-x)(x^2-x+2)\cancel{(x+3)}}{\cancel{(x+3)}(\frac{1}{2}-x)(x^2+x-2)}\geq 0\\
x\neq-3
\end{cases}
$$

Quindi per studiare il segno della disequazione bisogna considerare quando tutti i polinomi che lo compongono sono maggiori o uguali a zero:
$$
\begin{flalign}
&x-1\qquad x-1\geq0\qquad &x\geq 1\\
&5-x\qquad 5-x\geq 0 \qquad &x\leq5\\
&x^2-x+2\qquad x^2-x+2 > 0 \qquad \Delta = 1-4\cdot2 = -7 &\forall x\in ℝ
\end{flalign}
$$

L'ultima è particolare:
$x^2+x-2$ ha il $\Delta = 9$ allora si possono dividere due strade:
1. Scompongo il polinomio e ottengo $(x+1)(x-2)$
2. Risolvo la disequazione e ottengo $x< -2 \cup x>1$

In ogni caso va bene poi nella parte finale

#### Ma come si esegue il primo caso?
Per poter eseguire il primo caso è necessario considerare la regola che:
$se\ ax^2+bx+c\ ha\ \Delta>0\ allora\ può\ dar \exists x_1,x_2$