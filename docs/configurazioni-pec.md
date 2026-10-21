---
title: Configurazioni PEC
nav_order: 120
parent: "Impostazioni dell'Ente"
description: Spiega come configurare la casella di Posta Elettronica Certificata dell'Ente, verificarla con un messaggio di prova ed eventualmente eliminarla.
keywords: [PEC, posta elettronica certificata, casella PEC, SMTP, porta, crittografia, SSL, TLS, messaggio di prova, notifiche]
IDRegione: 99
IDTipoPratica: 9999
Fonte: Manuale Enti
---

# Configurazioni PEC

Questa sezione spiega come configurare la casella di Posta Elettronica Certificata (PEC) dell'Ente, cioè la casella da cui GeoTecSUE invia le notifiche via PEC ai professionisti.

La casella configurata qui viene usata quando, nella [Scheda Ente](scheda-ente.html), il campo **Tipo notifica** è impostato su **PEC** oppure su **Entrambe**. In questi casi le notifiche ai professionisti (ad esempio la protocollazione di una pratica) partono, oltre o invece della mail normale, dalla casella PEC dell'Ente verso l'indirizzo PEC del professionista.

{: .note }
> Ogni Ente ha **una sola** casella PEC. La pagina mostra sempre la configurazione corrente: se non ne esiste ancora una, i campi sono vuoti e salvando la crei.

## Accedere alla pagina

Dal menu in alto scegli **Impostazioni › Configurazioni PEC**.

La pagina si intitola **Configurazione Posta Elettronica Certificata** e contiene un'unica scheda, **Casella PEC dell'ente**.

{: .schermata }
> `assets/images/configurazioni-pec-panoramica.png` — La scheda "Casella PEC dell'ente" compilata, con il badge "Configurata" e i pulsanti in basso.

## Stato della configurazione

Accanto al titolo della scheda un badge indica lo stato:

| Badge | Significato |
|-------|-------------|
| **Configurata** (verde) | La casella PEC è stata salvata. Sono disponibili il messaggio di prova ed eventualmente l'eliminazione. |
| **Non configurata** (grigio) | Non esiste ancora una casella PEC per l'Ente. Compila i campi e salva. |

Se la casella è usata per l'invio delle notifiche (campo **Tipo notifica** della Scheda Ente impostato su **PEC** o **Entrambe**), sotto il titolo compare il messaggio *"La casella è usata per l'invio delle notifiche, per questo non si può eliminare."* e il pulsante **Elimina** non è visibile.

## Campi della scheda

I campi sono raggruppati in tre sezioni. I campi con l'asterisco rosso sono obbligatori.

### Casella

| Campo | Obbligatorio | Descrizione |
|-------|--------------|-------------|
| **Descrizione** | Sì | Nome descrittivo della casella, ad uso interno (es. "PEC Ufficio Tecnico"). |
| **Indirizzo PEC** | Sì | Indirizzo della casella PEC dell'Ente. È l'indirizzo che compare come mittente delle PEC inviate. Deve contenere il carattere `@`. |

### Server di invio (SMTP)

Questi dati sono forniti dal gestore della casella PEC (ad esempio nelle istruzioni per configurare un programma di posta).

| Campo | Obbligatorio | Descrizione |
|-------|--------------|-------------|
| **Server SMTP** | Sì | Indirizzo del server di posta in uscita del gestore PEC (es. `smtps.pec.aruba.it`). |
| **Porta** | Sì | Porta del server SMTP: un numero da 1 a 65535 (comunemente 465 o 587, secondo le indicazioni del gestore). |
| **Crittografia** | No | **SSL/TLS** (predefinito) oppure **TLS 1.2**. Scegli **TLS 1.2** se il gestore richiede esplicitamente questo protocollo. |
| **SSL** | No | Interruttore che indica l'uso di una connessione protetta SSL. <!-- DA VERIFICARE: l'interruttore SSL viene salvato ma l'invio delle PEC sembra basarsi solo su "SSL implicito" e "Crittografia" --> |
| **SSL implicito** | No | Accendilo se il server richiede una connessione cifrata fin dall'inizio (tipico della porta 465). Spento, la connessione viene cifrata dopo l'apertura (tipico della porta 587). |

### Credenziali

