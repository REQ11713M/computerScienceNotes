# Appunti Di Informatica
## Programmazione 1
### Lezione 1 (2024/09/19):
		"Il mio tempo, che sto spendendo perché mi pagano, mica faccio volontariato" -A. Mazzei
		"Siete venuti qua e ve lo aspettavate, programmazione 1, mica è matematica discreta" -A. Mazzei
		"Dovete sentire la gioia che si prova quando si programma, e poi certo ci sono i soldi" -A. Mazzei
		- Capire cos'è un algoritmo
		- Macchina di Von Neumann (tutti i computer sono macchine di Von Neumann)
		- Prog 1 --> paradigma imperativo
		- Differenza tra algoritmo e programma
		- Differenza tra C e altri linguaggi (differenza tra linguaggi ad alto e basso livello)
		- 48 ore di teoria + 30 ore di laboratorio
		Mette in tutte le slide il simbolo della pace perché "Siamo fortunati a poterlo fare (studiare all'università) in una situazione di pace.
			Mi piace mettere questo simbolo perché lo riusciamo a afare solo perché siamo oim una situazione di pace e non è una cosa scontata"
		C è un linguaggio imperativo e strutturato
			Un algoritmo è una sequenza di ordini e istruzioni che servono per risolvere un problema --> imperativa
			Strutturata perché le istruzioni vengono raggruppate in dei blocchi che vengono strutturati (if, for, ecc...)
		All'inizio si spostavano i fili, poi con 0 e 1, solo dagli anni '60 circa si usa la programmazione strutturata
		All'esame: un esercizio di programmazione iterativa e un esercizio di programmazione ricorsiva
		La programmazione ricorsiva è un approccio diverso alla risoluzione dei problemi
		Programmazione ricorsiva: caso base e caso più complesso riconducibile al caso base (es. Sequenza di Fibonacci)
		Per alcuni problemi è più facile la soluzione ricorsiva di quella iterativa, nonostante una soluzione iterativa sia sempre trovabile (supporrei tramite i cicli?)
		Un altro esercizio nell'esame riguarderà lo stato della memoria
		Utilizzeremo infatti lo spazio che ci mette a disposizione la macchian di Von Neumann
		Attraverso un test a risposta multipla ci fanno vedere un pezzo di codice e ci chiedono quale sia lo stato della memoria
		Altro esercizio riguarda la correttezza: riesco a dire se un programma sia corretto senza eseguirlo? --> Semantica assiomatica
		"Per imparare a programmare c'è bisogno di 10 anni, diceva Peter Novig"
		"Il linguaggio C - Fondamenti e tecniche di programmazione, Nona edizione" - gratis su telegram
		Useremo il terminale per programmare
		La macchina di Von Neumann è divisa in HEAP e STACK
		Prendere appunti serve per rimanere concentrati più che per studiare
		LA MARATONA NETFLIX!!!!!! (ergo: non seguire le lezioni e guardarsi le registrazioni i giorni prima dell'esame non è una buona strategia di studio)
		"Non voglio creare stress nelle persone, quindi magari facciamo su base volontaria. Vorrei promuovere l'interazione, in tutto il corso potete dire tutte le sciocchezze che volete"
		Il C è uno dei primi linguaggi di programmazione, ma sono linguaggi con paradigmi diversi
		C++ e C# utilizzano il paradigma a oggetti, C utilizza il paradigma imperativo
		C è di "medio-alto" livello
		"Se vi sentite un po' confusi, sappiate che non siete gli unici. Non vi preoccupate, succede di avere degli intoppi, io sono stato bocciato ai primi tre esami"
		"Mi arrivavano una volta le mail da cavaliereoscuro@gmail.com. Io rispondo solo alle mail d'ateneo, non cavaliere oscuro"
		
		Cosa sono i computer e gli algoritmi?
			I computer sono uno dei tanti modelli computazionali per risolvere algoritmi
			I computer erano delle persone molto brave a fare i conti
			Dagli anni '50 è programmabile
			Dijkstra è uno degli informatici più influenti del secolo scorso. L'informatica non è la scienza dei calcolatori, il calcolatore è lo strumento.
			L'informatica è quindi lo studio degli algoritmi
			Informatica = INFORmazione autoMATICA
			Le lingue umane sono molto compatte - una frase è molto ambigua ma noi siamo in grado di disambiguarla e interpretarla
			La macchina di Von Neumann non riuscirebbe a disambiguare. I linguaggi di programmazione non sono ambigui.
			Si inizia a parlare di algoritmi intorno all'800, da quando al-Khwarizmi ha scritto "Calcoli con i numerali indiani"
			Un algoritmo è un insieme di operazioni non ambigue ed effettivamente computabili che quando eseguito produce un risultato e si arresta in un tempo finito
			Non ambigue ed effettivamente computabili: c'è un agente di calcolo, cioè colui a cui è rivolto l'algoritmo
			Il nostro agente di calcolo in questo caso è il compilatore di C, che poi rende comprensibili le istruzioni per la macchina di Von Neumann
			"Gli algoritmi sono simili a un libro di cucina: hai un input, gli ingredienti, e un output... Si spera."
			La stessa istruzione può essere ottima per un cuoco e pessima per un altro
			Il concetto di unità o di numero è difficile da spiegare perché è un concetto, ma l'addizione è meccanica.
			Gli algoritmi manipolano dei segni e così ottengono anche dei significati
			Gestire all'interno di uno spazio dei valori.
			Assegnare un certo valore a una certa variabile vuol dire che vado ad assegnare sul foglio quel valore. Il "foglio" della macchina di Von Neumann
				si chiama memoria primaria. A ogni spazio assegnamo un nome (per esempio, "i")
			Ciò che c'è nella memoria mi dà lo stato della memoria
			"Ci sono tre cose importanti nell'informatica: zero... uno... due..." perché a tutti gli informatici piace iniziare a contare da zero
			Pseudocodice: una roba che assomiglia un po' al linguaggio umano e un po' a C. Non va bene per la macchina di Von Neumann, ma forse manco per gli umani
			Se io riesco a scrivere un algoritmo per fare le addizioni posso delegare a "qualcun altro" il compito di farlo
			"Qua ho scritto mio fratello, ma lo pago, per non sfruttarlo proprio a gratis" -A. Mazzei
			"Ho spoilerato diciamo, mo' non venite perché dite <<boh ho già visto tutto>>" -A. Mazzei
			Automatizzare vuol dire guadagnare un sacco di tempo della nostra vita, "e siamo tutti felici"
### Lezione 2 (2024/09/23)
		Accumulatore per memorizzare la somma parziale
		Un contatore i per memorizzare il numero di addizioni
		FLOW-CHART o PSEUDOCODICE: alternative per scrivere codice comprensibile all'essere umano
		La differenza tra questo corso (prog1) e quello di algoritmi è che qui impariamo la sintassi fondamentalmente e come trasformare da italiano a C, ad algoritmi invece progettiamo algoritmi
		Che cos'è la macchina di Von Neumann?
			Sia pc che telefoni che tablet eccetera sono tutte macchine di Von Neumann (approfondimento all'esame di architettura degli elaboratori)
			La storia dell'informatica:
				Parte da lontano (algoritmi nel 800 d.C. con al-Khwarizmi)
				Turing (1936)
				Architettura di Von Neumann (1945)
				Personal Computer (1975)
				La Pascalina (1642), inventata da Blaise Pascal, è la prima addizionatrice meccanica
				La differenza tra la Pascalina e il calcolatore moderno è che la Pascalina può fare UNA SOLA COSA (fare operazioni), mentre il calcolatore moderno è PROGRAMMABILE
					(calcolatore vs calcolatrice)
				Possiamo creare un calcolatore programmabile se è possibile esprimere input e output numericamente
				La prima macchina programmabile è stata creata da Charles Babbage (1840)
					Il linguaggio di programmazione utilizzato è simile all'assembly
					La macchina è Turing-complete, la differenza tra la macchina di Turing e quella di Babbage è che la seconda è analogica
						Entrambe sono comunque solo macchine teoriche che non sono mai state realizzate
					Turing introduce il concetto di macchina universale
						Nasce così uno dei pilastri dell'informatica: la teoria della calcolabilità
						Turing ha creato il primo algoritmo degli scacchi (Turochamp)
						Esistono problemi che non possono essere risolti da un algoritmo generale
						Ci sono operazioni che vengono scelte in base allo stato interno della macchina
				Prima macchina di Von Neumann costruita (EDVAC):
					1944 da J. Mauchly e J. Presper Eckert
					Rappresentazione binaria dei dati
						BInary digiT --> BIT (anche: Binary Information Token).
							Elemento di base dell'informazione
						Vero/falso, sì/no, acceso/spento, etc...
							Può essere implementato con vari dispositivi hardware di semplice realizzazione fisica (relè, valvole, transistor)
							Da qui la sua adozione nei calcolatori moderni rispetto alla rappresentazione decimale usata dai primi calcolatori
								Molto conveniente perché si possono utilizzare vari fenomeni fisici "vero/falso" (direzione campo magnetico, etc...)
							b: bit, B: byte
					6000 valvole e 12000 diodi, è composta da:
						memoria primaria (ram): 1024 parole di 44 bit
						mememoria secondaria a nastro magnetico per lettura/scrittura
						unità di controllo con un oscilloscopio
						ALU (arithmetic logic unit) che esegue le operazione su due operandi
					Un programma viene eseguito nella memoria primaria, perché è notevolmente più veloce
					Cambiando dei bit nella memoria primaria, riprogrammi il computer. Se prima fa le divisioni, ora può togliere gli occhi rossi dalle foto, etc...
					Per indicare quale cella ti interessa nella RAM devi fornire il suo indirizzo binario
					La CPU legge ed esegue ciò che c'è nella memoria primaria
					Lo stato della macchina è effettivamente dato dalla memoria primaria
					La memoria primaria contiene dentro di sè sia l'algoritmo che l'input. Sono nello stesso spazio fisico.
				Quando noi programmiamo stiamo scrivendo nella memoria primaria, che è il nostro "spazio"
		Linguaggi ad alto e basso livello:
			Indica la vicinanza al linguaggio della macchina (basso --> più vicino, alto --> più lontano)
			Differenza tra C e Assembly:
				Linguaggio ad alto livello:
					Mi astraggo dai dettagli della macchina e programmo una macchina di Von Neumann generale
				Funzionamento di una CPU:
					Implementa semplici istruzioni aritmetiche sui registri
					Può copiare dati fra memoria e registri
					Può eseguire istruzioni in ordine anche non consecutivo
					Istruzioni di salto incondizionato
					Istruzioni di salto condizionato
					Control Unit: preleva dalla memoria e deocidifica una istruzione alla volta
					Istruzioni codificate su 16 bit l'una
						0010 00 0110010000 = Carica / nel registro R0 / il contenuto del 401esimo byte
					Programma: codifica di un algoritmo in un linguaggio di programmazione (in quale lingua voglio parlare)
					Linguaggio di programmazione:
						Framework ("ambiente") per scrivere ed eseguire algoritmi (o programmi, scritti in quella specifica lingua)
						Insieme di parole e di regole definite in modo formale per consentire la programmazione di un calcolatore affinché esegua compiti predeterminati
						L'EDVAC era programmato in linguaggio macchina
						Il linguaggio assembly viene sviluppato alla fine degli '40 per sollevare il programmatore dai task più error-prone
						L'insieme di istruzioni assembly viene detto sorgente assembly
						I primi programmatori programmavano proprio in 0 e 1, successivamente è stato creato l'assembly (che però non è portabile, ciascuna macchina ha il suo)
						Esempio: addizione fra interi in assembly
							ADDR A = 400
							ADDR B = 402
							LOAD, R0, A
							LOAD, R1, B
							ADD, R0, R1
							STORE, R0, A
						Esempio: moltiplicazione di interi in assembly
							LOAD, R0, 0
							LOAD, R1, 0
							LOAD, R2, m
							LOAD, R3, n
							CMP, R1, R3
							JMPEQ <riga 10>
							ADD, R0, R2
							ADD, R1, 1
							JMP <riga 5>
							STORE, R0, m
						La codifica in linugaggio assembly è efficiente ma è un processo di codifica lungo e facile all'errore
							4 righe di codice per addizione, 10 per la moltiplicazione
						Richiede la consocenza dell'architettura della CPU, poiché il codice scritto per una CPU deve essere riscritto da capo per funzionare su un'altra CPU se implementano istruzioni differenti
						A partire dagli anni '50 vennero sviluppato linguaggi di programmazione con istruzioni dalla semantica più vicino al linugaggio umano e che permettessero di astrarre il programma dalle caratteristiche dell'hardware
						"Scialla Fra! Ma forse non si usa più scialla. Cosa si usa adesso? Chill? <<Chill bro>>, dal prossimo anno scrivo <<Chill bro>> sulle slide" - A. Mazzei
						Vogliamo un interprete, qualcuno con cui possiamo dialogare con una logica più vicina agli esseri umani
						Il linguaggio FORTRAN (FORmula TRANslator):
							All'inizio degli anni '50 IBM progetta il modello 704 per calcoli scinetifici in virgola mobile con una certa quantià di requisiti
								Per esempio, gli scienziati non devono aver bisogno di conoscere nello specifico la maccina su cui programmano ma devono concentrarsi sulla risoluzione dei problemi
							Versioni moderni offrono costruitti if, while, etc...
							Un compilatore traduce ogni istruzione FORTRAN in una o più istruzione assembly specifiche per la macchina utilizzata
							Se cambia la macchina utilizzata, è sufficiente ricompilare il programma per l'hardware relativo
							Insieme a LISP, ALGOL, COBOL rappresenta il capostipite dei linguaggi di terza generazione, famiglia a cui appartiene il linguaggio C originario
						Le variabile sono "spazi" in cui voglio mettere dei valori, ma sono spazi generici
							Bisogna astrarsi dalla macchina
						Utilizziamo C perché è ancora uno dei più utilizzati al mondo
						--> Il Python si scrive alla cazzo di cane, quindi non lo usiamo. Il motivo per cui è molto utilizzato è perché è pieno di librerie: cose già fatte
### Laboratorio, lezione 1 (2024/09/25)
	"Il pinguino felice, perché ha appena mangiato un pesce ed è felice"
	"Linus è stato morsooooooo da un pinguinoooo"
	"Perché il simbolo di Windows è una finestra? Perché windows in inglese vuol dire finestra, e quindi è una finestra"
	Alcuni comandi sono integrati e caratterizzano l'uso standard del terminali
	Altri comandi (come il compilatore gcc per Windows) sono invece esterni
	C:\Users\amazzei>echo %PATH%
		ci mostra la directory in cui siamo
	"bin" sta per binary, non cestino lol. È il codice pronto per essere eseguito
	(Sì, questi appunti sono stati inutili ma perché non ha detto niente insomma. È tutto nelle slide lol)
### Lezione 3 (2024/09/26)
	Esistono linguaggi di alto livello e basso livello
	Il linguaggio C
		Nel 1969 Ken Thompson inizia a scrivere un sistema operativo
		Inizialmente sviluppato per uso interno sui computer pdp-7 e pdp-11
		Veros la fine degli 80 è standardizzato da ANSI e ISO per uso su una varietà di hardaware differente
		Lo standard ha subito numerosi aggiornamenti (C-99, C-11)
		Il libro di testo fa riferimento a C-11
			Il libro di Kernighan e Ritchie "The C programming language" è pensato per insegnare il C, non per insegnare a programmare
		Il linguaggio C è un linguaggio di programmazione:
			- Compilato:
				--> Un compilatore traduce i sorgenti C nel linguaggio macchina del caso
			- Imperativo:
				--> Il programma è un insieme di istruzione pensate come ordini per il compilatore
			- Strutturato:
				--> Il codice sorgetne è organizzato in blocchi racchiusi da delimitatori
			- Fortemente tipizzato:
				--> Il programmatore deve specificare il tipo di ogni variabile
			Il codice sorgente si avvicina alla logica degli esseri umani ma non è un linguaggio umano
				"Mica possiamo parlare di calcio con la macchina di Von Neumann" -A. Mazzei
				"La programmazione imperativa si avvicina alle ricette di cucina. A me hanno criticato i troppi esempi di cucina" -A. Mazzei
				"Se devo fare una torta divido la base dalla farcitura, e ciascuna di queste posso dividerle in ulteriori fasi" -A. Mazzei
				C'è una struttura nella soluzione
					Dividiamo i problemi in problemi più piccoli e più piccoli e così via.
						nb: si chiama "Divide et impera", nel caso in cui qualcuno volesse approfondire la cosa cercando su google
					"Be- OPS stavo per morire" -A. Mazzei
				L'esecuzione è fatta dalla macchina di Von Neumann direttamente con un codice in linguaggio macchina
				"IK-s (x)" -A. Mazzei
				"In passato il Pascal..." bro abbiamo capito che hai imparato a programmare con Pascal lol
		Primo programma in C:
			Capitolo 2 del libro di testo

---

	// fig02_01.c

	// A first program in c.

	#include <stdio.h>

	// function main begins program execution

	int main(void){

		printf("Welcome to C!\n");
	
	} // end function main

 ---
 

		"Sono tempi dolci per noi programmatori" -A. Mazzei
		"Se voi non indentate lo fate per cattiveria. Eh così Mazzei ci mette più tempo, ma Mazzei decide anche il vostro voto" -A. Mazzei
		"Microsoft non credeva in internet" -A. Mazzei
		"Questo è il simbolo di uno gnu... che mi pare sia... africano? Credo di sì" -A. Mazzei
		"Oh è Microsoft che mi rompe le cose... Non è vero di Unix, io c'ho Windows- Ecco vedete che funziona di nuovo? Ora esplode" -A. Mazzei
		Tipi di dati:
			Un tipo di dato è caratterizzato:
				Dalla rappresentazione in memoria dei dati di quel aprticolare tipo
				Dall'insieme di operazione ammissibili su dati di quel tipo
			A cosa servono i tipi di dati:
				Permettono di effettuare controllo statici sulla correttezza sintattica del programma e quindi prevenire errori
    			Tipi:
				- char 		1 byte				%c
				- int 		4 byte (d.s.)		%d
				- short 	2 byte (d.s.)		%d
				- long 		8 byte (d.s.)		%ld
				- float 	4 byte (d.s.)		%f
				- double 	8 byte (d.s.) 		%lf
					
				--> d.s. = di solito
