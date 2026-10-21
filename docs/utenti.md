---
title: Gestione utenti
nav_order: 160
parent: "Impostazioni dell'Ente"
description: Spiega come creare, modificare ed eliminare gli utenti in consultazione dell'Ente, con il Comune consultabile e la password di accesso.
keywords: [utenti, utenti in consultazione, gestione utenti, username, password, comune consultabile, tutti i comuni, unione, accesso consultazione]
IDRegione: 99
IDTipoPratica: 9999
Fonte: Manuale Enti
---

# Gestione utenti

Questa sezione spiega come gestire gli **utenti in consultazione** dell'Ente: le credenziali (username e password) con cui una persona può accedere alla consultazione delle pratiche, limitata eventualmente a un solo Comune.

{: .note }
> Gli utenti in consultazione non sono operatori del back office: servono solo per accedere alla consultazione. Le impostazioni di cosa è visibile si trovano nella pagina [Consultazione](consultazione.html).

## Accedere alla pagina

Dal menu in alto scegli **Impostazioni › Gestione Utenti**. La pagina si intitola **Gestione Utenti in Consultazione**.

## Elenco degli utenti

La scheda **Utenti in consultazione** mostra gli utenti dell'Ente; il badge accanto al titolo ne riporta il numero.

{: .schermata }
> `assets/images/utenti-elenco.png` — La scheda "Utenti in consultazione" con alcuni utenti, la colonna "Comune consultabile" e i pulsanti di modifica ed eliminazione.

| Colonna | Contenuto |
|---------|-----------|
| **Username** | Nome utente con cui si accede alla consultazione. |
| **Comune consultabile** | Comune di cui l'utente può consultare le pratiche, oppure il badge blu **Tutti i comuni**. Visibile solo se l'Ente gestisce più Comuni (ad esempio un'Unione). |
| (pulsanti) | **Modifica** (matita): modifica l'utente o cambia la password. **Elimina** (cestino): elimina l'utente. |

L'elenco è ordinato per username e ha **Cerca**, ordinamento e paginazione da 25 righe: vedi [Interfaccia e convenzioni](interfaccia-e-convenzioni.html). Se non ci sono utenti compare *"Nessun utente in consultazione: usa Nuovo utente per aggiungerne uno."*

## Creare un utente

1. Clicca su **Nuovo utente**.
2. Si apre la finestra **Nuovo utente**.
3. Compila i campi (vedi tabella sotto).
4. Clicca su **Salva** (o premi Invio).
5. Compare la notifica verde **Utente creato** con lo username.

| Campo | Obbligatorio | Descrizione |
|-------|--------------|-------------|
| **Username** | Sì | Nome utente. Deve essere unico nell'Ente. Dopo la creazione non si può più modificare. |
| **Comune consultabile** | — | Solo per gli Enti con più Comuni. Scegli **Tutti i comuni** oppure un singolo Comune. Negli Enti con un solo Comune il campo non compare e l'utente è associato al Comune dell'Ente. |
| **Password** | Sì | Almeno 8 caratteri. Gli spazi all'inizio e alla fine vengono ignorati. |
| **Conferma password** | Sì | Ripeti la password: deve coincidere con la precedente. |

Il pulsante con l'occhio accanto alla password mostra o nasconde entrambe le password digitate.

{: .note }
> La password non viene mai mostrata dopo il salvataggio. Comunicala all'utente in modo sicuro al momento della creazione.

## Modificare un utente o cambiarne la password

1. Clicca sulla matita nella riga dell'utente.
2. Si apre la finestra **Modifica utente**. Lo **Username** è visibile ma non modificabile.
3. Se l'Ente ha più Comuni, puoi cambiare il **Comune consultabile**.
4. Per cambiare la password, compila **Nuova password** e **Conferma password**. Per mantenere quella attuale lascia entrambi i campi vuoti.
5. Clicca su **Salva**.
6. Compare la notifica **Utente salvato** oppure **Utente salvato, password cambiata**.

## Messaggi di errore

Se qualcosa non va compare la finestra **Attenzione**; chiudendola si torna alla finestra dell'utente con i dati inseriti.

| Messaggio | Causa |
|-----------|-------|
| *"Inserire lo username."* | Username vuoto (nuovo utente). |
| *"Inserire la password."* | Password vuota (nuovo utente). |
| *"La password deve avere almeno 8 caratteri."* | Password troppo corta. |
| *"Le due password non coincidono."* | **Password** e **Conferma password** sono diverse. |
| *"Username già presente."* | Esiste già un utente dell'Ente con quello username. |

## Eliminare un utente

1. Clicca sul cestino nella riga dell'utente.
2. Si apre la finestra **Eliminare l'utente?** con lo username e l'avviso *"Non potrà più accedere alla consultazione."*
3. Clicca su **Elimina** per confermare, oppure su **Annulla**.
4. Compare la notifica **Utente eliminato**.

{: .warning }
> L'eliminazione è definitiva: per ridare l'accesso alla persona dovrai creare un nuovo utente.
