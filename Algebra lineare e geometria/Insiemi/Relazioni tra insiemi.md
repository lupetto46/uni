Le relazioni di insiemi è quello che ci permette di prendere un insieme e mettere i suoi stessi valori in relazione
> [!example] Esempio
> Per esempio nell'insieme degli alunni di una classe quali hanno lo stesso cognome

Questo permette di creare dei sottoinsiemi di un insieme.
Ad esempio avendo un insieme $S=\{a,b,c\}$
*Decido io* quali sono le sue relazioni $R$ (*in questa parte posso deciderle io queste cose*)
per esempio io scelgo $a R b, bRc, aRc, aRa$ e così via a piacimento.

Queste relazioni saranno quindi un sottoinsieme di $S\times S \supset R= \cases{(a,b)(b,c)\\(a,c)(a,a)}$
> [!example] Esempio di relazione
> Un esempio di relazione si trova nell'insieme dei numeri reali: $ℕ=\{0,1,2,3...\}$
> In questo caso la relazione è $\leq$ e lo notiamo $1\leq2\qquad 1\leq3\qquad 1\leq 4$
> In questo caso  è una **relazione d'ordine** che corrisponde al sottoinsieme delle coppie di valori in $ℕ$ $i,j$ tale che $i\leq j$  oppure si può scrivere $\{(i,j)|i\leq\ j\}\supseteq ℕ\times ℕ$


### Relazioni di uguaglianza e d'ordine
Ci sono due tipi di relazioni e una relazione deve soddisfare delle proprietà per essere tale:
- **Relazione d'ordine**: 
	- Riflessiva : $\forall a \in S\qquad aRa$
	- Antisimmetrica : $\forall a,b\in S$ se $aRb \wedge bRa \qquad a=b$
	- Transitiva : $\forall a,b,c\in S$ se $aRb \wedge bRc$ allora $aRc$
- **Relazione equivalente**:
	- Riflessiva :  $\forall a \in S\qquad aRa$
	- Simmetrica : $\forall a,b\in S$ se $aRb$ allora $bRa$
	- Transitiva : $\forall a,b,c \in S$ se $aRb \wedge bRc$ allora $aRc$

> [!example] Esempio
> Per esempio avendo $a,b\in ℤ$ e la relazione è $aRb\ (=)$ se hanno la stessa parità
> Questa è una relazione di equivalenza in quanto è:
> - Riflessiva: $aRa$ il numero $2$ per esempio avrà sempre la stessa parità di se stesso
> - Simmetrica $aRb$ allora $bRa$ se $2R6$ allora $6R2$ indipendentemente dall'ordine sono *entrambi pari*
> - Transitiva: $aRb \wedge bRc$ allora $aRc$ se $2R4$ e $4R6$ allora $2R6$
> 
> Tutto questo conferma quindi che questa è una relazione equivalente
> Ma esattamente *quando due numeri hanno la stessa parità?* quando la loro differenza è divisibile per $2$
> In questo caso si può scrivere in vari modi:
> - $a\equiv b\ mod\ 2$ questo $mod$ sta per *modulo*
> - $2|a-b$


### Congruenza modulo n
Prendiamo di esempio:
$a,b\in ℤ,\qquad n\geq1\qquad aR_nb \Longleftrightarrow n|a-b \Longleftrightarrow a\equiv b\ mod\ n$
### Ma cos'è questo modulo?
#### Classe equivalenti
innanzitutto è utile sapere cos'è una classe equivalente.

Avendo un insieme $S$ e una relazione di equivalenza $R$ su $S\qquad a\subset S$
Quali sono gli altri elementi in relazione con l'unico elemento $a$ di $S$ che abbiamo?
$[a]=\{b\in S|aRb\}\subset S \Rightarrow$ classe equivalente di $a$
Questo significa quindi che si crea un insieme di tutti i valori che sono equivalenti ad $a$

> [!example] esempio
> $ℤ$ con la congruenza modulo $2$
> Quali sono i numeri che divisi per $2$ non danno resto?
> $[0]=\{2n|n\inℤ\}$ 
> > [!attention] Attenzione
> > abbiamo scelto lo zero ($[0]$) come **rappresentante** ma potevamo mettere *qualsiasi numero divisibile per $2$*
> 
> mentre invece l'insieme complementare sarà l'insieme dei numeri non divisibili per 2
> $[1]=\{2n+1|n\inℤ\}$



Ci sono un paio di cose da ricordare di cui anche un **lemma**:
- $[b]\cup[a]=S$ l'unione di tutti gli elementi di $[a]$ risulta tutto l'insieme $S$ se $a\in S$

Il **lemma** è: $a,b\in S\qquad [a]\cap[b]=\cases{\emptyset\ se\ a \not R b\\ [a]=[b]\ se\ aRb}$

> [!note] Dimostrazione
> Se $[a]\cap[b]\neq \emptyset\ \exists c\in S:c\in[b]\Leftrightarrow cRa\wedge cRb$  allora $aRb \Leftarrow$ questo è un assurdo
> Perché se l'intersezione tra le due classi è nulla non esiste nessuna $c\in S$ che è in relazione di equivalenza sia con gli elementi di $a$ che con gli elementi di $b$