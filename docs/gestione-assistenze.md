---
title: Gestione assistenze
nav_order: 30
parent: PagoPA, professionisti e assistenze
description: Come leggere le richieste di assistenza tecnica inviate dai professionisti all'Ente e come rispondere, nel portale e via mail
keywords: [assistenza tecnica, richieste di assistenza, rispondere al professionista, risposta, ticket, mail, descrizione del problema, richiedente, supporto]
IDRegione: 99
IDTipoPratica: 9999
Fonte: Manuale Enti
---

# Gestione assistenze

Questa sezione spiega come leggere le richieste di assistenza tecnica che i professionisti inviano dal portale e come rispondere.

{: .note }
> Le richieste di assistenza sono gestite **dall'assistenza SISCOM** di GeoTecSUE, quindi raramente troverai richieste aperte in questa pagina. Se è necessario coinvolgere l'Ente nella richiesta di un professionista, l'assistenza SISCOM vi contatta telefonicamente.

## Accedere alla pagina

Clicca sulla voce **Gestione Assistenze** nella barra di menu in alto.

La pagina si intitola **Assistenza tecnica** e contiene il riquadro **Richieste di assistenza in attesa di risposta**. Accanto al titolo un badge grigio indica quante richieste aspettano una risposta.

## Da dove arrivano le richieste

Il professionista invia la richiesta dal proprio portale, dal menu personale **Assistenza tecnica**. Nel modulo indica:

- **Cognome**, **Nome**, **Email** e **Telefono** (precompilati dal suo profilo, ma modificabili);
- la **Descrizione del problema**;
- se vuole ricevere la risposta anche via mail (casella **Invia la risposta anche via mail**).

Il professionista legge poi la risposta nel portale, nella sezione **Le mie richieste** della sua pagina di assistenza, e, se lo ha chiesto, anche via mail.

## L'elenco delle richieste

Nell'elenco compaiono **solo** le richieste del tuo Ente che non hanno ancora ricevuto risposta. Quando rispondi, la richiesta esce dall'elenco.

L'elenco è una tabella con ricerca, ordinamento e paginazione (vedi [Interfaccia e convenzioni](interfaccia-e-convenzioni.html)). All'apertura è ordinato per data di invio, dalla **più vecchia**: in cima trovi le richieste che aspettano da più tempo.

| Colonna | Contenuto |
|---------|-----------|
| **Inviata il** | Data e ora di invio (gg/mm/aaaa hh:mm) |
| **#** | Numero della richiesta |
| **Richiedente** | Cognome e nome del professionista e, sotto, il suo indirizzo e-mail |
| **Descrizione del problema** | Le prime due righe del testo; passa con il mouse sopra per leggerlo tutto |
| *(senza titolo)* | Pulsante **Rispondi** |

Il campo **Cerca** trova le richieste anche per indirizzo e-mail e per il testo della descrizione.

Se non ci sono richieste in attesa compare il messaggio "Nessuna richiesta di assistenza in attesa di risposta.".

{: .note }
> A differenza di altri elenchi del back office, questa tabella non ricorda ricerca e ordinamento: ogni volta che apri la pagina riparte dalla richiesta più vecchia.

## Rispondere a una richiesta

1. Clicca su **Rispondi** nella riga della richiesta.
2. Si apre la finestra **Richiesta di assistenza #** seguita dal numero. In alto trovi:
   - **Richiedente**;
   - **E-mail** (clicca sull'indirizzo per scrivere al professionista con il tuo programma di posta);
   - **Telefono**;
   - **Inviata il**;
   - **Descrizione del problema**, con il testo completo.
3. Leggi la riga sotto il campo di risposta:
   - "Il professionista ha chiesto di ricevere la risposta anche via mail." oppure
   - "La risposta sarà visibile al professionista nel portale."
4. Scrivi il testo nel campo **Risposta** (obbligatorio).
5. Clicca su **Invia risposta**. Per chiudere senza inviare clicca su **Annulla**.

Se il campo **Risposta** è vuoto, nella finestra compare in rosso "Scrivi la risposta prima di inviarla." e la risposta non viene inviata.

Se chiudi la finestra e la riapri sulla stessa richiesta, il testo già scritto resta; se apri un'altra richiesta, il campo riparte vuoto.

### Dopo l'invio

La pagina si ricarica, la richiesta esce dall'elenco e compare la notifica verde **Risposta inviata (richiesta #…)** con uno di questi dettagli:

| Dettaglio della notifica | Significato |
|--------------------------|-------------|
| "Il professionista la vede nel portale." | Il professionista non aveva chiesto la mail: la risposta è visibile solo nel portale |
| "Inviata anche via mail a …" | La risposta è visibile nel portale ed è stata spedita anche all'indirizzo indicato |
| "Attenzione: la mail al professionista non è stata inviata, la risposta è comunque visibile nel portale." | La risposta è stata registrata, ma la mail non è partita (ad esempio perché il professionista non aveva indicato un indirizzo) |

La mail al professionista ha come oggetto **GeotecSUE: Assistenza Tecnica #** seguito dal numero della richiesta.

{: .warning }
> Ogni richiesta riceve **una sola risposta** e, una volta inviata, non si può modificare né annullare dalla pagina. Se il professionista ha chiesto la mail, la risposta gli arriva subito anche per posta. Rileggi il testo prima di cliccare su **Invia risposta**.

{: .note }
> Se la mail non è partita, la risposta resta comunque disponibile al professionista nel portale. Se vuoi avvisarlo, puoi scrivergli direttamente usando l'indirizzo e-mail della richiesta o quello presente in [Gestione professionisti](gestione-professionisti.html).

## Messaggi di errore

| Messaggio | Dove compare | Quando |
|-----------|--------------|--------|
| "Scrivi la risposta prima di inviarla." | Nella finestra di risposta | Il campo **Risposta** è vuoto |
| "Non è stato possibile registrare la risposta. Riprova." | Nella finestra di risposta | La risposta non è stata salvata |
| "Errore API: …" | Nella finestra di risposta | Il servizio ha restituito un errore durante l'invio |
| "Richiesta di assistenza non trovata: ricarica la pagina." | Finestra **Attenzione** | La richiesta non è più disponibile |
| "A questa richiesta è già stata data una risposta: ricarica la pagina." | Finestra **Attenzione** | Un collega ha già risposto nel frattempo |
| "Si è verificato un errore durante la lettura/elaborazione dei dati" | Finestra **Attenzione** o finestra di risposta | Errore generico |

Quando l'errore compare nella finestra di risposta, la finestra si riapre da sola con il testo che avevi scritto: non devi riscriverlo.

## Cosa può chiedere il professionista all'Ente

Anche queste richieste arrivano in prima battuta all'assistenza SISCOM, ma alcune riguardano decisioni che spettano **solo all'Ente**: in questi casi l'assistenza SISCOM non può decidere al posto vostro e vi coinvolge. Le più frequenti:

| Richiesta | Dove intervieni |
|-----------|-----------------|
| Rendere facoltativo un pagamento obbligatorio che blocca l'invio | [Gestione PagoPA](gestione-pagopa.html) |
| Voltura della pratica ad altro professionista | [Dettaglio della pratica](dettaglio-pratica.html) |
| Importare una pratica presentata prima di GeoTecSUE | [Richieste di importazione](richieste-importazione.html) |

{: .warning }
> In particolare, rendere facoltativo un pagamento obbligatorio è una decisione dell'Ente: l'assistenza SISCOM non può farlo in autonomia (vedi [Gestione PagoPA](gestione-pagopa.html#perche-questa-pagina-e-importante)).
