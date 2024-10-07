

Sono entrato dopo quindi farmi dare gli appunti

### Prodotto cartesiano
$A=\{a,b,c\}\qquad B=\{1,2,3\}$

$A\times B= \cases{(a,1)(b,1)(c,1)\\(a,2)(b,2)(c,2)\\(a,3)(b,3)(c,3)}$
In questo caso è importante ricordare che gli elementi di $A$ devono essere nella *prima posizione*.
Nel caso in cui fosse stato $B\times A$ il risultato sarebbe stato $\cases{(1,a)(2,a)(3,a)\\(1,b)(2,b)(3,b)\\(1,c)(2,c)(3,c)}$

### La cardinalità
Ci sono inoltre due segni per rappresentare la *cardinalità* di un insieme
$\#A$ oppure $|A|$
La cardinalità non è altro che il *numero di elementi* all'interno di un insieme

In questo caso riprendendo i due insiemi di prima:
$A=\{a,b,c\}\qquad B=\{1,2,3\}$
$|A|=3\qquad |B|=3$
Allora  $|A\times B|= |A|\cdot|B|=9$

Ci sono diverse operazioni che si possono fare tra due insiemi:
- Unione:
	- $A\cup B=\{c|c\in A \vee c\in B |\}$ Si crea un nuovo insieme composto da elementi che appartengono o ad $A$ o a $B$
- Intersezione:
	- $A\cap B = \{c|c\in A \wedge c\in B|\}$ Si crea un nuovo insieme composto da elementi che devono appartenere sia ad $A$ che a $B$ contemporaneamente
- Differenza:
	- $A \backslash B= \{c|c\in A\wedge c\notin B|\}$ Si crea un insieme composto da elementi che appartengono ad $A$ ma non appartengono a $B$

## Le relazioni tra elementi di insiemi
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


## Quoziente
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

## Insiemi con operazioni
$S\neq\emptyset$ un operazione su $S$ è una funzione:
$*:S * S\longrightarrow S$
$(a,b)\longmapsto a*b$

La stella ($*$) indica un'*operazione generica*
> [!example] Esempio
> $+:ℕ*ℕ\longrightarrow ℕ$
> $(a,b)\longmapsto a+b$


### Proprietà delle operazioni
- Un operazione ***può*** essere associativa:
	- $\forall a,b,c\in S\qquad (a*b)*c=(b*c)*a=(c*a)*b$
- Un operazione ***può*** essere commutativa:
	- $\forall a,b,c\in S\qquad a*b=b*a$
- ***Può*** esistere un elemento $e_1$ : $\exists e_1\in S:\forall a \in S\quad e_1 * a= a$ chiamato elemento neutro sinistro
- ***Può*** esistere un elemento $e_2$ : $\exists e_2\in S:\forall a \in S\quad a*e_1= a$ chiamato elemento neutro destro
- ***Può*** esistere un elemento $e$ : $\exists e\in S:\forall a \in S\quad a*e=e*a=a$

**Lemma**: Un insieme $S$ con operazione $*$ : $(S,*)$ ammette un solo elemento neutro sinistro $e_1$, e solo un elemento neutro destro $e_2\qquad e_1=e_2$ 

> [!note] Dimostrazione
> $e_1=e_1*e_2=e_2$ in quanto $e_1=e_1*e_2$ perché $e_2$ è l'elemento neutro a destra
> $H_p$
> Avendo $(S,*)$ quanti elementi neutri ci sono?
> Supponiamo per assurdo che ci siano sia l'elemento neutro $e$ che e l'elemento neutro $e_1$:
> $e*e_1=e$
> Ma allo stesso tempo
> $e*e_1=e_1$
> Il che implica che: $e=e_1$ confermando che ce n'è solo uno 


## Definizioni

