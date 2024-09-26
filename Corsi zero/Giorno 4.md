## Gli intervalli
### Illimitati
Ci sono diversi tipi di intervalli
- Non limitati: $\forall x \in ℝ$
- Limitati inferiormente
	- Aperto: $\forall x \in ℝ: x> a: ]a, +\infty[;]a,+\infty)$![[Pasted image 20240925163414.png]]
	- Chiuso: $\forall x \in ℝ: x\geq a: [a, +\infty[;[a,+\infty)$![[Pasted image 20240925163431.png]]
- Limitati superiormente
	- Aperto: $\forall x \in ℝ: x< a: ]-\infty, a[;(-\infty,a[$![[Pasted image 20240925163446.png]]
	- Chiuso: $\forall x \in ℝ: x\leq a: ]-\infty, a];(-\infty,a]$![[Pasted image 20240925163454.png]]

### Limitati
Diamo ovviamente ai due valori ($a,b$) dove si trovano e specifichiamo delle cose:
$a,b \in ℝ$
$a<b$

E questi possono essere di 4 tipi:
- Aperto : $\forall x\in ℝ: a<x<b:]a,b[$![[Pasted image 20240925164015.png]]
- Chiuso : $\forall x\in ℝ: a\leq x \leq b: [a,b]$![[Pasted image 20240925164024.png]]
- Aperto a sinistra chiuso a destra : $\forall x \in ℝ: a<x\leq b; ]a,b]$![[Pasted image 20240925164037.png]]
- Chiuso a sinistra aperto a destra : $\forall x \in ℝ : a \leq x < b: [a,b[$![[Pasted image 20240925164050.png]]

Poi i complementari prendono gli uguali dove l'intervallo non lo ha![[Pasted image 20240925164135.png]]
## Proprietà delle potenze
### Con stessa base
$proddotto\rightleftharpoons somma\ :\ A^a\cdot B^b\cdot C^c=A^{a+b+c}$
$rapporto \rightleftharpoons differenza\ :\ \frac{A^n}{A^m}=A^{n-m}$
$potenza \rightleftharpoons prodotto\ :\ \{[(A^n)^m]^p\}^y=A^{n\cdot m\cdot p\cdot y}$
### Con stesso esponente
$A^n\cdot B^n \cdot C^n=(A\cdot B\cdot C)^n$
$B\neq 0\ allora\ \frac{A^n}{B^n}=(\frac{A}{B})^n$

### A esponente intero o razionale
Avendo $A^\alpha$ con $A\in ℝ\qquad A\neq 0\qquad\alpha\in ℝ$  

Nel caso in cui $\alpha = 0$ allora $A=1$
Nel caso in cui $\alpha\inℕ$ e $\alpha=n$ allora $A^n=\underbrace{A\cdot A\cdot A \cdot...\cdot A}_{n-volte}$
Nel caso in cui $\alpha<0$ allora $A^{-n}=\frac{1}{A^n}$
Nel caso in cui $\alpha=\frac{m}{n}\qquad n\neq0$ allora $A^{\frac{m}{n}=\sqrt[n]{A^m}}$
> [!warning] Attenzione
> È vero che che $\sqrt{(x-1)^2}=(x-1)^{\frac{\cancel{2}}{\cancel{2}}}$
> Ma si deve preservare la qualità di $(x-1)^2$ di essere sempre maggiore di zero. Per fare questo si può utilizzare il valore assoluto di conseguenza si ottiene: $\sqrt{(x-1)^2}=|x-1|$. Vige quindi sempre la regola di rispettare sempre le condizioni di esistenza che nel caso della radice con indice pari è $f(x)\geq0$



## Equazioni e disequazioni esponenziale
Quando un'equazione  è esponenziale?
Quando la $x$ si trova all'esponente: $2^{\sin x}+5^x+3=0$
Queste sono eseguibili a patto che siamo in grado di ricondurle alle forme normali ovvero:
$Sia\ a\inℝ,\qquad a\neq0$
$a^{f(x)}=a^{g(x)}\rightleftharpoons f(x)=g(x)$
Ma abbiamo adesso delle cose molto importanti da dire prima di arrivare al perché le forme normali delle disequazioni:

Presa $y=a^x\qquad a>0\qquad a\neq1$ otteniamo un grafico
![[untitled.jpg]]
Nel caso in cui abbiamo $a>1$ e prendiamo due valori $x_1,x_2$:
![[untitled.jpg]]
Notiamo come in questo caso se $x_1>x_2 \rightleftharpoons a^{x_1} > a^{x_2}$

Nel caso in cui invece $0<a<1$:
![[untitled 1.jpg]]
Notiamo come al contrario quando $x_1<x_2 \rightleftharpoons a^{x_1} > a^{x_2}$

Ottenendo quindi compattato:
Sia $a\in ℝ\quad a>0\qquad a\neq 1$ allora
Se $a>0$:
- $a^{f(x)}\geq a^{g(x)}\rightleftharpoons f(x)\geq g(x)$
- $a^{f(x)}\leq a^{g(x)}\rightleftharpoons f(x)\leq g(x)$

Se $0<a<1$:
- $a^{f(x)}\geq a^{g(x)}\rightleftharpoons f(x)\leq g(x)$
- $a^{f(x)}\leq a^{g(x)}\rightleftharpoons f(x)\geq g(x)$

## logaritmi
### Definizione formale
Sia $a,b\in ℝ:b>0,\qquad a>0,\qquad a\neq 1$
Sia $c \in ℝ:a^c=b$ allora diciamo che $c=log_ab$

In relazione a ciò si può dire $a^c=b\rightleftharpoons c=log_ab$

Quindi per esempio se abbiamo:
$3^x=7$
$x = log_3 7$
$3^{log_3 7}=7$

## Proprietà dei logaritmi
Siano $A,B,a\inℝ:A>0,B>0,a>0,a\neq1$
$log_aA+log_aB=log_a(A\cdot B)$
$log_aA-log_aB=log_a(\frac{A}{B})$ 
$\alpha log_aA=log_aA^\alpha\qquad,\qquad \alpha\inℝ$

## Come lo calcolo il logaritmo
Qui possiamo usare la formula del cambio base:
$log_ab=\frac{log_\alpha b}{log_\alpha a}$ di cui $\alpha>0,\alpha\neq1$

Riguardante il grafico
![[Pasted image 20240926191412.png]]
Notiamo che siano $x_1,x_2 \in ℝ$ con $0<x_1<x_2$:
- Se $a>0$ $log_ax_1 < log_ax_2$
- Se $0<a<1$ $log_ax_1 > log_ax_2$ 

## Equazioni logaritmiche
Le equazioni logaritmiche hanno come forma normale:
$log_af(x)=log_ag(x)$
Dove $a>0\qquad a\neq1$
Avendo definito le condizioni di esistenza otteniamo quindi
$\cases{Insieme\ di\ esistenza\\ f(x)=g(x)}$

Ci sono un altro tipo di equazioni logaritmiche:
$log_{a(x)}f(x)=log_{a(x)}g(x)$
In quel caso si devono specificare le condizioni di esistenza degli argomenti
$\cases{C.E.argomenti\\ a(x)>0\ \land\ a(x)\neq1\\ f(x)= g(x)}$

## Disequazioni logaritmiche
Le disequazioni logaritmiche sono di due tipi:
1. $log_af(x)\geq log_ag(x)$
	 Dobbiamo vedere il caso in cui $a>1$ che mi fa ottenere:
	 $\cases{Insieme\ di\ esistenza\\ f(x)\geq g(x)}$
	 E il caso in cui $0<a<1$ che ci fa ottenere:
	 $\cases{I.E.\\ f(x)\leq g(x)}$
2. $log_af(x)\leq log_ag(x)$
   Esattamente come prima dobbiamo vedere se $a>1$ che ci fa ottenere:
   $\cases{I.E.\\ f(x)\leq g(x)}$
   e il caso in cui $0<a<1$ che ci fa ottenere:
   $\cases{Insieme\ di\ esistenza\\ f(x)\geq g(x)}$

Il caso in cui la nostra disequazione è:
$log_{a(x)}f(x)\geq log_{a(x)}g(x)$ 
È più complicato. In questo caso si ottengono due sistemi
$$
\begin{align}
&log_{a(x)}f(x)\geq log_{a(x)}g(x)\\\\
&1)\begin{cases}
I.E. Argomenti\\
a(x)>1\\
f(x)\leq g(x)
\end{cases} \rightarrow Soluzione_1\\\\
&2)\begin{cases}
I.E. Argomenti\\
0<a(x)<1\implies\cases{a(x)>0\\ a(x)<1}\\
f(x)\geq g(x)
\end{cases} \rightarrow Soluzione_2
\end{align}
$$
E poi la soluzione sarà:
$Soluzione = Soluzione_1\cup Soluzione_2$

Nel caso in cui la disequazione sia $log_{a(x)}f(x)\leq log_{a(x)}g(x)$ è la stessa cosa ma il segno della disequazione alle fine dei sistemi è invertito
