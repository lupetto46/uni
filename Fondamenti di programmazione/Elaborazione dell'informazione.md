#fondamenti_di_programmazione
La complessità computazionale cerca di ottenere delle metriche indipendenti dal calcolatore in cui un algoritmo viene eseguito

Ci sono due metriche:
- Numero di istruzioni per eseguire una riga di comando
- Spazio in memoria necessario per risolverlo

Sfortunatamente la storia ci ha fatto scoprire che è impossibile ottimizzare sia il numero di istruzioni che lo spazio

È quindi necessario capire in che contesto sto creando l'algoritmo

> [!example] esempio
> Un profilo utente chiederebbe minimo 100 byte tra nome cognome data di nascita codice fiscale ecc..
> Per 100 alunni sarebbe 10 Kb


Se volessi studiare la rete internet e ne volessi studiare il grafo avrei bisogno di una matrice bidimensionale $nxn$ quindi $10^{12}\cdot10^{12}$ e non ci basta quindi più la memoria

Scopo e obbiettivi:
- Ingegneria informatica
	- Scopo pratico e applicativo
- Scienza informatica
	- Prove matematiche, dimostrazioni a scopo di ricerca di nuovi algoritmi

### Programmazione
SI predispone l'elaboratore a risolvere un problema attraverso dei passi e dei dati che devo trovare io
Un programma è una sequenza di istruzioni o comandi allo scopo di ottenere il risultato desiderato
Quando viene eseguito esegue le istruzioni del programma in modo sequenziale

### problema
Un problema deve essere definito chiaramente e formalmente spesso in termini di inputo desiderato e output atteso

## Definizioni
- **Soluzione di un problema**:
	 - Esprimere un *elenco di istruzioni* che poi l'*esecutore interpreterà* è importante inoltre avere un modo per *verificare che i dati in uscita sia corretta*
- **Esecutore**:
	- *Macchina astratta* il cui scopo è *interpretare* delle *istruzioni* scritte in un programma
- **Macchina astratta**:
	- Indica un modello teorico di hardware o software in grado di *eseguire operazioni*, *memorizzare dati* e *seguire il flusso dell'algoritmo*

- Quali sono le condizioni per dire che un problema è ben formulato?
	- Non è *a priori* evidente che *non esistono* soluzioni
	  >[!important] importante
	- Il *criterio di verifica* delle soluzioni *è univoco* e si sa come applicarlo
	- L'insieme dei *dati iniziali* è completo
- 