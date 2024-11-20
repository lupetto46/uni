Per quanto riguarda l'uguaglianza di un sistema dipende tutto da quello che guardo.
Si dice *a meno* di similitudini.

Per esempio per me una persona è identica all'altra *a meno* di cognome (ovvero per me due persone se hanno lo stesso cognome sono la stessa persona)

Sotto forma di insiemi se abbiamo l'insieme $S$ e una relazione $R$ su $S$ di equivalenza
$\frac{S}{R}=\{[a]\ |a\in S\}\Rightarrow$ tutte le classi di equivalenza

> [!example] Esempio
> $ℤ;\equiv mod\ 2$
> normalmente si scrive così: $\frac{ℤ}{\equiv mod\ 2}=:\frac{ℤ}{ℤ\equiv mod\ 2}=\{[0], [1]\}=\{\overline{0},\overline{1}\}$
> 
> In questo caso il motivo di questo risultato è $\{[0],[1]\}$ perché tutte le classi di equivalenza che può avere questo quoziente è il caso in cui il numero è pari e il caso in cui il numero è dispari che noi contrassegniamo con $[0]$ tutti i casi in cui il numero è pari e $[1]$ il caso in cui il numero è dispari


In realtà il modulo non è altro che una *funzione* che **ritorna** il *resto di una divisione*

> [!example] Esempio
> $\frac{5}{2}$ fa $2$ con resto $1$ di conseguenza $5\ mod\ 2= 1$

Tra le classi di equivalenze della differenza tra insieme e relazione ci saranno tutti i valori che danno il resto da $0$ a $n-1$ di cui $n$ è il numero per cui si sta facendo il modulo

$\frac{ℤ}{3ℤ}=\frac{ℤ}{ℤ\equiv mod\ 3}=3|a-b|$
ci sono:
- Tutti i numeri che divisi per 3 danno come resto : $[0]=\{3,6,9,12 ...\}$
- Tutti i numeri che divisi per 3 danno come resto : $[1] =\{4,7,10,13 ...\}$
- Tutti i numeri che divisi per 3 danno come resto : $[2]=\{5,8,11,14 ...\}$
- Non possono esserci numeri che danno resto più di $2$ ovviamente

Quindi il risultato di $\frac{ℤ}{3ℤ}=\{\overline{0}, \overline{1}, \overline{2}\}$

Si giunge quindi alla conclusione che $\frac{ℤ}{\equiv mod\ n}=:\frac{ℤ}{nℤ}=\{\overline{0}, \overline{1}, \overline{2}...\overline{n-1}\}$