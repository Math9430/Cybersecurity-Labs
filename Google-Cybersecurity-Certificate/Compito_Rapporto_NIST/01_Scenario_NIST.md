# Scenario – Piano di Sicurezza basato sul NIST CSF

Sei un analista della cybersicurezza che lavora per un’azienda multimediale che offre servizi di web design, graphic design e soluzioni di marketing sui social media per piccole imprese. La tua organizzazione ha recentemente subito un attacco DDoS che ha compromesso la rete interna per due ore prima di essere risolto.

Durante l’attacco, i servizi di rete dell’organizzazione hanno smesso improvvisamente di rispondere a causa di un flusso in entrata di pacchetti ICMP. Il traffico interno normale non riusciva ad accedere a nessuna risorsa di rete. Il team di gestione degli incidenti è intervenuto bloccando i pacchetti ICMP in entrata, mettendo offline tutti i servizi non critici e ripristinando i servizi di rete critici.

Successivamente, il team di cybersicurezza ha indagato sull’incidente e ha scoperto che un attore malevolo aveva inviato un flood di richieste ICMP (ping) nella rete aziendale attraverso un firewall non configurato. Questa vulnerabilità ha permesso all’attaccante di sovraccaricare la rete aziendale con un attacco DDoS (Distributed Denial of Service).

Per affrontare questo evento di sicurezza, il team ha implementato:
- Una nuova regola del firewall per limitare il tasso di pacchetti ICMP in arrivo
- Una verifica dell’indirizzo IP di origine sul firewall per rilevare IP contraffatti nei pacchetti ICMP
- Un software di monitoraggio della rete per rilevare schemi di traffico anomali
- Un sistema IDS/IPS per filtrare parte del traffico ICMP in base a caratteristiche sospette

---

## 🛠 Obiettivo del compito

Come analista della cybersicurezza, il tuo compito è usare questo evento di sicurezza per creare un piano di miglioramento della sicurezza di rete della tua azienda, seguendo il **Cybersecurity Framework (CSF)** del **NIST**.  
Utilizzerai il CSF per guidarti attraverso le diverse fasi dell’analisi dell’incidente e integrarla in una strategia di sicurezza generale.

---

## 📌 Linee guida (NIST CSF)

Il tuo piano dovrà articolarsi secondo le 5 funzioni principali del NIST CSF:

### 1. **Identify**
- Riconoscere i rischi per la sicurezza attraverso audit regolari delle reti, dei sistemi, dei dispositivi e dei privilegi di accesso.

### 2. **Protect**
- Proteggere le risorse interne tramite politiche, procedure, formazione e strumenti che mitigano le minacce.

### 3. **Detect**
- Rilevare potenziali incidenti di sicurezza e rafforzare la capacità di monitoraggio.

### 4. **Respond**
- Contenere, neutralizzare e analizzare gli incidenti; migliorare il processo di risposta.

### 5. **Recover**
- Recuperare i sistemi colpiti e ripristinare i dati e le risorse compromesse.

---

🧠 **Nota:** Questo scenario è pensato per sviluppare capacità di analisi strategica e operativa in ambito difensivo. L’approccio strutturato secondo il NIST CSF ti aiuterà a formalizzare piani di risposta a incidenti reali.
