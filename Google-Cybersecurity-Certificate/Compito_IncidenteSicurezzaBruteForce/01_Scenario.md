# 🛡️ Scenario di Sicurezza: Attacco Brute Force su YummyRecipesForMe.com

## Contesto
Sei un analista della sicurezza informatica incaricato di indagare su un incidente presso **YummyRecipesForMe.com**, un sito web che vende ricette e libri di cucina.

## Attacco
Un ex dipendente ha condotto un attacco brute force contro l'host del sito per ottenere l'accesso all'account amministratore, sfruttando una password predefinita mai cambiata.

Una volta entrato:
- Ha modificato il codice sorgente del sito.
- Ha inserito una funzione **JavaScript** che invitava i visitatori a scaricare ed eseguire un file.
- Dopo l'accesso iniziale, ha cambiato la password dell'amministratore.

## Conseguenze
- Il file scaricato reindirizzava gli utenti al sito **greatrecipesforme.com**, contenente **malware**.
- Numerosi utenti hanno segnalato problemi all’assistenza: rallentamenti del PC e cambi improvvisi di URL.

## Indagine
Come parte del team di risposta:
- Hai creato un ambiente **sandbox**.
- Avviato **tcpdump** per analisi del traffico.
- Visitato il sito ed eseguito il file.
- Verificato il comportamento malevolo: reindirizzamento automatico.

## Traffico di rete osservato
1. DNS → yummyrecipesforme.com
2. HTTP → yummyrecipesforme.com
3. Download del malware
4. DNS → greatrecipesforme.com
5. HTTP → greatrecipesforme.com

## Conferme tecniche
- Il codice sorgente include **JavaScript malevolo**.
- Lo script reindirizza l'utente post-download.

## Vulnerabilità identificate
- Password predefinita non modificata
- Assenza di meccanismi anti-brute force (rate limiting, captcha, lockout)

## Obiettivo del Lab
📌 Documentare l’incidente e:
- Identificare i **protocolli di rete** coinvolti
- Raccomandare **misure di sicurezza** per prevenire attacchi simili

---
