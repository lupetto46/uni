---
Data: 24-11-2024
tags: Fondamenti_di_programmazione
---


# Architettura del calcolatore
I calcolatori utilizzano ormai quasi per standard un'architettura particolare ideata da Von-Neuman
![[Pasted image 20241018154310.png]]
Questa architettura ha 4 componenti principali:
1. [[#La memoria]] centrale (per il momento non ci interessa sapere esattamente di che tipologia è l'importante è sapere che è una memoria)
2. Un'unità di controllo ovvero la CPU o Processore
3. L'unità aritmetico logica che ha il compito di eseguire le operazioni aritmetiche (come addizioni e sottrazioni) o i confronti tra due numeri
4. L'unità input\output che ha il compito di prendere valori di input (esempio più banale sarebbe l'input da tastiera o il mouse) oppure inviare valori di output (un esempio sarebbe l'output di immagini su schermo)

## La memoria

Le memorie sono generalmente divise in due tipologie:
- Memorie interne o centrali:
  L'esempio più banale è la RAM del nostro computer ed è la memoria su cui vengono copiati i programmi quando vengono utilizzati dalla CPU
  
  Ha delle particolarità:
  - Accesso casuale: Significa che si può accedere al singolo byte cosa che non è fattibile in tutte le memorie
  - Volatile: Se si stacca la corrente i dati si perdono
  - Più veloce
  - Più costosa: in quanto è più difficile da creare e la tecnologia è più avanzata
- Memoria esterna o di massa:
  L'esempio più basilare sarebbe una chiavetta USB e anche questa ha delle particolarità:
  - Si accede a blocchi: contrariamente dall'accesso casuale questa è divisa a blocchi e quando si vuole accedere a un dato si deve trasferire all'interno della memoria centrale un intero blocco della memoria di massa
  - Persistente: I dati rimangono anche se si spegne
  - Più lenta
  - Meno costosa in quanto più facilmente creabile e la tecnologia è meno avanzata

### Tecnologie di memoria
Ci sono diverse tipologie di memoria e ognuna di queste sono organizzate in ordine di velocità o meglio in velocità di risposta (*latenza*)

La latenza non è altro che il tempo che ci mette una memoria a dare il dato che gli è stato richiesto
![[Pasted image 20241018155628.png]]

#### Tipologie di memorie interne
Le memorie interne o centrali sono quelle in cui devono stare tutti i dati che dovranno poi essere trattati dalla CPU e ce ne sono di 3 tipi:
- Random Access Memory (RAM): La memoria centrale del computer in cui vengono inseriti i programmi quando vengono eseguiti
- Read-Only Memory (ROM): Questa è una memoria persistente la cui unica operazione che permette è la lettura e viene utilizzata nella maggior parte dei casi per far partire il programma di accensione del computer.
- Cache Memory: La memoria Cache è una memoria relativamente piccola gestita direttamente dall'hardware in cui vengono messi gli ultimi comandi che sono stati eseguiti *nel caso in cui* vengano eseguiti di nuovo così da risparmiare il tempo che si impiega per accedere alla memoria centrale

#### Tipologie di memorie esterne
Le memorie esterne sono le memorie in cui si inseriscono i dati sotto forma di file anche di questa ci sono 3 tipi:
- Tecnologia magnetica:
  Una tecnologia che sfrutta le proprietà magnetiche dei materiali per poter salvare i dati.
  
  Un esempio riguardante questa tecnologia è la Hard Disk (HDD):
  Ovvero un dispositivo che sfrutto uno o più dischi magnetici per poter, attraverso una levetta posta sopra di essi, salvare e leggere dati.
- Tecnologia SSD:
  Questa tecnologia sfrutta schede di memoria flash collegate fra loro e, contrariamente dall'HDD, non ha parti mobili.
- Tecnologia ottica:
  La tecnologia ottica è una tecnologia come il DVD o il CD o il Blu-Ray che sfrutta un raggio laser per leggere su un disco con sopra un sottile foglio di metallo.

# Esecuzione dei programmi
## Cosa avviene realmente in un programma?

È abbastanza nascosto dagli ambienti di programmazione 
Si passa dal linguaggio sorgente al linguaggio oggetto ovvero un linguaggio intermedio molto vicino al linguaggio macchina. Ha dei cosiddetti "simboli non risolti" ovvero problemi che io ritrovo già risolti in librerie pre-esistenti

Per poter garantire la portabilità del sorgente
Ovvero che indipendentemente dal calcolatore e le sue impostazioni il sorgente fa ciò che c'è scritto che dovrà fare

### Quando vengono cercate queste librerie già pronte?
Durante la fase di read

Controllo tutti i simboli e li associo con il codice della libreria a cui sono associati

Il linguaggio oggetto è uguale per tutti i linguaggi di programmazione.

Il linguaggio oggetto è legato all'architettura e al sistema operativo.

Passo del link che è ancora più legato alla macchina.

### Collegamento con i programmi di supporto
I linguaggi interpretati hanno bisogno sempre dell'interprete


### Caricamento in memoria
Poi si carica la memoria


## Cosa succede durante la compilazione?

### Analisi
Un'analisi lessicale, grammaticale e contestuale. 
Controlla se la sintassi del codice sorgente è corretta
Poi un analisi contestuale ovvero se tutto ciò che si trova nel programma trova corrispondenza in tutto quello che c'è scritto nel programma

### Trasformazione da sorgente a oggetto
#### Creazione di una tabella di simboli
I simboli sono solo nomi che si assegnano come i nomi delle variabili o altre cose questi nomi delle variabili vengono inserite all'interno di una tabella

### Ottimizzazioni
L'ottimizzazione viene eseguita del compilatore permettendo al programmatore di concentrarsi sulla leggibilità del codice

## Il linker
Il linker è ciò che collega diversi moduli e oggetti attraverso simboli

## Il loader
Il loader carica il programma in memoria

# Ambienti integrati

Gli IDE automatizzano la procedure compilando il file sorgente e invocano i linker

ma per farlo devono sapere quali sono i file sorgenti che costituiscono l'applicazione e il nome dell'eseguibile da produrre

# Struttura di un programma
## Le libreria
Intanto si dichiarano le librerie.
*Ricordare di inserire le librerie solo se necessarie*
La sintassi in C per includere le librerie è:
```C
#include <stdio.h>
```

## Dichiarazione delle funzioni
Una funzione in C è particolarmente importante ovvero il "**Main**" e il suo scopo è per dire al programma "*inizia da qua*"

```C
#include <stdio.h>

int main() {
	/* Il codice inizia da qui */
}
```

### Dichiarazioni delle variabili
Il C è un linguaggio tipizzato quindi quando si crea una variabile è necessario inserire il tipo (Se è intero, reale, una stringa, una lista ecc).
Una volta dichiarata il compilatore creerà il simbolo lo inserirà nella tabella e capirà come interpretarla

