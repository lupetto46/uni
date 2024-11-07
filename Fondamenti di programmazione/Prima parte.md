#fondamenti_di_programmazione
# Elaborazione dell'informazione
## Definire un problema
Ci sono definizioni particolari per poter dire che un problema è ben formulato:
- Non è evidente che non esistano soluzioni
- Il criterio di verifica delle soluzioni è univoco
- L'insieme dei dati iniziali è incompleto

Una soluzione si definisce effettiva invece quando:
- L'esecutore è in grado di interpretare i dati in ingresso.
  è importante capire che un dato debba essere leggibile in qualche modo dal computer e poi deve poter essere *rappresentabile* (per esempio i numeri reali) 
- L'esecutore deve essere in grado di risolvere il problema attraverso una serie di azioni da eseguire per essere in grado di eseguirla
- L'esecutore deve essere in grado di risolvere questo e soprattutto, *importantissimo*, deve essere in grado di completarlo in un **tempo finito**. (È importante che non ci siano azioni all'interno del nostro codice o programma che continuano all'infinito senza **condizione di fine**)

## Algoritmo
L'algoritmo per poter essere chiamato tale ed essere un *buon algoritmo* deve avere delle proprietà particolari:
- Non ambiguità:
  Ogni azione elementare deve essere ben definita e deve essere in grado di dare risultati per tutti i valori che potranno andargli in ingresso
- Eseguibilità:
	- Ogni azione deve essere eseguita in un tempo finito. Quindi un'azione non può andare all'infinito
- Determinismo:
	- Il programma deve essere sequenziale. Quindi un'azione ha un solo passo successivo
- Finitezza:
	- L'algoritmo deve finire arrivato ad un certo punto. (Sempre importante che il programma non vada avanti all'infinito senza una condizione di fine.)
- Terminazione:
	- Come già detto il programma prima o poi deve terminare.

### Esempio
#### Calcolare il massimo tra due numeri
Il programmatore quando ha un problema semplice come quello di calcolare il massimo tra due numeri deve prima di tutto spezzettare il problema.

Per esempio il primo passaggio sarebbe:
leggere i due numeri e inserirli da qualche parte come prima cosa.
Poi il secondo passaggio sarebbe porsi la domanda: 
"il primo numero è più grande di del secondo?"
Nel caso in cui il primo numero è più grande allora quello sarà il massimo
Al contrario lo sarebbe l'altro

Scritto in pseudo codice verrebbe:
```Pseudo-codice
Leggi un numero intero e mettilo in A
Leggi un numero intero e mettilo in B
Se A > B:
	Stampa "A è il massimo"
Altrimenti:
	Stampa "B è il massimo"
```

### Quando due algoritmi sono equivalenti
Due algoritmi sono considerati equivalenti quando i loro dati in input (*dominio di entrata*) e i loro dati in output (*dominio di uscita*) sono uguali e con gli stessi dati in input danno lo stesso output.

In poche parole quando fanno la stessa identica cosa

### La complessità computazionale
La complessità computazionale cerca di ottenere delle metriche indipendenti dal calcolatore in cui un algoritmo viene eseguito

Ci sono due metriche:
- Numero di istruzioni per eseguire una riga di comando
- Spazio in memoria necessario per risolverlo

Sfortunatamente la storia ci ha fatto scoprire che è impossibile ottimizzare sia il numero di istruzioni che lo spazio

È quindi necessario capire in che contesto sto creando l'algoritmo

> [!example] esempio
> Un profilo utente chiederebbe minimo 100 byte tra nome cognome data di nascita codice fiscale ecc..
> Per 100 alunni sarebbe 10 Kb che se siamo a corto di memoria non va bene ma se la memoria non fosse un nostro problema allora va anche bene
## Processo di soluzione
Per creare un algoritmo di soluzione di un problema si devono seguire degli step:
1. Analizzare il problema e trovarne una soluzione. (Se devo risolvere questo allora devo fare questo)
2. Formalizzare il problema e definire un algoritmo risolutivo:
   Questo passaggio consiste nel *spezzettare* la soluzione che abbiamo trovato nel primo step in tanti piccoli *passi elementali*
3. Scrittura di un programma nel linguaggio di programmazione:
   I passaggi che devono essere scritti nel secondo passo devono essere come uno pseudo codice.
   > [!info] Esempio
   > ```Pseudo codice
   > Istruzione 1: Prendo un numero intero e lo salvo da qualche parte
   > Istruzione 2: Prendo quel valore lo sommo a un altro valore e lo salvo da qualche altra parte
   > Istruzione 3: Stampo la somma che ho appena salvato
   > ```
   > Tutti questi passaggi elementali hanno una traduzione in linguaggio di programmazione
   > Un esempio in python:
   > ```python
   > A=int(input("Inserire un numero: "))#Prendo un intero e lo salvo in A
   > B = A+3 # Prendo il valore in A gli sommo 3 e lo salvo in B
   > print(B) # Stampo B
   > ```
   
