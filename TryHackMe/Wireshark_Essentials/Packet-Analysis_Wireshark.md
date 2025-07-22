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

![Wireshark2-ezgif com-video-to-gif-converter](https://github.com/user-attachments/assets/4200ca8f-8e26-479f-a9bd-7fff57a46947)

---

### 🖼️ Esportare immagine e calcolare hash MD5  
Dal pacchetto 12 si legge un commento che rimanda a un altro pacchetto contenente un'immagine. L'immagine viene esportata e l’hash calcolato con il comando `md5sum`.

![Wireshark3-ezgif com-video-to-gif-converter](https://github.com/user-attachments/assets/5c3b87db-9aee-433c-af2c-f645878b82ca)

![Wireshark3-2-ezgif com-video-to-gif-converter](https://github.com/user-attachments/assets/dff7673f-1b03-428a-9e5e-4e07649db760)

![Wireshark3-3-ezgif com-video-to-gif-converter](https://github.com/user-attachments/assets/09376344-bf36-42cf-9d5b-6384f0f03875)

---

### 👽 Trovare il file `.txt` e identificare il nome dell’alieno  
Ispezione della cattura per individuare un file `.txt` contenente il nome di un alieno.

![Wireshark4-ezgif com-video-to-gif-converter](https://github.com/user-attachments/assets/c822cb32-247e-4c93-a8b7-c4ce4093680d)

---

### 🌐 Lettura stream HTTP e identificazione artista  
Analisi del pacchetto 33790 e visualizzazione dello **stream HTTP** per determinare il **numero di artisti** e identificare il **secondo artista** nella risposta del server.

![Wireshark5-1-ezgif com-video-to-gif-converter](https://github.com/user-attachments/assets/40ce0257-c260-4162-887f-75b13fb6d7d4)

![Wireshark5-2-ezgif com-video-to-gif-converter](https://github.com/user-attachments/assets/fde70961-dd16-4df7-88e3-02db11d49936)

---

## ✂️ Nota sulla Selezione degli Esercizi  
Sono stati riportati solo gli esercizi più significativi. Alcuni passaggi più semplici sono stati omessi per motivi logistici e di ottimizzazione della documentazione.

---

## 🎓 Collegamento con Esperienze Pregresse  
Tutti gli strumenti trattati in questa sezione sono già stati approfonditi durante il percorso formativo del **Google Cybersecurity Certificate**, che ha fornito le basi teoriche necessarie per comprenderne l’utilizzo in contesti reali.
