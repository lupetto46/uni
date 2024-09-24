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

Quindi quando si pone un 