---
title: Gestione PagoPA
nav_order: 10
parent: PagoPA, professionisti e assistenze
description: Come consultare i pagamenti PagoPA delle pratiche ancora in compilazione presso i professionisti e come renderli obbligatori o facoltativi
keywords: [PagoPA, pagamenti, IUV, pagamento obbligatorio, pagamento facoltativo, servizio PagoPA, stato del pagamento, pratiche in compilazione, filtri, professionista]
IDRegione: 99
IDTipoPratica: 9999
Fonte: Manuale Enti
---

# Gestione PagoPA

Questa sezione spiega come consultare i pagamenti PagoPA delle pratiche che i professionisti stanno ancora compilando e come decidere, pagamento per pagamento, se è **obbligatorio** o **facoltativo**.

## Accedere alla pagina

Clicca sulla voce **Gestione PagoPA** nella barra di menu in alto.

La pagina si intitola **Gestione PagoPA** e contiene un unico riquadro: **Pagamenti delle pratiche in lavorazione presso i professionisti**.

{: .schermata }
> `assets/images/gestione-pagopa-elenco.png` — La pagina Gestione PagoPA con la card dei filtri compilata e l'elenco dei pagamenti, con i pulsanti Obbligatorio/Facoltativo nella colonna Pagamento.

## Quali pagamenti vedi

Nella pagina compaiono **solo** i pagamenti delle pratiche che il professionista **non ha ancora inviato**, cioè delle pratiche ancora in compilazione. Vedi solo i pagamenti delle pratiche del tuo Ente.

I pagamenti delle pratiche già trasmesse non sono qui: li trovi nel [dettaglio della pratica](dettaglio-pratica.html) (o nel [dettaglio della pratica importata](dettaglio-importata.html)).

Accanto al titolo del riquadro trovi:
- un badge viola con il **numero di pagamenti** trovati;
- un badge giallo con il numero di **filtri attivi** (es. "1 filtro", "3 filtri"), visibile solo se hai impostato almeno un filtro.

Sotto il titolo, un riquadro informativo azzurro ricorda che con il pulsante nella colonna **Pagamento** rendi un pagamento obbligatorio o facoltativo.

{: .note }
> Per l'elenco delle pratiche in compilazione (non solo dei loro pagamenti) usa la pagina [Pratiche in corso](pratiche-in-corso.html). I servizi di pagamento disponibili e la loro obbligatorietà iniziale si impostano in [Configurazione PagoPA](pagopa-configurazione.html).

## Filtrare i pagamenti

La card dei filtri contiene questi campi:

