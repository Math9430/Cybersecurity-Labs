# 🛡️ Report di Analisi – Incidente di Sicurezza: Brute Force su YummyRecipesForMe.com

## 🧩 Descrizione dell’Incidente
Il sito web *yummyrecipesforme.com* è stato compromesso da un ex dipendente tramite un attacco **brute force** sull’account amministratore. La password era rimasta quella predefinita, e l’assenza di misure di protezione ha permesso all’attaccante di ottenere l’accesso completo al backend del sito.

Una volta dentro, l’hacker ha inserito codice JavaScript malevolo nel sito, forzando il download di un file .exe contenente malware. Gli utenti che lo hanno eseguito sono stati reindirizzati automaticamente a un sito fasullo, *greatrecipesforme.com*, che ospitava il contenuto dannoso.

## 🧪 Azioni Intrusion Detection & Analisi
È stato creato un ambiente sandbox per simulare l’accesso al sito. Le attività sono state monitorate con `tcpdump`.

### 🔄 Flusso dell’attacco (riassunto tecnico)
1. **Risoluzione DNS** per *yummyrecipesforme.com*
2. **Connessione HTTP** al sito
3. **Download automatico** del file eseguibile
4. **Esecuzione del file** da parte dell’utente (in sandbox)
5. **Risoluzione DNS** per *greatrecipesforme.com*
6. **Redirect automatico** al sito clone infetto

I log catturati confermano la catena di eventi e dimostrano un comportamento coerente con compromissione e distribuzione di malware.

## 🛠️ Protocolli di Rete Utilizzati
- **DNS (Porta 53)**: per la risoluzione degli indirizzi IP
- **HTTP (Porta 80)**: per la comunicazione client-server non cifrata

> Nessuna traccia di HTTPS: un segnale chiaro di mancata implementazione di sicurezza base.

---

## 🚨 Cause dell’Incidente
- **Password amministratore predefinita**
- **Assenza di sistemi di protezione brute-force (rate limiting, captcha, 2FA)**
- **Assenza di crittografia del traffico (niente HTTPS)**
- **Codice lato client non validato**

---

## ✅ Raccomandazioni di Sicurezza
- **Modifica immediata di tutte le credenziali** (evitare password predefinite)
- **Implementazione di sistemi di protezione da brute force**: blocchi IP dopo tentativi falliti, autenticazione a più fattori
- **Passaggio obbligatorio a HTTPS con certificati validi**
- **Codice JavaScript sottoposto a revisione e firma digitale**
- **Monitoraggio continuo del sito tramite strumenti IDS/IPS**
- **Backup regolari del sito web**

---

## 👨‍💻 Conclusione
L'incidente è un classico esempio di attacco evitabile con misure minime di cybersecurity. Questo caso mostra l'importanza della **proattività** nella protezione degli asset digitali e il rischio che deriva da configurazioni deboli o trascurate.
