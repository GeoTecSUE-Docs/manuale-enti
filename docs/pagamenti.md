---
title: Pagamenti
nav_order: 20
parent: "Impostazioni dell'Ente"
description: Come gestire le schede informative sui pagamenti e sui diritti di segreteria dell'Ente, con testo in formato Markdown, allegati, priorità e attivazione.
keywords: [pagamenti, diritti di segreteria, tariffe, informazioni, markdown, allegati, priorità, attivazione, eliminazione, professionisti]
IDRegione: 99
IDTipoPratica: 9999
Fonte: Manuale Enti
---

# Pagamenti

Questa sezione spiega come gestire le schede informative sui pagamenti dell'Ente (ad esempio i diritti di segreteria): crearle, scriverne il testo, allegare documenti, attivarle o disattivarle ed eliminarle.

## A cosa serve

In questa pagina l'Ente pubblica **informazioni testuali** sui pagamenti: ogni scheda ha un titolo, un testo formattato ed eventuali allegati (ad esempio la delibera delle tariffe o le istruzioni per il versamento).

{: .note }
> Questa pagina **non** configura gli importi né i pagamenti PagoPA richiesti nelle pratiche. Per stabilire quali pagamenti il professionista deve effettuare, e con quale importo, usa [Configurazione PagoPA](pagopa-configurazione.html).

Dal punto di vista del professionista, le schede **attive** sono consultabili sul portale dei professionisti come informazioni sui pagamenti dovuti all'Ente; quelle con **Priorità** attiva sono messe in evidenza.

## Accedere alla pagina

Dal menu in alto scegli **Impostazioni › Pagamenti**.

Si apre la pagina **Gestione Pagamenti** con l'elenco delle schede dell'Ente.

{: .schermata }
> `assets/images/pagamenti-elenco.png` — La pagina Gestione Pagamenti con l'elenco delle schede, i badge Priorità e Attiva e i pulsanti di modifica ed eliminazione.

## Elenco dei pagamenti

L'elenco mostra 10 schede per pagina; per scorrere le pagine usa i numeri e le frecce **<<** e **>>** sotto la tabella. Questo elenco non ha la casella **Cerca** e non si ordina cliccando sulle colonne.

Se non ci sono schede, al posto della tabella compare il messaggio **Nessun pagamento presente**.

| Colonna | Contenuto |
|---------|-----------|
| **Inserimento** | Data di inserimento |
| **Titolo** | Titolo della scheda |
| **Testo** | Inizio del testo, senza formattazione. Passa con il mouse sopra il testo per leggerne una parte più lunga |
| **Priorità** | Badge **Sì** (giallo) o **No** (grigio) cliccabile |
| **Attiva** | Badge **Sì** (verde) o **No** (grigio) cliccabile |
| **Azioni** | Matita (modifica) e cestino (elimina) |

### Attivare o disattivare una scheda

1. Clicca sul badge nella colonna **Attiva**.
2. Il valore passa da **Sì** a **No** o viceversa e la modifica viene salvata subito.

Compare la notifica **Pagamento attivato** oppure **Pagamento disattivato**.

### Attivare o togliere la priorità

1. Clicca sul badge nella colonna **Priorità**.
2. Il valore passa da **Sì** a **No** o viceversa e la modifica viene salvata subito.

Compare la notifica **Priorità attivata** oppure **Priorità disattivata**.

## Creare una scheda

1. Clicca su **Nuovo pagamento** in alto a destra nell'elenco.
2. Si apre la finestra **Nuovo pagamento**: compila i campi (vedi la tabella sotto).
3. Scrivi il testo nell'editor.
4. Clicca su **Salva**.

La pagina si ricarica e compare la notifica **Pagamento creato**, con l'indicazione che ora puoi aggiungere gli allegati da **Modifica**.

{: .note }
> Gli allegati si possono aggiungere solo a una scheda già salvata: nella finestra **Nuovo pagamento** la sezione **Allegati** mostra il messaggio **Salva il pagamento per poter aggiungere allegati.** Dopo il primo salvataggio, riapri la scheda con la matita per caricare i file.

