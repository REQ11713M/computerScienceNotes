# Appunti Di Informatica
## Fondamenti dell'informatica
### Lezione 2 (2024/09/20)
		Tipi di computazione
			1- Digitale (informatica "autentica)
				- Discreta (associata ai numeri interi)
			2- Analogico
				- Continua (associata ai numeri reali)
			
			Ci sono anche quantistici, reversibili, probabilistici, biologici, eccetera
			
			Un algoritmo, da un insieme finito di input, a passi finiti, rende l'output
			La macchina di Turing è un particolare automa formale che permette di esprimere gli algoritmi in termini di opreazioni finitarie su un nastro
			I motivi per cui la macchina di Turing e il modello digitale si sono imposto sul modello analogico sono vari tra cui:
				- Sono in grado di simulare tutti gli algoritmi
				- Sono in grado di simulare una qualsiasi altra macchina
				- Evita alcune imprecisioni delle macchine analogiche
					Si programmano in termini di equazioni differenziali, era molto apprezzata dagli ingegneri
					Ha un problema: non si possono misurare bene i risultati perché viene scalata sull'hardware
			Turing va in contro a problemi matematici:
				- Precisare cosa sia un algoritmo
				- Gli informatici sono costretti a fare attenzione agli aspetti formali, diversamente dai matematici
			Matematica --> Logica --> Informatica --> Matematica
			Tutto ciò che facciamo nei computer digitali è trasformare una sequenza di 0 e 1, quindi numeri
			L'efficienza di un algoritmo si valuta in termini di complessità computazionale
			Per esempio nel caso degli algoritmi di ordinamento, per esempio la maggior parte di questi hanno complessità O(N^2)
				quicksort, mergesort e heapsort hanno complessità O(N*log(N))
				Per esempio supponiamo di avere N=1000000 elementi da ordinare, cioè 10^6
					Con i primi algoritmi faremo N^2 10^6 * 10^6 = 10^12 confronti
					Con gli altri tre avremo N*logN 10^6 * 6 confronti
					
		Bit e la loro archiviazione
			Cifre binarie o binary digits --> Binary digIT --> BIT
			Similmente a come succede nel corpo umano, noi siamo analogici ma ragioniamo in modo digitale
			Il computer in pratica sarebbe analogico, ma gli ingegneri fanno di tutto in modo che si comporti digitalmente (0-1V=0, 4-5V=1, 1-4V=BOH)
			Operazioni binarie principali: AND, OR, XOR, NOT. A seguire, le tabelle di verità:
			AND:
				0 AND 0 = 0
				0 AND 1 = 0
				1 AND 0 = 0
				1 AND 1 = 1
			OR:
				0 OR 0 = 0
				0 OR 1 = 1
				1 OR 0 = 1
				1 OR 1 = 1
			XOR:
				0 XOR 0 = 0
				0 XOR 1 = 1
				1 XOR 0 = 1
				1 XOR 1 = 0
			NOT:
				NOT 0 = 1
				NOT 1 = 0
			Si usano degli amplificatori (indicati con un triangolo che punta verso destra) per assicurarsi che il voltaggio sia sempre corretto.
				Infatti, con cavi troppo lunghi il voltaggio tende a calare.
					Fondamentalmente la redstone è uguale alla vita reale ma più debole e non riducibile. Non a caso è Turing Complete lol.
			"Esistono i <<fiflòp>>" -L. L. Paolini
			Circuiti SEQUENZIALI, che sono circuiti con retrazione (flip-flop, appunto)
				L'output produce uno dei valori dell'input.
					"Gridi per piacere, non so se gli altri... Sarò io sordo" L. L. Paolini
					Normalmente i computer hanno un alimentatore che genera una alimentazione fissa
					Dentro i chip si potrebbe realizzare tutto con queste porte e basta, ma ci sono anche tecnologie più avanzate per alcuni scopi.
				La prima porta si chiama SET perché la sua attivazione setta l'output a 1
				La seconda porta si chiama RESET perché la sua attivazione setta l'output a 0
				0-0 mantiene lo stesso output
				1-1 è una combinazione che non viene utilizzata
			Circuiti COMBINATORI, che sono privi di retrazione
				
			Con i flip-flop abbiamo usato i gate per far vedere come costruire qualcosa di più complicato
				Per capire come funziona un flip-flop non c'è bisogno di conoscere nel dettaglio come funzionano le singole parti (astrazione)
			È comodo scrivere i numeri binari in esadecimale
				In alcuni linguaggi si scrive 0x davanti al numero esadecimale
					e.g. 1101 --> 0xD