| Campo | Tipo | Cosa filtra |
|-------|------|-------------|
| **Tipo pratica** | Tendina con ricerca | I tipi di pratica attivi per il tuo Ente |
| **Professionista** | Tendina con ricerca | I professionisti che operano con l'Ente, in ordine di cognome e nome |
| **Servizio PagoPA** | Tendina con ricerca | I servizi PagoPA configurati per l'Ente |
| **Stato del pagamento** | Tendina | Uno degli stati del pagamento (vedi [tabella degli stati](#stati-del-pagamento)); **Tutti** non filtra |
| **Titolare** | Testo | Il nome del titolare della pratica |
| **# Pratica** | Testo | Il numero della pratica |
| **Codice IUV** | Testo | Il codice IUV del pagamento |

Le tendine **Tipo pratica**, **Professionista** e **Servizio PagoPA** mostrano "Tutti" quando sono vuote: puoi scrivere qualche lettera per cercare la voce e svuotarle con la piccola **x**.

Per applicare i filtri:
1. Compila uno o più campi.
2. Clicca su **Filtra** (oppure premi Invio in un campo di testo).

L'elenco si ricarica con i soli pagamenti che rispettano **tutti** i filtri impostati.

Per tornare all'elenco completo clicca su **Rimuovi filtri**. Il pulsante compare solo quando almeno un filtro è attivo.

## L'elenco dei pagamenti

L'elenco è una tabella con ricerca, ordinamento e paginazione (vedi [Interfaccia e convenzioni](interfaccia-e-convenzioni.html)). All'apertura è ordinato per **# Pratica**, dalle più recenti: l'ordinamento considera prima l'anno e poi il numero.

| Colonna | Contenuto |
|---------|-----------|
| **# Pratica** | Numero della pratica |
| **Tipo** | Tipo di pratica |
| **Titolare** | Titolare della pratica, in maiuscolo |
| **Professionista** | Professionista che compila la pratica, in maiuscolo |
| **Servizio PagoPA** | Descrizione del servizio di pagamento |
| **Importo** | Importo in euro; se l'importo non è ancora stato indicato compare *da valorizzare* |
| **Stato** | Badge con lo stato del pagamento e, sotto, il **codice IUV** se è già stato generato |
| **Pagamento** | Pulsante **Obbligatorio** o **Facoltativo** (vedi sotto) |

Il campo **Cerca** della tabella cerca anche nel codice IUV.

Quando nessun pagamento corrisponde ai filtri compare il messaggio "Nessun pagamento corrisponde ai filtri.".

### Stati del pagamento

Il badge nella colonna **Stato** ha un colore che aiuta a riconoscere a colpo d'occhio la situazione del pagamento:

| Stato | Colore del badge |
|-------|------------------|
| **Senza IUV** | Neutro |
| **Inviato, in attesa di IUV** | Giallo |
| **IUV creato, pagabile su PagoPA** | Azzurro |
| **Inoltrato** | Azzurro |
| **Accettato** | Azzurro |
| **Autorizzato** | Azzurro |
| **Differito** | Azzurro |
| **In attesa di esito** | Azzurro |
| **Eseguito** | Verde |
| **Eseguito parzialmente** | Verde |
| **Incassato** | Verde |
| **Non eseguito** | Rosso |
| **Non eseguito per decorrenza dei termini** | Rosso |
| **Stornato** | Rosso |
| **Revocato** | Rosso |
| **Scaduto** | Rosso |
| **Annullato** | Rosso |

In sintesi: azzurro indica che il pagamento è pagabile o in corso, verde che è andato a buon fine, rosso che non è andato a buon fine o non è più valido.

{: .note }
> **Senza IUV** significa che il professionista non ha ancora generato il codice di pagamento. Gli stati successivi arrivano dal sistema PagoPA. Il significato dettagliato di ogni stato è descritto, dal punto di vista del professionista, nell'appendice "Stati PagoPA" del manuale dei professionisti.

## Rendere un pagamento obbligatorio o facoltativo

Nella colonna **Pagamento** ogni riga ha un pulsante che mostra la situazione attuale:

| Pulsante | Significato | Cosa succede se lo clicchi |
|----------|-------------|----------------------------|
| **Obbligatorio** (verde, lucchetto chiuso) | Il professionista deve effettuare il pagamento prima di poter inviare la pratica | Ti viene chiesto se renderlo facoltativo |
| **Facoltativo** (grigio, lucchetto aperto) | Il professionista può inviare la pratica anche senza pagare | Ti viene chiesto se renderlo obbligatorio |

Per cambiare l'obbligatorietà:
1. Individua il pagamento nell'elenco.
2. Clicca sul pulsante nella colonna **Pagamento**.
3. Si apre la finestra di conferma con il titolo **Rendere obbligatorio il pagamento?** oppure **Rendere facoltativo il pagamento?**. La finestra riporta il servizio, il numero della pratica, l'importo e una spiegazione dell'effetto.
4. Clicca su **Rendi obbligatorio** (o **Rendi facoltativo**) per confermare, oppure su **Annulla** per lasciare tutto com'è.

Dopo la conferma l'elenco si ricarica mantenendo i filtri impostati e compare la notifica verde **Pagamento reso obbligatorio** (o **Pagamento reso facoltativo**) con il numero della pratica.

{: .schermata }
> `assets/images/gestione-pagopa-conferma-obbligo.png` — La finestra "Rendere facoltativo il pagamento?" con servizio, numero di pratica, importo e il pulsante Rendi facoltativo.

{: .warning }
> La modifica ha effetto direttamente sul professionista: un pagamento reso **obbligatorio** blocca l'invio della pratica finché non risulta pagato; un pagamento reso **facoltativo** gli consente di inviare la pratica senza pagare. Il professionista non può cambiare da solo questa impostazione: è l'Ente che decide.

{: .note }
> Se nella [Configurazione PagoPA](pagopa-configurazione.html) il servizio è impostato come **Obbligatorio se in sanatoria**, quando cambi l'obbligatorietà di un pagamento di quel servizio la stessa scelta vale anche per il caso di sanatoria.

### Quando usare questa funzione

Usala, per esempio, quando un professionista ti segnala di aver già pagato con un altro canale (es. bonifico) e la pratica risulta bloccata da un pagamento obbligatorio: dopo le tue verifiche puoi rendere quel pagamento facoltativo e consentirgli l'invio.

## Messaggi di errore

| Messaggio | Quando compare |
|-----------|----------------|
| "Pagamento non trovato: ricarica la pagina." | Il pagamento su cui hai cliccato non è più disponibile. Ricarica la pagina e riprova. |
| "Si è verificato un errore durante la lettura/elaborazione dei dati" | Errore generico durante il caricamento o il salvataggio |
| "Errore API: …" | Il servizio che fornisce i dati ha restituito un errore; il messaggio ne riporta il codice |

I messaggi compaiono nella finestra **Attenzione** (vedi [Interfaccia e convenzioni](interfaccia-e-convenzioni.html)).