### Campi della finestra

| Campo | Obbligatorio | Note |
|-------|--------------|------|
| **Titolo** | ✅ | Massimo 200 caratteri |
| **Data di inserimento** | ✅ | Proposta con la data di oggi; puoi cambiarla scrivendola (gg/mm/aaaa) o con il calendario |
| **Priorità** | ❌ | **Sì** / **No** (predefinito **No**) |
| **Attiva** | ❌ | **Sì** / **No** (predefinito **Sì**) |
| **Testo** | ❌ | Testo in formato Markdown, scritto con l'editor |

A differenza delle [News](news.html), qui non c'è la data di fine validità.

Se un controllo non è superato, compare la finestra **Attenzione** con uno di questi messaggi:

| Messaggio | Causa |
|-----------|-------|
| **Necessario inserire una data valida** | Data di inserimento vuota o non valida |
| **Necessario inserire un titolo** | Titolo vuoto |
| **Il titolo non può superare i 200 caratteri** | Titolo troppo lungo |

{: .warning }
> Quando compare un errore la finestra di modifica si chiude e il testo scritto nell'editor non viene conservato. Per i testi lunghi, copia il testo prima di cliccare su **Salva**.

### Scrivere il testo

L'editor del campo **Testo** è lo stesso delle news: barra con **Grassetto**, **Corsivo**, **Titolo**, **Elenco puntato**, **Elenco numerato**, **Citazione**, **Link**, **Linea orizzontale**, **Anteprima**, **Annulla** e **Ripeti**. Per i dettagli vedi [Scrivere il testo](news.html#scrivere-il-testo).

{: .schermata }
> `assets/images/pagamenti-finestra-modifica.png` — La finestra Modifica pagamento con titolo, data, priorità, attivazione, editor del testo e sezione Allegati.

## Modificare una scheda

1. Clicca sulla matita nella colonna **Azioni**.
2. Si apre la finestra **Modifica pagamento** con i dati salvati.
3. Modifica i campi e il testo.
4. Clicca su **Salva**.

Compare la notifica **Pagamento salvato**. Per chiudere senza salvare clicca su **Annulla** o sulla **X**.

## Allegati

La sezione **Allegati** è disponibile nella finestra **Modifica pagamento** e funziona come quella delle news:

1. Scrivi la **Descrizione** del file.
2. In **File** seleziona il documento.
3. Clicca su **Carica**.

Compare la notifica **Allegato caricato** e il file si aggiunge all'elenco. Per ogni allegato puoi usare **Scarica il file** (freccia) o **Elimina il file** (cestino).

{: .warning }
> L'eliminazione di un allegato è immediata e non chiede conferma. Inoltre il caricamento di un allegato ricarica il testo com'era all'ultimo salvataggio: salva prima il testo, poi carica gli allegati.

I messaggi di errore possibili sono gli stessi delle news (**ATTENZIONE ! Descrizione non inserita.**, **ATTENZIONE ! Selezionare il file.**, **ATTENZIONE ! Dimensione del file superiore a … MB.**). Il limite di dimensione è quello impostato nella [Scheda Ente](scheda-ente.html) (**Limite dimensione file**).

## Eliminare una scheda

1. Clicca sul cestino nella colonna **Azioni**.
2. Si apre la finestra **Conferma eliminazione** con il messaggio **Eliminare definitivamente il pagamento (con i suoi allegati):** seguito dal titolo.
3. Clicca su **Elimina** per confermare, oppure su **Annulla**.

Compare la notifica **Pagamento eliminato**.

{: .warning }
> L'eliminazione è definitiva e cancella anche tutti gli allegati della scheda. Se vuoi solo nasconderla, imposta il badge **Attiva** su **No**.

## Messaggi e notifiche

Le notifiche verdi di conferma e la finestra **Attenzione** per gli errori seguono le convenzioni comuni del back office, descritte in [Interfaccia e convenzioni](interfaccia-e-convenzioni.html).