1. Traduzione del programma dal linguaggio di programmazione a un linguaggio compreso dalla macchina:
   Questo è normalmente uno step che fa in automatico il compilatore. è il passaggio in cui il *file sorgente* viene trasformato nel file .exe di windows 
2. Esecuzione del programma

## Definire l'informazione
Informazione indica il concetto di dare forma, descrivere un concetto astratto.
È in poche parole la pratica in cui si trova un modo per rappresentare un qualcosa di reale.

In informatica o meglio nell'ambito dei calcolatori l'esempio più banale è i numeri interi con il sistema binario.

Anche se tra le tecniche di rappresentazione oltre a quella binaria ci sta anche quella analogica.

> [!faq] Cos'è l'analogico e il digitale?
> Il sistema analogico consiste nel rappresentare informazione attraverso l'utilizzo di tutti i numeri (dal $-\infty$ al $+\infty$) mentre invece il digitale consiste nel rappresentare l'informazione attraverso una serie di zero e uno.

Lo scopo dell'informazione è quello di rappresentare i dati in un modo utile e significativo per scopi pratici.

### Rappresentare l'informazione
La rappresentazione dell'informazione non è altro che prendere un simbolo o un valore e trovare un modo per far si che questo simbolo rappresenti univocamente un oggetto reale.
Nell'immagine si fa l'esempio della parola "gatto" che rappresenta il gatto reale.
![[Pasted image 20241017174503.png]]

Come detto quindi non si devono presentare ambiguità. Quindi simboli che significano due cose contemporaneamente.

Il processo di trasformazione di un concetto in un simbolo si chiama codificazione
E il simbolo utilizzato per rappresentare un informazione può essere di qualsiasi tipo.
> [!info] Esempio
> Si può fare l'esempio di una tensione elettrica alta o bassa {Vhigh (alta), Vlow (bassa)}

### Ma come si applica in un algoritmo
Ci interessa quindi rappresentare i dati che vengono inseriti come input 
Possiamo considerare come valori numerici se sta piovendo o meno:
1 = sta piovendo
0 = non sta piovendo

Oppure voglio trovare un modo per rappresentare i  valori numerici come i numeri interi razionali o naturali.

Ci può interessare anche rappresentare valori non numerici ad esempio le immagini il testo o i caratteri

## Le unità che utilizza il computer
### Il bit
Il computer usa una unità più piccola che sarebbe il bit o "binary digit" ed è la più piccola quantità di dati che il computer è in grado di rappresentare.

### Il byte
Ma per poter essere utili questi vengono messi assieme creando quindi il byte ovvero l'unione di 8 bit. 
Così facendo siamo passati dai soli due stati che posso ottenere (acceso o spento) dal singolo bit ai $2^8$ stati che sono ottenibili con 8 bit messi assieme.
Quindi il numero di stati rappresentabili utilizzando il sistema binario è uguale a $2^{n-bit}$ che nel caso di un byte è 256 stati

## GigaByte e GiBiByte
### Gigabyte
Il gigabyte l'unità di misura rappresentate in multipli di $10$. 
Un gigabyte è uguale a un 1000 megabyte

### GiBibyte
Essendo il calcolatore basato su un architettura binaria non funziona a multipli di $10$ ma multipli di due
In fatti un Gibibyte equivale a 1024 Mebibyte (MiB)

# Sistemi di numerazione
## Rappresentazione polinomiale
La rappresentazione polinomiale di una serie di bit è vista come la somma tra tutte le cifre della seria di bit moltiplicate dalla loro posizione a partire dallo 0 (*il bit più a destra*) fino ad arrivare a n-1 (*Il bit più a sinistra*)
- In generale della B la base e $c_i$ i coefficienti
$$
N=\sum^{n}_{i=0} c_i\cdot b^i
$$

## Conversione di base

