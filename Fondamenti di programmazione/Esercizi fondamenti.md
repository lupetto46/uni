---
Data: 24-11-2024
tags: Fondamenti_di_programmazione
---


# Esercizi fondamenti
## Prendere un numero e controllare se è positivo
```C
#include <stdio.h>

  

/* Esempio 1 n deve essere positivo */

  

int main(void)

{

    int n; // dichiarazione variabile intera chiamata n

    printf("Inserisci un numero: "); // stampare una stringa

    scanf("%d", &n); // leggere da terminale un intero e memorizzarlo in n

    if (n < 0) // controllo se n è minore di 0

        printf("Errore: n deve essere positivo\n"); // stampare una stringa

    else

        printf("%d\n", n); // stampare il valore di n

    return 0;

}
```

## Preso un numero controllare se è compreso tra 3 e 15
```C
#include <stdio.h>

  

/* Esempio 2 n deve essere compreso tra 3 e 15 */

  

int main(void)

{

    int n; // dichiarazione variabile intera chiamata n

    printf("Inserisci un numero: "); // stampare una stringa

    scanf("%d", &n); // leggere da terminale un intero e memorizzarlo in n

    if (n < 3 || n > 15) // controllo se il numero è minore di 3 oppure se è maggiore di 15

        printf("Errore: n deve essere compreso tra 3 e 15\n"); // stampare una stringa

    else

        printf("Il valore è corretto: %d\n", n); // stampare il valore di n

    return 0;

}
```

