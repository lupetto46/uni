# Tecniche dimostrative
Ci sono diversi modi per dimostrare un concetto matematico:
- Deduttivo
- Per assurdo
- Induttivo

## Induttivo
Viene utilizzata quando bisogna dimostrare la validità di un enunciato in funzione dei numeri naturali

> [!cite] "Dimostrare che per $\forall n\in ℕ$ vale qualcosa"

Come funziona:
1. Intanto dimostrare che l'enunciato vale per $n=0$
2. Poi supponendo che $P(n)$ sia vera si deve controllare se è vera anche con $P(n+1)$

Quindi se $P(n) \Longrightarrow P(n+1)$

### Esempio
Vogliamo dimostrare che per ogni $n\geq 1 \in ℕ$ la somma dei primi $n$ numeri naturali $S(n)$ è uguale a:
$$
S(n) = \frac{n(n+1)}{2}\ \forall n\geq 1
$$

Quindi seguiamo i passaggi:
1. Verifichiamo se è vera per $n=1$
   $$
   S(1)=\frac{1(1+1)}{2}= \frac{2}{2}=1
   $$
2. Si *suppone* che sia vera per $S(n)$
   $$
   S(n)=\frac{n(n+1)}{2}
   $$
3. Si dimostra che sia vera per $S(n+1)$
   $$
   S(n+1)=\frac{(n+1)((n+1)+1)}{2}=\frac{(n+1)(n+2)}{2}=\frac{n^2+3n+2}{2}
   $$

	Visto che $S(n)$ è la somma dei primi $n$ numeri naturali $S(n+1)$ è la somma dei primi $n+1$ numeri naturali ed è quindi scrivibile come:
	$$
	S(n+1)=\overbrace{1+2+3+4+...+n}^{S(n)} + (n+1)
	$$
	Allora si può anche scrivere che $S(n+1)=S(n)+n+1$ dando questa come ipotesi induttiva
	Quindi proviamo a  scriverla così vedendo se raggiungiamo lo stesso risultato di prima ($\frac{n^2+3n+2}{2}$)
	quindi 
	$$
	\begin{align}
	S(n+1)&=\frac{n(n+1)}{2}+(n+1)=\\
	&= \frac{n(n+1)+2(n+1)}{2}=\\
	&= \frac{n^2+3n+2}{2}
	\end{align}
	$$
	Confermando che la formula è vera per $\forall n\geq 1$

### Disuguaglianza di Bernoulli
Dimostrare che 
$\forall n\in ℕ\ e\ h>-1, h\inℝ$
$(1+h)^n\geq 1+nh$

1. Supponiamo che valga per $n=1$
   $1+h\geq 1+h$ vale vera l'uguaglianza
2. Supponiamo sia vera per n
   $(1+h)^n\geq 1+nh$
3. Supponiamo che sia uguale per $n+1$
   *$(1+h)^{n+1}\geq 1+h(n+1)$*
   Ora utilizziamo le proprietà delle potenze al primo membro per scrivere:
   $(1+h)(1+h)^n\geq$
   Per quanto riguardai l secondo membro guardiamo invece dobbiamo ragionare con il fatto che $(1+n)^h$ è $\geq 1+nh$
   Quindi: $(1+h)(1+h)^n\geq (1+nh)(1+h)$
   Questo perché sappiamo che $h > -1$ quindi il polinomio $(1+h)$ è sicuramente positivo quindi si può moltiplicare questo valore per entrambi i membri
   Questo ci riporta alla proprietà $P(n)=(1+n)^h\geq 1+nh$ ma dopo aver moltiplicato tutti e due i membri per $(1+h)$
   
   Quindi cerchiamo di capire come raggiungere la proprietà tramite quello che abbiamo adesso:
   $(1+h)(1+h)^n\geq (1+nh)(1+h)$
   Ma ora concentriamoci nel secondo membro
   Eseguiamo la moltiplicazione tra polinomi al secondo membro
   $1+h+nh+nh^2$
   Ma se raccogliamo la $h$ solo nella parte $h+nh$ otteniamo
   $1+ (1+n)h+nh^2$
   riordinando otteniamo:
   *$h(n+1)+ 1$* $+nh^2$
   
   Quindi il secondo membro non è altro che $h(n+1)+ 1$ della proprietà originale ma aggiungendo $nh^2$
   
   Possiamo quindi dire sicuramente che questo ultimo membro è:
   $h(n+1)+ 1+nh^2\geq h(n+1) + 1$ 
   Questo perché se si toglie il valore sicuramente positivo $nh^2$ il risultato che verrà sarà sicuramente più piccolo quindi matematicamente è come dire $7+3\geq 7$
   
   Otteniamo quindi quindi la disuguaglianza iniziale:
   ***$(1+h)^{n+1}\geq h(n+1)+1$***