### Da base 2 a base 10
Utilizziamo proprio la somma vista sopra per convertire da base
$0111_{(2)}= 0\cdot 2^3 + 1\cdot 2^2+ 1\cdot 2^1+1\cdot 2^0=7_{(10)}$
Non è altro che prendere il bit da destra verso sinistra e moltiplicarlo per la posizione del bit a partire da 0 fino a $(n-bit)-1$
### Da base 10 a base 2
Da base 10 a binario invece è diverso
È necessario prendere il valore dividerlo per la base e scrivere solo il resto che si ottiene dalla divisione:
$\frac{19}{2}$ fa $9$ con resto $1$
$\frac{9}{2}$ fa $4$ con resto $1$
$\frac{4}{2}$ fa $2$ con resto $0$
$\frac{2}{2}$ fa $1$ con resto $0$
$\frac{1}{2}$ fa $0$ con resto $1$

Si legge poi dal basso verso l'altro ottenendo che $17_{(10)}= 10011_{(2)}$
### Modulo e segno
Per rappresentare un numero con il segno si prende innanzitutto il bit più a sinistra tra i bit disponibili.
> [!question] Perché il bit più a sinistra
> È una convenzione

E si utilizza come segno

*$1$*$0000000$ Questo numero è negativo
*$0$*$0000000$ Questo numero è invece positivo

ottenendo quindi che l'intervallo
$n\in [-(2^{k-1} - 1), 2^{k-1} - 1]$ in cui $k$ è il numero di bit disponibili

Il problema è che questo metodo ha 2 modi per rappresentare lo zero:
- $10000000$
- $00000000$

### Le operazioni
Prima di andare avanti è importante considerare i risultati che possono dare le varie operazioni.
- Overflow
	- Quando il numero che sta risultando dall'operazione è troppo grande per essere rappresentato con il numero di bit disponibili. Se si verifica questo caso lo si può sapere attraverso un bit chiamato **bit di carry**, ovvero un bit aggiuntivo che si attiva solo nel caso in cui si sommano i due bit più significativi. ^f264c5
- Underflow:
	- Il caso in cui il valore che si sta cercando di rappresentare è troppo piccolo per essere rappresentato con il numero di bit che ho in questo momento

Ma la domanda è: **Come posso rappresentare i numeri negativi avendo solo un  rappresentazione dello zero?**

Per evitare questo problema delle due rappresentazioni dello zero si possono rappresentare i numeri come:
$127-n$
Quindi se voglio il numero 3 posso rappresentarlo come:
$127 - 124 = 3$
così facendo ho una sola rappresentazione dello $0$ che sarebbe $127-127$

## Complemento a 2
Per trasformare un numero da numero positivo a numero negativo ci sono vari metodi in binario uno di questi è:

Il primo passaggio consiste nel prendere il numero che si vuole rendere negativo e invertire i bit di cui è composto
$3=0011$
$\overline{3}=1100$
Dopodiché al numero *negato bit per bit* si somma $1$
$\overline{3}+1=1100+0001=1101$
(*Da specificare che quest'ultima è una vera e propria somma tra numeri binari e quindi non si deve semplicemente mettere 1 alla fine se non c'è ma si deve sommare 1*)
### Operazioni con complemento a 2
Ma come eseguire le operazioni (in particolare la sottrazione) con i bit?

Ci sono due modi:
#### Calcolo con segno:
Si guarda quale dei due numeri (senza segno) è più grande, poi si sommano i due numeri e si mette il segno del numero più grande

Questo metodo non viene utilizzato molto in quando richiedere troppi passaggi e se n'è trovato un altro più semplice 
#### Calcolo con complemento a 2:
Come prima cosa si calcola il complemento a 2 prendendo il numero negativo della sottrazione e si calcola il complemento a due.

