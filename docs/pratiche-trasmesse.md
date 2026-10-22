---
title: Pratiche e comunicazioni trasmesse
nav_order: 10
parent: Gestione pratiche
description: Spiega come consultare e filtrare le pratiche, le comunicazioni e le integrazioni trasmesse dai professionisti all'Ente e come aprirne il dettaglio.
keywords: [pratiche trasmesse, comunicazioni, richieste di integrazione, filtri, stato pratica, numero protocollo, titolare, professionista, elenco pratiche, data di invio]
IDRegione: 99
IDTipoPratica: 9999
Fonte: Manuale Enti
---

# Pratiche e comunicazioni trasmesse

Questa sezione spiega come consultare l'elenco delle pratiche, delle comunicazioni e delle integrazioni che i professionisti hanno trasmesso al tuo Ente, come filtrarle e come aprirne il dettaglio.

Vedi solo le pratiche del tuo Ente.

## Accedere alla pagina

Dal menu in alto scegli **Gestione Pratiche › Pratiche e comunicazioni trasmesse**.

La pagina si intitola **Pratiche e comunicazioni trasmesse** ed è organizzata in tre schede.

{: .schermata }
> `assets/images/pratiche-trasmesse-elenco.png` — La pagina con la scheda Pratiche aperta, la card dei filtri e la tabella con i badge colorati di stato.

## Le schede

| Scheda | Cosa contiene |
|--------|---------------|
| **Pratiche** | Le pratiche (istanze) trasmesse dai professionisti |
| **Comunicazioni** | Le comunicazioni collegate a una pratica già trasmessa (es. inizio lavori, fine lavori) |
| **Richieste di integrazione** | Le pratiche coinvolte in una richiesta di integrazione documentale |

Accanto al nome di ogni scheda trovi:

- un badge blu con il **numero di elementi** trovati;
- un badge giallo con il numero di **filtri attivi** (es. "2 filtri"), solo se hai applicato almeno un filtro.

La scheda aperta viene ricordata: dopo un filtro o al ritorno dal dettaglio di una pratica ritrovi la stessa scheda.

## Filtrare gli elenchi

Ogni scheda ha la sua card dei filtri, indipendente dalle altre. Per le convenzioni comuni (contatore dei filtri, campi data con calendario) vedi [Interfaccia e convenzioni](interfaccia-e-convenzioni.html).

### Filtri della scheda Pratiche

| Filtro | Cosa cerca |
|--------|-----------|
| **Tipo pratica** | Uno dei tipi di pratica attivi per l'Ente (**Tutti** per non filtrare) |
| **Stato pratica** | Uno degli stati di lavorazione (da **Inviata** in poi; **Tutti** per non filtrare) |
| **# Pratica** | Il numero della pratica assegnato da GeoTecSUE |
| **Numero pratica** | Il numero di pratica attribuito dall'Ente |
| **Numero protocollo** | Il numero di protocollo |
| **Titolare** | Il nominativo del titolare |
| **Professionista** | Il nominativo del professionista |
| **Comune** | Solo per gli Enti che gestiscono più Comuni (es. Unioni): il Comune dell'intervento |
| **Data di invio** dal / al | Intervallo della data di trasmissione |
| **Data di protocollo** dal / al | Intervallo della data di protocollo |

### Filtri della scheda Comunicazioni

**Tipo comunicazione**, **# Comunicazione**, **Comune** (solo per gli Enti con più Comuni), **Titolare**, **Professionista** e **Data di invio** dal / al.

### Filtri della scheda Richieste di integrazione

**Tipo pratica**, **Stato pratica**, **# Pratica**, **Titolare**, **Professionista** e **Data di invio** dal / al.

### Applicare e rimuovere i filtri

1. Compila uno o più campi.
2. Clicca su **Filtra** (oppure premi Invio in un campo).
3. Per tornare all'elenco completo clicca su **Rimuovi filtri** (nelle schede Comunicazioni e Richieste di integrazione il pulsante si chiama **Rimuovi**). Il pulsante compare solo quando c'è almeno un filtro attivo.

Le date vanno scritte nel formato gg/mm/aaaa oppure scelte dal calendario. Se una data non è valida, o se la data iniziale è successiva a quella finale, si apre la finestra **Attenzione** con il motivo, ad esempio:

