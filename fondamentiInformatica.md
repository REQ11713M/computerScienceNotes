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

### Lezione 3 (2024/09/24)
		"Qualcuno non è interessato, lo invito ad andare a chiacchierare altrove. Purtroppo il dipartiento è spostato dal centro, provedderemo a spostarlo così potete andare in bar più carini" -L. Paolini
		"Circuiti come fliflòp" L. Paolini
		Macchine a 64 bit --> possiamo avere 2^64 (1.8*10^19) indirizzi di memoria
		Salvare vuol dire memorizzare in qualche dove anche in assenza di alimentazione l'informazione viene mantenuta
		"Non c'è nessun problema a riprenderlo" grandissima cit falsa di Paolini, probably
		"Se apro le mail adesso ho decine di mail. Dalle offerte di viagra a tutto il resto... Sarà l'età" -L. Paolini
		I primi (?) metodi di archiviazione dell'informazione sono stati i dischi magnetici
			Organizzati in dischi uno sopra l'altro
			Per chiedere al disco di avere un byte bisognava indicargli tre informazioni:
				- Il cilindro: il fascio di tracce
				- Head (testina): sopra sotto
				- Settore
			Funzionano magnetizzando con poli diversi i "bit" del disco
		Altri dispositivi di memoria di massa sono i cd, i dvd e i blu-ray
			Per i dischi non riscrivibili vengono bruciate delle parti riflettenti in modo che non riflettano più
				"Una luce così forte da bruciare lo specchio, come quando io mi guardo la mattina allo specchio"
			Nel caso dei blu-ray la capacità di memoria è maggiore grazie al fatto che possono essere letti sia da sopra che da sotto e sono composti da layer
			Le informazioni sono scritte a spirale, quindi il lettore non può saltare da una parte all'altra (non sono infatti divisibili in settori concentrici)
		Flash Drives
			I bit sono memorizzati in celle di ossido di silicone. Vengono depositati degli elettroni. Se non ci sono, l'informazione è 0
			Hanno il vantaggio che queste celle di ossido di silicone mantengono intrappolati gli elettroni per qualche anno
		SSD (Dischi allo Stato Solido)
			Sono privi di motore --> consumano meno e non fanno rumore
				"I vecchi computer facevano un rumore abbastanza... rrrrrr... non banale"
			Essendo privi di puntina, se cadono non c'è rischio che la puntina vada a rovinare il disco
		SD (Secure Digital) memory cards (SD cards), SDHC (High Capacity), SDXC (Extended Capacity)
			Anche queste funzionano con l'ossido di silicone
		Tutta l'informazione che noi memorizziamo nei computer digitali è composta da soli numeri
		"La prima proposta p stata quella del codice ASCII (AS-kee), a volte ASCII (ashi)... NON HASHISH"
		ASCII
			A ogni sequenza di 0 e 1 corrisponde un numero, una lettera, un simbolo o una "azione"
			"Ovviamente li dovete sapere tutti a memoria... Ovviamente scherzo" -L. Paolini (aggiungo: molto divertente. Aggiungo: ironia)
			Il fatto che ci fosse un bit in più a disposizione ha portato varie espansioni
			Molti dei computer, soprattutto quelli Windows, utilizzano UNICODE. Utilizza fino a 21 e l'obiettivo è che abbia caratteri sufficienti per scrivere in qualsiasi lingua e qualsiasi simbolo l'umanità abbia mai inventato
			"Parentesi angolououse" -L. Paolini
			L'informazione è sempre scritta in un file di testo, anche se si deve usare un certo font o se il testo è in grassetto e così via.

---

Per provare a convertire con l'ASCII e altra roba che non ho seguito

https://www.rapidtables.com/convert/number/ascii-hex-bin-dec-converter.html

---