$(S, *)$ è detta struttura algebrica 
- Se $*$ è associativa, $(S, *)$ è chiamato semigruppo
- Se un semigruppo $(S, *)$ ammette un elemento neutro è chiamato monoide
- Un semigruppo / monoide $(S,*)$ si dice **commutativo** o **abeliano** se l'operazione è commutativa
- Avendo un monoide $(S, *): a\in S$ diciamo che questo elemento è invertibile se $\exists b\in S: b*a=e=a*b$ in tal caso $b$ si dice l'inverso di $a$
- Un monoide di cui ogni elemento è invertibile è chiamato gruppo 

Per esempio sono gruppi:
$(ℤ,+,0),(ℚ\backslash\{0\},\cdot,1)$
$(ℚ, +, 0), (ℝ\backslash\{0\},\cdot, 1)$
$(ℝ, +, 0)$

È un gruppo anche:
$(\frac{ℤ}{2ℤ},+, \overline{0})$

perché
- L'invertibile di $\overline{0}$ è $\overline{0}$ in quanto = $\overline{0}+\overline{0}=\overline{0}$
- E l'invertibile di $\overline{1}$ è $\overline{1}$ in quanto $\overline{1}+\overline{1}=\overline{2}$ che visto che stiamo parlando di $n\ mod\ 2$ scrivere $\overline{2}$ è la stessa cosa di scrivere $\overline{0}$

Questo si può fare anche con la moltiplicazione:
$(\frac{ℤ}{3ℤ},\cdotp,\overline{1})$

$\overline{0}\cdot\overline{0}=\overline{0}$
$\overline{0}\cdot\overline{1}=\overline{0}$
$\overline{1}\cdot\overline{0}=\overline{0}$
$\overline{1}\cdot\overline{1}=\overline{1}$
$\overline{1}\cdot\overline{2}= \overline{2}$
$\overline{2}\cdot\overline{1}= \overline{2}$
$\overline{2}\cdot\overline{2}= \overline{0}$
$\overline{1}\cdot\overline{2}= \overline{2}$
$\overline{2}\cdot\overline{2}= \overline{4} = \overline{1}$

Tuttavia $(\frac{ℤ}{4ℤ}\backslash\{0\}, \cdotp, \overline{1})$ non è un gruppo in quanto:
- L'inverso di $\overline{2}$ sarebbe $\overline{2}$ ma non è fattibile in quanto $\overline{4}=\overline{0}$ che nell'insieme che in questo caso è $\frac{ℤ}{4ℤ}\backslash\{0\}=\{\overline{1},\overline{2}, \overline{3}\}$ non esiste

Questo implica quindi che negli insiemi con modulo e come operazione la moltiplicazione è un *gruppo solo se il numero del modulo è un numero primo* ad esempio:
$(\frac{ℤ}{Pℤ},\cdotp,\overline{1}) =>$ in cui $P$ è un numero primo


|            | Addizione | Moltiplica | Generale |
| ---------- | --------- | ---------- | -------- |
| Operazione | $+$       | $\cdot$    | $*$      |
| Inverso    | $-a$      | $a^{-1}$   | $a^{-1}$ |
| Neutro     | $0$       | $1$        | $e$      |

## Gli insieme con più operazioni
### Definizione di anello
Per essere un anello è un insieme non vuoto con due operazione $+$ e $\cdot$ devono essere:
1) $(S,+)$ sia un gruppo abeliano con elemento neutro $0$
2) $(S,\cdotp)$ un semigruppo
3) $\forall a,b,c\in S,\quad a\cdot(b+c)=a\cdot b+a\cdot b,a\cdot(b+c)=a\cdot b+a\cdot c$
4) Se la moltiplicazione è commutativo l'anello si chiama commutativo
5) Se la moltiplicazione ammette un elemento neutro $1$ l'anello si dice unitario
6) $(S,+,\cdotp,0)$ è un anello. Siano $a,b\in S: a\cdot b=0$ oppure $b\cdot a= 0$ allora $a$ e $b$ si dicono **divisori dello zero**
7) Se $(S, +, \cdotp, 0)$ non ha divisioni dello zero si dice un dominio di integrità
8) Se $(S\backslash\{0\}, \cdotp)$ è un gruppo abeliano con elemento neutro $1\neq 0$ allora $(S, +, \cdotp,0,1)$ si dice **un campo**

