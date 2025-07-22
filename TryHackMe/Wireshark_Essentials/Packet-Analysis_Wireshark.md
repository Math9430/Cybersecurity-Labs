# 📡 Analisi di Base con Wireshark

In questa attività è stato utilizzato un file `.pcap` denominato `exercise`, fornito da TryHackMe. Ogni esercizio è stato documentato tramite una GIF che ne mostra visivamente i passaggi principali.

---

## 🎯 Esercizi Svolti

### 🏴 Trovare la flag nel commento del file catturato  
Analisi dei pacchetti alla ricerca di un commento contenente una flag nascosta.

![GIF Flag nel commento](https://github.com/user-attachments/assets/b00dfb64-5528-4d32-b8d0-efc08e846bae)


---

### 🎧 Cercare la stringa “r4w” per identificare il primo artista  
Utilizzo della funzione di ricerca per isolare stringhe testuali e identificare un artista specifico.

![GIF Artista 1 - stringa r4w](<inserisci-percorso-immagine>)

---

### 🖼️ Esportare immagine e calcolare hash MD5  
Dal pacchetto 12 si legge un commento che rimanda a un altro pacchetto contenente un'immagine. L'immagine viene esportata e l’hash calcolato con il comando `md5sum`.

![GIF esportazione immagine e hash](<inserisci-percorso-immagine>)

---

### 👽 Trovare il file `.txt` e identificare il nome dell’alieno  
Ispezione della cattura per individuare un file `.txt` contenente il nome di un alieno.

![GIF alieno - file .txt](<inserisci-percorso-immagine>)

---

### 🌐 Lettura stream HTTP e identificazione artista  
Analisi del pacchetto 33790 e visualizzazione dello **stream HTTP** per determinare il **numero di artisti** e identificare il **secondo artista** nella risposta del server.

![GIF stream HTTP](<inserisci-percorso-immagine>)

---

## ✂️ Nota sulla Selezione degli Esercizi  
Sono stati riportati solo gli esercizi più significativi. Alcuni passaggi più semplici sono stati omessi per motivi logistici e di ottimizzazione della documentazione.

---

## 🎓 Collegamento con Esperienze Pregresse  
Tutti gli strumenti trattati in questa sezione sono già stati approfonditi durante il percorso formativo del **Google Cybersecurity Certificate**, che ha fornito le basi teoriche necessarie per comprenderne l’utilizzo in contesti reali.