| Campo | Obbligatorio | Descrizione |
|-------|--------------|-------------|
| **Nome utente** | Sì | Nome utente con cui accedere alla casella PEC (di solito coincide con l'indirizzo PEC). |
| **Password** | Solo alla prima configurazione | Password della casella PEC. |

Sulla password valgono queste regole:

- La password salvata **non viene mai mostrata** nella pagina. Quando la casella è già configurata, il campo è vuoto e riporta il suggerimento *"Lascia vuoto per non modificarla"*.
- Se lasci il campo vuoto e salvi, la password già memorizzata resta invariata. Scrivi una nuova password solo quando vuoi cambiarla.
- Il pulsante con l'occhio accanto al campo mostra o nasconde i caratteri che stai digitando, per controllare di averli scritti correttamente.

{: .note }
> Se cambi la password della casella presso il gestore PEC, ricordati di aggiornarla anche qui: altrimenti l'invio delle PEC ai professionisti non riuscirà.

## Salvare la configurazione

1. Compila o modifica i campi.
2. Clicca su **Salva** (puoi anche premere Invio in uno dei campi).
3. Se manca un dato obbligatorio o un valore non è valido, compare la finestra **Attenzione** con il motivo, ad esempio:
   - *"Inserire la descrizione."*
   - *"L'indirizzo PEC non è valido."*
   - *"Inserire una porta valida (da 1 a 65535)."*
   - *"Inserire la password."* (solo alla prima configurazione)
4. Se il salvataggio riesce, compare la notifica verde **Impostazioni PEC salvate** con l'indirizzo PEC e il badge diventa **Configurata**.

Per scartare le modifiche non ancora salvate clicca su **Annulla modifiche**: i campi tornano ai valori memorizzati.

Per le convenzioni comuni (notifiche verdi, finestra "Attenzione", spinner) vedi [Interfaccia e convenzioni](interfaccia-e-convenzioni.html).

## Inviare un messaggio di prova

Quando la casella è configurata, in basso compare il pulsante **Invia messaggio di prova**, con l'indicazione del destinatario della prova (*"Con i dati salvati, a …"*).

1. Salva prima eventuali modifiche: la prova usa **i dati salvati**, non quelli che stai digitando.
2. Clicca su **Invia messaggio di prova**.
3. Se l'invio riesce compare la notifica verde **Messaggio di prova inviato**, con mittente e destinatario.
4. Se l'invio non riesce compare la finestra **Attenzione** con il testo *"Invio di prova non riuscito:"* seguito dal messaggio restituito dal server di posta. Il messaggio aiuta a capire il problema (server, porta, credenziali o crittografia errati).

{: .note }
> Il messaggio di prova viene inviato a un indirizzo di verifica predefinito, mostrato accanto al pulsante, e non a una casella dell'Ente. Serve a verificare che i parametri di invio siano corretti.

{: .schermata }
> `assets/images/configurazioni-pec-prova.png` — La parte bassa della scheda con il pulsante "Invia messaggio di prova" e l'indirizzo del destinatario di prova.

## Eliminare la configurazione

Il pulsante **Elimina** è visibile solo se la casella è configurata **e non** è usata per le notifiche. Se nella Scheda Ente il **Tipo notifica** è **PEC** o **Entrambe**, prima imposta **Mail normale** nella [Scheda Ente](scheda-ente.html) e poi torna qui.

1. Clicca su **Elimina**.
2. Si apre la finestra **Eliminare la configurazione PEC?** con l'avviso *"Verranno eliminati i parametri della casella PEC dell'ente. L'operazione non si può annullare."*
3. Clicca su **Elimina** per confermare, oppure su **Annulla** per tornare indietro.
4. Compare la notifica **Configurazione PEC eliminata** e il badge torna **Non configurata**.

{: .warning }
> L'eliminazione è definitiva: per tornare a inviare PEC dovrai reinserire tutti i parametri, compresa la password.

## Legame con la Scheda Ente

Nella [Scheda Ente](scheda-ente.html), il campo **Tipo notifica** accetta **PEC** o **Entrambe** solo se la casella PEC è già configurata: in caso contrario il salvataggio della Scheda Ente segnala *"Necessario configurare i parametri della PEC"* e riporta il valore a **Mail normale**. Configura quindi prima la casella in questa pagina.

Quali eventi generano una notifica al professionista si decide nella pagina [Mail](mail.html).
