# Scenario

Durante la giornata lavorativa, il sito web aziendale diventa improvvisamente irraggiungibile. I dipendenti e i clienti ricevono errori di tipo "Gateway Timeout" (504) e non riescono a connettersi al sito.

Un’analisi dei log di rete mostra una quantità anomala di pacchetti TCP SYN provenienti da un singolo indirizzo IP esterno non autorizzato.

Il server risponde con pacchetti SYN-ACK, ma non riceve mai l’ACK finale. Le connessioni incomplete saturano progressivamente le risorse del server, rendendo il sito inaccessibile agli utenti legittimi.

L’attacco viene identificato come un SYN Flood, una tipologia di attacco Denial of Service (DoS) che sfrutta il meccanismo di handshake TCP per interrompere la disponibilità del servizio.

Il team di sicurezza è incaricato di analizzare i log, identificare l’attacco e proporre contromisure efficaci.
