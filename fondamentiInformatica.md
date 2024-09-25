# Appunti Di Informatica
## Fondamenti dell'informatica
### Lezione 1 (2024/09/18)
		In realtà non abbiamo detto praticamente niente
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

Per provare a convertire con l'ASCII, binario, decimale e così via (utile per gli esercizi)

https://www.rapidtables.com/convert/number/

---

		Come si rappresentano le immagini?
		
			Mappatura dei bit --> si può rappresentare una immagine
			"Il passaggio a una immagine a colori non è molto complicato" (ci sono volute solo un po' di decine di anni lol)
			Con 8bit possiamo scrivere 256 colori
			*immagini di gufi a bassa risoluzione*
				Normalmente le immmagini vengono memorizzate in questo modo, cioè con le bitmap o raster
			Un altro metodo sono le immagini vettoriali
				Le immagini vettoriali sono composte da funzioni che descrivono le forme
			Paolini ha appena guardato malissimo due tizi che sono entrati dieci minuti in ritardo lol
			Non è stabilito quale tra raster e vettoriale occupi meno spazio
			"Sì qua ho fatto dei... pasticci" -L. Paolini
		Come si rappresenta il suono?
		
			Il suono è rappresentano da un'onda
			Se prendiamo dei timing sufficientemente ravvicinati non ci accorgiamo di questi timing
			Alcuni formati audio:
				- .wav
				- .mid
				
		Formati video
			Diapositive: se prendete delle foto e le fate passare abbastanza velocemente vedete un susseguirsi delle immagini, non le vedete passare singolarmente
			Il video funziona nello stesso modo. Però ha detto una cavolata, che milione in qualche secondo. Solitamente per i film e le animazioni si usano 24fps
				Con un milione di fotogrammi per un'animazione a 24fps così ottieniamo oltre 11 ore di video lol.
		
		Rappresentazione dei numeri nei vari sistemi o qualcosa del genere non ho ben capito cosa vuole fare (forse è un titolo troppo lungo per un paragrafo)
			375 (decimale) è composto da centinaia, decine e unità.
				3 * 10^2 + 7 * 10^1 + 5 * 10^0
			1011 (binario)
				1 * 2^3 + 0 * 2^2 + 1 * 2^1 + 2 * 2^0 = 11
				Annotazione: mostrare un metodo di calcolo senza spiegare perché funziona è una tecnica di insegnamento inefficace
				SETTIMANA PROSSIMA NON C'È PAOLINI ho provato un certo piacere fisico
				"Se non muoio probabilmente il problema non è poi così importante" L. Paolini
				
			Come convertire da decimale a binario:
				Dividere per due e calcolare il resto
				es. 21
					21 / 2 = 10 + 1
					10 / 2 = 5 + 0
					5 / 2 = 2 + 1
					2 / 2 = 1 + 0
					1 / 2 = 0 + 1
					Il risultato va letto dal basso verso l'alto ed è 10101
					
					22
					22 / 2 = 11 + 0
					11 / 2 = 5 + 1
					5 / 2 = 2 + 1
					2 / 2 = 1 + 0
					1 / 2 = 0 + 1
					Il risultato è 10110
					
			Somma tra numeri binari:
				Fondamentalmente immaginate di dover fare un'operazione di AND a tre bit (che è un ottimo metodo per fare un sommatore di numeri binari e funziona anche con la redstone)
				
				0000000 +    <-- operatore di riporto
				0101101 +    <-- primo operatore
				0010110 =    <-- secondo operatore
				-------
				1000011      <-- risultato
				
				L'operatore di riporto è un operatore immaginario/mentale che è utile per ricordarsi il riporto per chi è alle prime armi con le addizioni in binario.
				È importante ricordare che 1 + 1 = 10
				
			Convertire da binario con virgola a decimale con virgola
				101.01
				101 non è un problema (vedi: Come convertire da decimale a binario)
				.01 --> + 0 * 2^-1 + 1 * 2^-2
				101.01 = 5 + 1/4 = 5.25
				
			Convertire da decimale con virgola a binario con virgola
				9.275
				Prima di tutto si trasforma il 9: 1001
				Per il 275 si moltiplica
				0.275 * 2 = 0.550
				0.550 * 2 = 1.10
				0.10 * 2 = 0.20
				0.20 * 2 = 0.40
				0.80 * 2 = 1.60
				0.60 * 2 = 1.20
				0.20 * 2 = 0.40
				0.40 * 2 = 0.80
				...
				(viene un numero periodico)
				Per la parte decimale si leggono i numeri dall'alto verso il basso
				--> 1001.01001100(1100110011001100110011...)
### Lezione 4 (2024/09/25)
		"Chi ha voglia di chiacchierare per cortesia vada altrove" grazie di ignorare i 10 minuti di pausa e pensare che in un minuto tutti riprendano la concentrazione
			Ripetuto tre volte, pergiunta
		Sul sito MOODLE sta iniziando a pubblicare cose --> fare esercizi eccetera direi
		"È abbastanza fastidioso avere persone che vanno avanti e indietro durante le lezioni" è appena finita la pausa bro eddai
		Nella scorsa lezione abbiamo visto come fare le conversioni da binario a decimale e viceversa e così via
			Sta proponendo così spesso il tool che secondo me l'ha creato lui e ci guadagna
			"Fortunatamente non mi sono sbagliato... Cioè non ho fatto la mia brutta figura"
				My man sbagliare è normale, dont you worry <3
			Sta facendo un ulteriore esempio, boh lo scrivo che è meglio che stare su Steam I guess
				9.35
					9/2=4+1
					4/2=2+0
					2/2=1+0
					1/2=0+1
						1001b = 9d
					0.35*2=0.7
					0.7*2=1.4
					0.4*2=0.8
					0.8*2=1.6
					0.6*2=1.2
					0.2*2=0.4
					-->0.8-->1.6-->1.2-->0.4
						.0101100(11001100110011...)b = .35d
					--> 1001.0101100(110011001100...)b = 9.35d
					nb: b accanto a un numero è usato per indicare un numero binario, d per indicare un numero decimale
				Ma perché ora sta parlando di programmazione? Mazzei sei tu?
					--> ha detto che double x = 9 / 2 in C non assegna 4.5 a x perché è un'operazione tra due interi
						Si può effettuare un casting per ottenere 4.5 nel seguente modo: double x = (double)9 / (double)2
		Nuovi argomenti:
		Numeri binari con segno (two's complement notation o notazione complemento a due)
		
			    10011011 +
			    11111111
			    --------
			   110011010
			   
			Problema con sopra: otteniamo un overflow, cioè il risultato occupa più bit degli addendi
			Il complemento a due sfrutta l'overflow
			Il complemento è un'operazione in cui invertiamo ciascun bit
				esempio:
					Il complemento 10101111 è 01010000
				Il complemento a due di un numero è quel numero che, sommato al primo numero, ci fa ottenere 000
				Cerco di parafrasare Paolini:
					-  Stabiliamo un numero binario, detto "A".
					-  Il complemento di A è A' ("A primo").
					-  Il complemento a due di A è A'+1.
					-  A + A' + 1 = 0
				Il libro suggerisce un'ulteriore tecnica, ma non ho fatto in tempo a segnarla.
				Alcuni dei più grandi buchi nella sicurezza della storia sono stati provocati da errori di overflow
				Il bit più significativo dei numeri negativi è il -1
				Lo 0 è incluso nei positivi, quindi i negativi vanno da -1 a -4 e i positivi vanno da 0 a 3
				Il complemento a due di un numero senza sapere quanti bit ci sono è impossibile da fare
				Il libro parla di una "excess notation" MA NON È NOTAZIONE A 3
					Esiste "eccesso a 3" ma non è la stessa cosa
					Le notazioni in eccesso sono notazioni alternative per la rappresentazione dei numeri
						Trasformare 5d in eccesso 8:
							5d + 8 = 13d
							Convertire su 4 bit
							13/2=6+1
							6/2=3+0
							3/2=1+1
							1/2=0+1
								1101
						Trasformare -3d in eccesso 8:
							-3d + 8 = 5d
							5/2=2+1
							2/2=1+0
							1/2=0+1
								0101 (lo 0 più significativo dobbiamo aggiungerlo noi)
						Tabella che rappresenta i valori in eccesso 8:
						- nb(è possibile verificare che 5 e -3 convertiti col metodo spiegato sopra rispettano i valori della tabella sottostante)
							--------------------------
							    Bit		 |	  Value
							  Pattern	 | Represented
							---------------------------
								1111	 |		+7
							---------------------------
								1110	 |		+6
							---------------------------
								1101	 |		+5
							---------------------------
								1100	 |		+4
							---------------------------
								1011	 |		+3
							---------------------------
								1010	 |		+2
							---------------------------
								1001	 |		+1
							---------------------------
								1000	 |		+0
							---------------------------
								0111	 |		-1
							---------------------------
								0110	 |		-2
							---------------------------
								0101	 |		-3
							---------------------------
								0100	 |		-4
							---------------------------
								0011	 |		-5
							---------------------------
								0010	 |		-6
							---------------------------
								0001	 |		-7
							---------------------------
								0000	 |		-8
							---------------------------
			
			Virgola mobile:
				"Chi di voi ha un milione di euro sul conto? Eh, beati voi" -L. Paolini
				"Quanti di voi con un milione di euro controllano i centesimi sul conto? (Io! Io sempre!) Eh va beh, genovesi?" -L. Paolini
				L'idea è di spostare la virgola per ottenere la precisione necessaria.
					Per esempio, se abbiamo un numero grandissimo non ci interessa la parte decimale. Se invece non abbiamo una parte intera, spostiamo la virgola per ottenere un numero più preciso
				Su 8 bit abbiamo:
					- Un segno (1 bit)
					- Un esponente (3 bit)
					- Una mantissa (4 bit)
				Non nel libro: ha menzionato dei dettagli di ottimizzazione
					- Solitamente per il floating point chiedono in eccesso 4. In eccesso 8 l'hanno chiesto ma non per il floating point.
					- Sfrutta un trucchetto sui valori subito prima e dopo la virgola per ottimizzare ulteriornmente lo spazio occupato dal numero
---

Convertitore (più complesso però) che mostra la conversione in floating point con segno, esponente e mantissa messi in evidenza					
https://www.h-schmidt.net/FloatConverter/IEEE754.html

---
				Noi normalmente tronchiamo i nostri numeri al numero di bit disponibili.
					Così facendo si perde una piccola parte di informazione
				Ci sono esercizi nella prima parte del libro
				Notare che nel capitolo 5 del libro (seconda parte) parla di number theory
				A fine capitolo 5 ci sono anche esercizi con domande ed esercizi numerici con le soluzioni
					Le soluzioni degli esercizi in blu sono spiegati molto bene, per quelli in nero ci sono solo le soluzioni