Una volta calcolato il complemento a 2 si sommano i due numeri scegliendo il segno attraverso [[#^f264c5|bit di carry]] che se sarà attivo darà segno positivo altrimenti il segno sarà negativo.

## Le flag
Una volta completata un'operazione il calcolatore utilizza delle flag particolari che sono semplicemente bit in una posizione specificata precedentemente.
Le flag in particolare sono 3:
1. OF (Overflow Flag). Verrà impostata 1 se l'operazione non è valida a causa del fatto che una somma tra due numeri attiva il bit di carry
2. SF (Sign Flag). Verrà impostata 1 se l'operazione ha segno positivo 0 altrimenti in questo caso prende l'informazione dal bit più significativo (il più a sinistra) del risultato
3. ZF (Zero Flag). Se il risultato che è stato dato è zero

## Problemi riguardanti le proprietà delle operazioni
Le *operazioni con numeri reali* non godono della proprietà commutativa perché sono affetti dalle rappresentazioni approssimate

Le *operazioni con numeri interi* invece sono rappresentazioni esatte e quindi godono della proprietà commutativa

# Come rappresentare i numeri reali
Per rappresentare i numeri reali, quindi i numeri con la virgola, ci sono due tecniche.
## Virgola fissa
In questo caso si utilizzano un numero di bit fissi per rappresentare i numeri prima della virgola e un numero di bit fisso per rappresentare i numeri dopo la virgola.

Consideriamo con la lettera $I$ i numeri prima della virgola, quindi i numeri interi, e con $D$ i numeri dopo la virgola, i decimali.

Inoltre alla $I$ togliamo un bit per rappresentare il segno
$$
N_{10}=(-1)^S\cdot(\sum^{I-1}_{i=0}a_i\cdot 2^i+\sum^{-D}_{d=-1}b_{d}\cdot b^d)
$$

Ad esempio se (per ora facciamo in decimale) dedichiamo 2 cifre per la parte decimale del numero e 6 cifre per la parte intera otteniamo che il numero
$12,3456$ 
Viene rappresentato come $+00012,34$ notare che prima della virgola ci sono esattamente $6$ cifre *compreso il segno* e dopo la virgola ce ne sono esattamente due.

È importante specificare come la parte decimale è stata troncata creando uno dei problemi più grandi della rappresentazione dei numeri reali ovvero l'impossibilità di rappresentare numeri che hanno valori infiniti dopo la virgola (periodici e non)
## Virgola mobile
Il numero a virgola mobile permette di scegliere *in un certo range* quanti bit possono essere utilizzati per la parte decimale e la parte intera del numero.

Si definiscono quindi 3 cose per poter utilizzare questa rappresentazione:
- $S$ il bit del segno
- $m$ O la mantissa che sono tutte le cifre senza nessuna virgola
- $e$ il numero che dice quante cifre ci sono dopo la virgola

Vengono uniti attraverso l'operazione $(-1)^S\cdot m\cdot 2^e$

di cui $m$ è il numero senza virgola ne niente ed $e$ è il numero di cifre che devono essere poi codificate come *cifre decimale*
In poche parole con il numero binario $10101010.0\cdot 2^e$ questa $e$ indica quanto si deve spostare verso destra il numero binario mantenendo la virgola dov'è:
$1010.1010$ = $10101010\cdot 2^4$ perché abbiamo preso il numero sopra e lo abbiamo spostato di 4 cifre verso destra

### Ma dove sono posizionati nell'intera serie di bit?
I vari range sono divisi seguendo lo standard IEEE754 a 32 bit in:
- 1 bit per rappresentare il segno
- 8 bit per rappresentare l'esponente $e$
- 23 bit per rappresentare la mantissa $m$

Ma come vengono ottenuti?

Innanzitutto si prende il valore con la virgola mobile
$18.75_{10}=10010.11_{2}$
Si normalizza il numero quindi *si lascia un solo bit dietro la virgola*
$1.001011$ e lo si moltiplica per $2$ elevato al numero di cifre per cui ci siamo dovuti spostare verso destra
$1.001011\cdot 2^4$ l'esponente in binario è $100$
Poi si applica il *biass* ovvero un valore per cui viene sommato l'esponente per permettere la rappresentazione degli esponenti negativi
$4_{(10)}+127_{(10)}=00000100_{(2)}+01111111_{(2)}=10000011_{(2)}$

Concatenando *$S$*$+$**$e$**$+$$m$ si ottiene il codice binario
*$0$* **$10000011$** $001\ 0110\ 0000\ 0000\ 0000\ 0000$

# Codici alfanumerici

I simboli alfa numerici non sono soltanto le i simboli che rappresentano le cifre numeriche o le lettere dell'alfabeto ma anche caratteri come lo spazio o i "va a capo"

Questi vengono raffigurati anche loro attraverso il codice binario ma la differenza è che invece di rappresentare un numero una specifica serie di bit.

Che simbolo viene rappresentato da che codice viene specificato attraverso la tabella ASCII
![[Pasted image 20241018121615.png]]

ovviamente la tabella ASCII ha tante cifre quante sono il numero di combinazioni che si possono ottenere con un certo numero di bit. Ad esempio con 8 bit possiamo avere $2^8=256$ caratteri rappresentabili
# Rappresentazione degli algoritmi
## Tipi di istruzione
- Istruzioni di ingresso e uscita (input\output), inserimento di dati o stampare dati
- Istruzioni di assegnamento (il processo in cui si assegna un valore a una certa cella di memoria)
- Istruzioni di controllo e alterazione della sequenza di istruzione
	- Alterazione condizionata ("*Se si verifica questa condizione vai qui*")
	- Alterazione incondizionata

## Flowchart
Il flowchart non è altro che una rappresentazione grafica di un algoritmo attraverso blocchi che hanno delle specifiche funzioni

![[Pasted image 20241018122729.png]]Abbiamo quindi:
- i due blocchi di *start e end* perché l'algoritmo deve avere necessariamente un inizio e una fine
- Process: il blocco che si occupa di fare operazioni e assegnarle a qualcosa *è quindi un istruzione di assegnamento*
- I due blocchi di input\output
- Test: Il blocco condizionale. Ce ne sono di vari tipi:
	- While: Esegui *in continuazione* una certa sequenza finché una certa condizione non diventa falsa
	- If: Esegui una sequenza se una certa condizione è vera

## Lo pseudo codice
In generale prima di utilizzare il linguaggio di programmazione conviene utilizzare il flowchart oppure lo pseudo codice così da creare un algoritmo di risoluzione di un problema senza dover pensare alla sintassi di qualcosa

Lo pseudo codice è quindi una specie di codice ma che non segue la sintassi di nessuno linguaggio di programmazione:
Esempio:
```Pseudo-codice
Inizio
	Leggi il numero intero A
	Leggi il numero intero B
	Somma = A + B
	Visualizzare Somma
Fine
```

È importante ricordare che durante un'operazione di assegnazione si legge da destra verso sinistra quindi si nell'esempio "Somma = A+B" prima si somma A+B e poi si inserisce dentro la variabile Somma

Ovviamente quando si crea uno pseudo codice si decide a che livello di dettaglio arrivare
Esempio dire semplicemente: "calcolare il valore assoluto" oppure descrivere tutti i passaggi per calcolare un valore assoluto di un numero

## La tabella di traccia
La tabella di traccia è solo una tabella che contiene tutte le variabili all'interno di un programma e tiene traccia dei valori che prendono in una certa istruzioni

# Programmazione strutturata
La programmazione strutturata consiste in delle regole fatte appositamente per rendere il codice o l'algoritmo *più leggibile*

Questo struttura contiene 3 blocchi:
- Blocco: concatenazione (Sarebbe in quadrato e rappresenta le operazioni che vengono eseguite)
- Selezione: Strutture condizionali che permettono di eseguire diverse operazioni 
- Ciclo: Strutture di iterazione

![[Pasted image 20241018124125.png]]

## Principio importante che ogni blocco deve avere
La cosà più importante di un blocco è il fatto che questo blocco debba avere un ingresso e un uscita
![[Pasted image 20241018125105.png]]
# Algebra di boole
L'algebra booleana si basa su due soli stati:
- Acceso (vero)
- Spento (falso)

Le variabili dell'algebra booleana possono prendere solo due valori e si chiamano variabili logiche

## Gli operatori logici
Le operazioni che si possono fare su due variabili logiche sono And, Or, Not

Attraverso queste operazioni possiamo creare delle tabelle booleane che descrivono semplicemente date due variabili logiche che valore risulterà una certa operazione
### And
L'*operatore logico* And (&&) si comporta esattamente come una moltiplicazione infatti la sua tabella della verità è:

| $A$ | $B$ | $A\cdot B$ |
| --- | --- | ---------- |
| $0$ | $0$ | $0$        |
| $1$ | $0$ | $0$        |
| $0$ | $1$ | $0$        |
| $1$ | $1$ | $1$        |
#### Proprietà dell'And
$A\text{ and } 0=0$
$A\text{ and }1=A$
$A\text{ and }A=A$
$A\text{ and }\overline{A}=0$
$A\text{ and }B=B\text{ and }A$ (Proprietà commutativa)
### Or
L'operatore logico Or (||) si comporta come un'addizione:

| $A$ | $B$ | $A+ B$ |
| --- | --- | ------ |
| $0$ | $0$ | $0$    |
| $1$ | $0$ | $1$    |
| $0$ | $1$ | $1$    |
| $1$ | $1$ | $1$    |
#### Proprietà dell'Or
$A\text{ or }0=A$
$A\text{ or }A=A$
$A\text{ or }1=1$
$A\text{ or }\overline{A}=1$
$A\text{ or }B=B\text{ or }A$
### Not
L'operatore logico Not invece è restituisce l'inverso del numero che gli viene dato:

| $A$ | $\overline{A}$ |
| --- | -------------- |
| $0$ | $1$            |
| $1$ | $0$            |

#### Proprietà del not
$\overline{\overline{A}}= A$
## Funzioni logiche
Le funzioni logiche sono funzioni nell'algebra booleana che date delle variabili restituiscono vero o falso e sono caratterizzate da una specifica tabella della verità