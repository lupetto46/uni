#fondamenti_di_programmazione
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
> Il sistema analogico consiste nel rappresentare informazione attraverso l'utilizzo di tutti i numeri dal $-\infty$ al $+\infty$ mentre invece il digitale consiste nel rappresentare l'informazione attraverso una serie di zero e uno.

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
- In generale della B la base e $c_i$ i coefficienti
$$
N=\sum^{n}_{i=0} c_i\cdot b^i
$$

## Conversione di base

### Da base 2 a base 10
$0111_{(2)}= 0\cdot 2^3 + 1\cdot 2^2+ 1\cdot 2^1+1\cdot 2^0=7_{(10)}$
Non è altro che prender il bit da destra verso sinistra e moltiplicarlo per la posizione del bit a partire da 0 fino a $(n-bit)-1$
### Da base 10 a base 2
Da base 10 a binario invece è diverso
È necessario prendere il valore dividerlo per la base e scrivere solo il resto che si ottiene dalla divisione:
$\frac{17}{2}$ fa $8$ con resto $1$
$\frac{8}{2}$ fa $4$ con resto $0$
$\frac{4}{2}$ fa $2$ con resto $0$
$\frac{2}{2}$ fa $1$ con resto $0$
$\frac{1}{2}$ fa $0$ con resto $1$

Si legge poi dal basso verso l'altro ottenendo che $17_{(10)}= 10001_{(2)}$
### Modulo e segno
Per rappresentare lo zero si prende innanzitutto il bit più a sinistra tra i bit disponibili.
> [!question] Perché il bit più a sinistra
> È una convenzione

E si utilizza come segno

*$1$*$0000000$ Questo numero è negativo
*$0$*$0000000$ Questo numero è invece positivo

ottenendo quindi che l'intervallo
$n\in [-(2^{k-1} - 1), 2^{k-1} - 1]$ in cui $k$ è il numero di bit disponibili

Il problema è che questo metodo ha 2 modi per rappresentare lo zero.

### Le operazioni
Prima di andare avanti è importante considerare le varie operazioni.
- Addizioni in modulo e segno:
	- Se i valori sono con lo stesso segno allora si sommano normalmente e il segno non cambia
	- Se i valori sono con segno diverso allora si fa la differenza tra il più grande e il più piccolo e il risultato è quello del più grande.
- Sottrazioni in modulo e segno:
	- In questo caso si deve cambiare il segno del sottraendo
	- E si utilizza l'algoritmo dell'addizione
- Overflow
	- Quando il numero che sta risultando dall'operazione è troppo grande per essere rappresentato con il numero di bit che si hanno. Se si verifica questo caso lo si può sapere attraverso un bit aggiuntivo che si attiva solo nel caso in cui si sommano i due bit più significativi
- Underflow:
	- Il caso in cui il valore che si sta cercando di rappresentare è troppo piccolo per essere rappresentato con il numero di bit che ho in questo momento
## Complemento a 2
Ma la domanda è: **Come posso rappresentare i numeri negativi avendo solo un  rappresentazione dello zero?**
I numeri si possono rappresentare come:
$127-n$
Quindi se voglio il numero 3 posso rappresentarlo come:
$127 - 124 = 3$
così facendo ho una sola rappresentazione dello $0$ che sarebbe $127-127$

Quindi:
Sia $k$ il numero di bit a disposizione

$n$ il nume binario naturale di $2^k+x$
Se voglio rappresentare il:
- $+6_{10}=+0110_{(2)}=2^4+0110= 1000+0110$

## Proprietà delle operazione
Le *operazioni con numeri reali* non godono della proprietà commutativa perché sono affetti dalle rappresentazioni approssimate

Le *operazioni con numeri interi* invece sono rappresentazioni esatte e quindi godono della proprietà commutativa