- *La data di invio iniziale «…» non è una data valida: usa il formato gg/mm/aaaa.*
- *Nell'intervallo della data di protocollo la data iniziale è successiva a quella finale.*

{: .note }
> I filtri vengono conservati quando apri il dettaglio di una pratica e torni indietro con **Ritorna**. Se invece riapri la pagina dal menu, i filtri ripartono vuoti.

## Le tabelle

Le tabelle hanno la ricerca libera (**Cerca**), l'ordinamento per colonna e la paginazione (25 righe per pagina). All'apertura sono ordinate per **Data invio**, dalla più recente. Pagina, ordinamento e testo di ricerca vengono ricordati finché il browser resta aperto.

### Colonne della scheda Pratiche

| Colonna | Contenuto |
|---------|-----------|
| **# Pratica** | Numero della pratica; cliccandolo apri il dettaglio |
| **Tipo** | Acronimo del tipo di pratica (passa con il mouse per leggere la descrizione completa) |
| **Comune** | Solo per gli Enti con più Comuni |
| **Data invio** | Data e ora di trasmissione |
| **Titolare** | Titolare della pratica |
| **Professionista** | Professionista che ha trasmesso la pratica |
| **Stato** | Badge colorato con lo stato attuale |
| **Protocollo** | "n. … del …"; la colonna compare solo se almeno una pratica dell'elenco è protocollata |
| (lente) | Apre il dettaglio della pratica |

### Colonne della scheda Comunicazioni

| Colonna | Contenuto |
|---------|-----------|
| **# Comunicazione** | Numero della comunicazione; cliccandolo apri il dettaglio della **pratica a cui la comunicazione si riferisce** |
| **Tipo** | Acronimo del tipo di comunicazione |
| **Comune** | Solo per gli Enti con più Comuni |
| **Data invio** | Data e ora di trasmissione |
| **Professionista** | Professionista che ha trasmesso la comunicazione |
| **Stato** | Badge colorato di stato |
| **# Pratica rif.** | Numero di riferimento <!-- DA VERIFICARE: nel codice questa colonna mostra lo stesso valore di "# Comunicazione"; potrebbe non riportare il numero della pratica di riferimento --> |
| **Tipo pratica rif.** | Tipo della pratica di riferimento (anche quando si tratta di una pratica importata) |
| (lente) | Apre il dettaglio della pratica di riferimento |

Nel dettaglio della pratica la comunicazione si trova nella scheda **Comunicazioni**: vedi [Dettaglio della pratica](dettaglio-pratica.html#scheda-comunicazioni).

### Colonne della scheda Richieste di integrazione

**# Pratica** (link al dettaglio della pratica di riferimento), **Tipo**, **Comune** (solo per gli Enti con più Comuni), **Data invio**, **Titolare**, **Professionista**, **Stato** e la lente per aprire il dettaglio.

### Colori degli stati

| Colore del badge | Stati |
|------------------|-------|
| Arancione | Inviata, Inviata SPRESALWEB (via MUDE) |
| Azzurro | Protocollata |
| Grigio | Registrata |
| Giallo | Richiesta Integrazioni, Richiesta Archiviazione, Invio Integrazioni |
| Verde | Esecutiva, Verificata, Protocollata SPRESALWEB |
| Rosso | Archiviata, Diniego, Rifiutata, Revoca Delegato |

Il significato di ogni stato è spiegato in [Stati delle pratiche](appendici/stati-pratica.html).

## Aprire il dettaglio

1. Clicca sul numero della pratica oppure sulla lente a destra della riga.
2. Si apre la pagina [Dettaglio della pratica](dettaglio-pratica.html).
3. Per tornare all'elenco clicca su **Ritorna**: ritrovi la stessa scheda, gli stessi filtri e la stessa pagina della tabella.

{: .note }
> Le pratiche importate e le notifiche preliminari si aprono nelle rispettive pagine di dettaglio: [Dettaglio pratica importata](dettaglio-importata.html) e [Dettaglio notifica preliminare](dettaglio-notifica-preliminare.html).

## Messaggi di errore

Se il caricamento non riesce compare la finestra **Attenzione** con il messaggio *Si è verificato un errore durante la lettura/elaborazione dei dati* oppure con l'indicazione dell'errore ricevuto dal server. Se la sessione è scaduta vieni riportato alla pagina di accesso (vedi [Accesso al back office](accesso.html)).
