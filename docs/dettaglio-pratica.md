---
title: Dettaglio della pratica
nav_order: 20
parent: Gestione pratiche
description: Descrive la pagina di dettaglio di una pratica trasmessa, con le schede informative e le azioni dell'Ente come protocollazione manuale, riporto allo stato precedente, voltura, ricevute e pagamenti PagoPA.
keywords: [dettaglio pratica, protocollazione, riporta allo stato precedente, voltura, ricevute, rigenera ricevuta, PagoPA, archivio zip, tracciabilità, invio libero, Regione Lombardia]
IDRegione: 99
IDTipoPratica: 9999
Fonte: Manuale Enti
---

# Dettaglio della pratica

Questa sezione spiega come consultare il dettaglio di una pratica trasmessa da un professionista e come usare le azioni che il back office mette a disposizione dell'Ente.

## Accedere alla pagina

Il dettaglio si apre cliccando sul numero o sulla lente di una pratica in:

- **Gestione Pratiche › Pratiche e comunicazioni trasmesse** (vedi [Pratiche e comunicazioni trasmesse](pratiche-trasmesse.html));
- **Gestione Pratiche › Gestione Protocollazione**, con il pulsante **Dettaglio della pratica** (vedi [Gestione protocollazione](gestione-protocollazione.html));
- **Gestione Pratiche › Trasmissioni Regione Lombardia** (vedi [Trasmissioni Regione Lombardia](trasmissioni-regione-lombardia.html)).

Le pratiche importate si aprono invece in [Dettaglio pratica importata](dettaglio-importata.html) e le notifiche preliminari in [Dettaglio notifica preliminare](dettaglio-notifica-preliminare.html): il passaggio è automatico.

Se la pratica non esiste o non è del tuo Ente compare l'avviso **Pratica non trovata** (*La pratica richiesta non esiste oppure non appartiene a questo Ente.*) con il solo pulsante **Ritorna**.

{: .schermata }
> `assets/images/dettaglio-pratica-panoramica.png` — L'intestazione della pratica con il badge di stato, il riquadro giallo "Da fare su questa pratica" e la fila delle schede.

## Intestazione

In alto trovi:

- la dicitura **Dettaglio pratica**, il **tipo di pratica** e il numero (**n. …**);
- il **badge di stato**, con i colori descritti in [Stati delle pratiche](appendici/stati-pratica.html);
- se la pratica è una variante, il pulsante **Variante a … n. …**, che apre il dettaglio della pratica originale.

Anche il titolo della scheda del browser riporta acronimo e numero della pratica.

A destra ci sono i pulsanti:

| Pulsante | Cosa fa | Quando compare |
|----------|---------|----------------|
| **Ritorna** | Torna alla pagina da cui hai aperto il dettaglio, con i filtri che avevi impostato | Sempre |
| **Archivio della pratica** | Scarica un file .zip con i documenti della pratica | Sempre |
| **Consenti invio libero** | Permette al professionista di trasmettere integrazioni volontarie per questa pratica | Vedi [Invio libero di integrazioni](#invio-libero-di-integrazioni) |
| **Rimuovi invio libero** | Revoca il permesso dato con **Consenti invio libero** | Vedi [Invio libero di integrazioni](#invio-libero-di-integrazioni) |

### Archivio della pratica

1. Clicca su **Archivio della pratica**.
2. Attendi la preparazione dell'archivio (compare lo spinner).
3. Il browser scarica il file `<numero pratica> - <acronimo>.zip`.

Il contenuto dell'archivio è preparato dal server con i documenti della pratica. <!-- DA VERIFICARE: l'elenco dei file inclusi nello zip (istanza, firmato, allegati, ricevute, comunicazioni) non è visibile nel codice del back office --> L'archivio è temporaneo: viene eliminato dopo lo scarico. Se la preparazione non riesce compare *Non è stato possibile creare l'archivio della pratica* oppure *L'archivio della pratica non è disponibile: riprova a generarlo.*

### Invio libero di integrazioni

I pulsanti **Consenti invio libero** / **Rimuovi invio libero** compaiono solo se nella [Scheda Ente](scheda-ente.html) l'opzione **Consenti al professionista l'invio libero di documentazione** è disattivata: in questo caso puoi aprire l'invio libero pratica per pratica. Se l'opzione è attiva per tutte le pratiche, i pulsanti non compaiono. Vedi sempre uno solo dei due, in base alla situazione della pratica.

1. Clicca su **Consenti invio libero**.
2. La pagina si ricarica con la notifica verde *Il professionista può ora inviare integrazioni volontarie*.

Con **Rimuovi invio libero** la notifica è *Invio libero di integrazioni non più consentito*.

## Riquadro "Da fare su questa pratica"

Sotto l'intestazione può comparire un riquadro giallo **Da fare su questa pratica**. Contiene solo le voci che riguardano la pratica in quel momento; se non ce n'è nessuna, il riquadro non compare.

### Richiesta di integrazioni in attesa di risposta

Compare quando sulla pratica c'è una richiesta di integrazioni ancora aperta. Mostra la data della richiesta (**dal …**), l'eventuale descrizione e l'elenco dei **Documenti richiesti**. È solo informativo: il professionista risponde dal proprio portale.

### Protocollazione della pratica

Compare solo se la pratica è nello stato **Inviata** e per il tuo Ente è attiva la protocollazione manuale (Enti senza protocollo informatico collegato). <!-- DA VERIFICARE: l'opzione di protocollazione manuale non si imposta da questo back office; indicare chi la attiva --> Le pratiche da protocollare si possono gestire anche tutte insieme dalla pagina [Gestione protocollazione](gestione-protocollazione.html).

1. Inserisci il **Numero di protocollo** (solo numero intero positivo).
2. Controlla la **Data di protocollo**: è già proposta la data di oggi; puoi sceglierne un'altra dal calendario, ma non una data futura.
3. Clicca su **Protocolla**.
4. Nella finestra **Protocollare la pratica?** verifica numero e data e clicca su **Protocolla**.

La pagina si ricarica con la notifica *Pratica protocollata (n. … del …)*. Se eri arrivato dalla pagina Gestione protocollazione, torni a quella pagina.

{: .warning }
> La protocollazione non si annulla dal back office. Il professionista riceve nel portale la notifica **Pratica Protocollata** con numero e data di protocollo e, se nella pagina [Mail](mail.html) l'evento **Protocollazione pratica** è abilitato per il professionista, anche un messaggio "GeotecSUE: Pratica Protocollata" via mail normale, PEC o entrambe, secondo il **Tipo notifica** della [Scheda Ente](scheda-ente.html). Nella tracciabilità viene registrato "Pratica Protocollata con Numero …".

Messaggi possibili:

- *Inserisci il numero di protocollo (un numero intero).*
- *Inserisci la data di protocollo nel formato gg/mm/aaaa.*
- *La data di protocollo non può essere futura.*
- *La pratica non è più nello stato "Inviata": ricarica la pagina.* (qualcun altro l'ha già lavorata)

### Riporta la pratica allo stato precedente

Compare solo se la pratica è nello stato **Inviata**. Serve a restituire al professionista una pratica che non può essere accettata così com'è, prima della protocollazione.

1. Scrivi la **Motivazione** (obbligatoria).
2. Clicca su **Riporta allo stato precedente**.
3. Nella finestra **Riportare la pratica allo stato precedente?** rileggi l'anteprima della motivazione.
4. Clicca su **Riporta allo stato precedente** per confermare, oppure su **Annulla**.

Dopo la conferma torni all'elenco da cui eri partito.

{: .warning }
> L'operazione ha effetto immediato verso il professionista. La pratica torna nello stato **Firmata** (se nella [Scheda Ente](scheda-ente.html) è attiva l'opzione **Richiedi il p7m in fase di invio pratica**) oppure **Completata**, e la data di invio viene cancellata: il professionista potrà modificarla e trasmetterla di nuovo. Riceve nel portale la notifica **Pratica regredita di stato** con la tua motivazione e un messaggio "GeotecSUE: Pratica regredita di stato" via mail normale, PEC o entrambe, secondo il **Tipo notifica** dell'Ente. La motivazione viene registrata anche nella tracciabilità.

Se la motivazione è vuota compare *Inserisci la motivazione: verrà inviata al professionista.*

## Le schede

Sotto il riquadro delle azioni la pratica è divisa in schede. Alcune compaiono solo se hanno un contenuto; accanto al nome alcune riportano un contatore. La scheda che stavi guardando viene ricordata per quella pratica finché il browser resta aperto.

| Scheda | Quando compare |
|--------|----------------|
| **Pratica** | Sempre |
| **Soggetti** | Sempre |
| **Documenti** (con il numero di allegati) | Sempre |
| **Ente** | Solo se l'Ente ha già registrato dati propri sulla pratica (protocollo, istruttoria) |
| **Comunicazioni** (con il numero) | Solo se esistono comunicazioni trasmesse collegate |
| **Ricevute** | Sempre |
| **Pagamenti** (con il numero) | Solo se esistono pagamenti PagoPA |
| **Storico** | Sempre |

### Scheda Pratica

La card **Dati generali** riporta **Numero pratica**, **Anno**, **Tipo pratica**, **Qualificazione intervento**, **Stato**, la **Descrizione dell'intervento** (se indicata) e le date **Registrata il**, **Ultima modifica** e **Inviata il**.

Sotto le date trovi i pulsanti per scaricare l'istanza:

- **Istanza (PDF)**: il modulo generato dal sistema;
- **Istanza firmata (P7M)**: il file firmato digitalmente caricato dal professionista.

Se un file non esiste il pulsante è grigio e disattivato (passa con il mouse per leggere il motivo).

La card **Localizzazione dell'intervento** riporta la **Località dei lavori**, il **Comune** (solo per gli Enti con più Comuni) e le tabelle **Catasto fabbricati** (Sezione, Foglio, Mappale, Subalterno) e **Catasto terreni** (Sezione, Foglio, Mappale). Se non ci sono dati catastali compare *Nessun riferimento catastale indicato.*

### Scheda Soggetti

La card **Titolare originale** riporta **Cognome e nome**, **Codice fiscale**, **Nascita**, **Residenza** ed **E-mail**. Possono comparire anche:

- il riquadro **Ditta / Società / Ente rappresentato** (Denominazione, Partita IVA / C.F., Sede, E-mail, PEC);
- la tabella **Altri titolari** (Cognome, Nome, Codice fiscale, Data di nascita);
- la tabella **Titolari dopo voltura** (Cognome e nome, Codice fiscale, Richiesta, Conferma, **Referente PagoPA**).

#### Referente dei pagamenti PagoPA

Nella tabella **Titolari dopo voltura** la colonna **Referente PagoPA** indica a quale titolare sono intestati i pagamenti PagoPA (badge verde **Sì**, grigio **No**).

1. Clicca sul badge del titolare da indicare come referente.
2. La notifica verde conferma *… è ora il referente dei pagamenti PagoPA*.

Il referente è uno solo: gli altri titolari diventano automaticamente **No**. Cliccando su un badge **Sì** togli il ruolo (*… non è più il referente dei pagamenti PagoPA*).

#### Professionista e voltura

La card **Professionista** riporta **Cognome e nome**, **Codice fiscale**, **Nascita** e, se presenti, **Iscritto all'ordine / collegio**, **Provincia** e **Numero**.

Con **Voltura ad altro professionista** puoi intestare la pratica a un altro professionista:

1. Nella casella di ricerca scrivi cognome, nome o codice fiscale e seleziona il professionista. L'elenco contiene i professionisti registrati presso l'Ente, escluso quello attuale. <!-- DA VERIFICARE: criterio esatto con cui il server compone l'elenco dei professionisti -->
2. Clicca su **Voltura**.
3. Nella finestra **Volturare la pratica?** controlla il nome e clicca su **Voltura**.

La pagina si ricarica con la notifica *Pratica volturata a …*.

{: .warning }
> Dopo la voltura la pratica è gestita dal nuovo professionista. Il professionista precedente riceve nel portale la notifica **Pratica Volturata** (non viene inviata alcuna mail) e nella tracciabilità viene registrato "Pratica Volturata da … a …". Se la pratica era nello stato **Revoca Delegato**, torna allo stato che aveva prima della revoca.

Se non selezioni nessuno compare *Seleziona il professionista a cui volturare la pratica.*

### Scheda Documenti

La tabella elenca gli allegati della pratica:

| Colonna | Contenuto |
|---------|-----------|
| **Inserito il** | Data e ora di caricamento |
| **Documento** | Descrizione e, sotto, il nome del file |
| **Disponibile fino al** | Data fino alla quale il file è scaricabile; se è passata compare il badge **Scaduto il …** |
| (freccia) | Scarica il file |

Per i documenti scaduti il pulsante di scarico è disattivato; se provi comunque compare *L'allegato non è più disponibile: era scaricabile fino al …*

### Scheda Ente

Contiene i dati che l'Ente ha registrato sulla pratica. Sono in sola lettura: in questa pagina non si modificano. <!-- DA VERIFICARE: i dati arrivano dal gestionale dell'Ente collegato a GeoTecSUE -->

- **Protocollo e istruttoria**: **Numero protocollo**, **Data protocollo**; se la pratica è registrata anche **Numero pratica dell'Ente** e **Registrata il**; se è assegnata **Responsabile del procedimento**, **Responsabile del servizio** e **Assegnata il**; se verificata **Verificata il**.
- **Provvedimento** (solo se c'è un numero di provvedimento): **Numero provvedimento**, **Data provvedimento** e la tabella dei documenti con **Emesso il**, **Documento**, **Letto dal professionista** e il pulsante di scarico.
- **Documenti inviati dall'Ente** (con il totale e quanti non sono ancora stati letti): **Tipo** (Documento, Rilascio provvedimento, Parere), **Emesso il**, **Descrizione**, **Letto dal professionista**. Le righe non ancora lette sono in grassetto e mostrano il badge **Non ancora**.
- **Richieste di integrazione** (con il numero): un elenco a fisarmonica, dalla più recente. Ogni voce mostra la descrizione, la data della richiesta e il badge **In attesa di risposta** (giallo) o **Risposta inviata** (verde). Aprendola vedi **Pratica di integrazione**, **Richiesta il**, **Inviata il**, **Accettata il**, **Protocollo** e i documenti trasmessi (**Accettato il**, **Documento**, **Disponibile fino al**, scarico).
- **Agibilità**: **Numero domanda**, **Protocollo**, **Tipo** (Parziale o Totale), **Rilascio**, **Data agibilità**.

{: .note }
> Scaricare un documento dell'Ente dal back office **non** lo segna come letto: la data di lettura è quella in cui lo ha aperto il professionista.

### Scheda Comunicazioni

Elenca, dalla più recente, le comunicazioni trasmesse dal professionista e collegate alla pratica. Ogni voce mostra tipo, numero, data di invio, badge di stato e il numero di allegati. Aprendola trovi:

- **Inviata il** e **Protocollo** (oppure *Non ancora protocollata*);
- i pulsanti **Comunicazione (PDF)** e **Firmata (P7M)**, disattivati se il file non esiste (ad esempio per un invio libero); per alcuni tipi di comunicazione i pulsanti non compaiono <!-- DA VERIFICARE: il codice esclude un tipo di comunicazione specifico, presumibilmente l'invio libero di documentazione -->;
- la tabella degli allegati (**Inserito il**, **Allegato**, **Disponibile fino al**, scarico).

### Scheda Ricevute

Per la pratica (card **Pratica n. …**) e per ogni comunicazione o integrazione collegata (card con tipo e numero) trovi le ricevute previste e il loro stato.

| Ricevuta | Pratica | Comunicazioni e integrazioni |
|----------|---------|------------------------------|
| **Ricevuta di invio** | ✅ | ✅ |
| **Ricevuta di protocollazione** | ✅ | ✅ |
| **Ricevuta di registrazione** | ✅ | ❌ |

| Stato | Significato | Pulsanti |
|-------|-------------|----------|
| **Disponibile** (verde) | La ricevuta esiste | **Rigenera**, **Scarica** |
| **In generazione** (giallo) | Ricevuta di invio, nella prima ora dopo la trasmissione: ricarica la pagina tra qualche minuto | **Rigenera** |
| **Non generata** (rosso) | La ricevuta manca | **Rigenera** |
| **Non ancora prevista** (neutro) | La pratica non ha ancora raggiunto lo stato che la prevede (protocollazione: dopo **Inviata**; registrazione: dopo **Protocollata**) | Nessuno |

Per scaricare una ricevuta clicca su **Scarica**: il file si chiama `RI_`, `RP_` o `RR_` seguito dal numero della pratica.

Per rigenerarla:

1. Clicca su **Rigenera**.
2. La pagina si ricarica con la notifica *Ricevuta … rigenerata (n. …)*.

Se la rigenerazione non riesce compare *Non è stato possibile rigenerare la ricevuta. Riprova tra qualche minuto.* <!-- DA VERIFICARE: se la ricevuta rigenerata viene resa disponibile o notificata anche al professionista -->

### Scheda Pagamenti

Compare solo se la pratica ha pagamenti PagoPA. Se il tuo Ente ha PagoPA attivo, all'apertura della pagina lo stato dei pagamenti viene aggiornato leggendolo da PagoPA.

La card **Pagamenti da effettuare** elenca i pagamenti già trasmessi a PagoPA e non ancora completati:

| Colonna | Contenuto |
|---------|-----------|
| **Descrizione** | Servizio PagoPA; "(generato dall'Ente)" se creato dall'Ente; "[Comunicazione - …]" se riguarda una comunicazione collegata |
| **Rata** | Numero della rata, se rateizzato |
| **Scadenza** | Scadenza dello IUV |
| **Importo** | Importo in euro, oppure *Da valorizzare* |
| **Codice IUV** | Codice del pagamento |
| **Stato** | Stato PagoPA (giallo se lo IUV è in attesa di generazione) |
| **Aggiorna stato** | Rilegge lo stato da PagoPA |

Se uno IUV è in attesa di generazione compare un avviso: attendi qualche minuto e clicca su **Aggiorna stato**. La notifica *Stato del pagamento aggiornato* riporta il nuovo stato; quando lo IUV viene generato, l'operazione è registrata anche nella tracciabilità.

La card **Pagamenti completati** elenca i pagamenti eseguiti con **Descrizione**, **Rata**, **Richiesta IUV**, **Pagato il**, **Importo**, **Codice IUV** e **Stato**.

Per la configurazione e il monitoraggio complessivo vedi [PagoPA](pagopa-configurazione.html) e [Gestione PagoPA](gestione-pagopa.html).

### Scheda Storico

La card **Tracciabilità** elenca tutte le operazioni registrate sulla pratica (**Data**, **Operazione**), dalla più recente, con ricerca e paginazione.

La card **Interoperabilità con Regione Lombardia** compare solo se la pratica è stata trasmessa a Regione Lombardia. Riporta **Fase di aggiornamento**, **Codice R.L.**, **ID R.L.**, **ID integrazione R.L.**, **Procedimento R.L.** e **Trasmessa il**. Per l'elenco di tutte le trasmissioni vedi [Trasmissioni Regione Lombardia](trasmissioni-regione-lombardia.html).

{: .schermata }
> `assets/images/dettaglio-pratica-ricevute.png` — La scheda Ricevute con i badge Disponibile, Non generata e Non ancora prevista e i pulsanti Rigenera e Scarica.

## Avvisi e messaggi

- Ogni parte della pagina si carica in modo indipendente. Se una parte non si carica compare la finestra **Attenzione** con *Non è stato possibile caricare: … Le altre informazioni della pratica sono corrette; se il problema si ripete, segnala il numero della pratica all'assistenza.*
- *Pratica non trovata: ricarica la pagina.* compare se la pratica non è più disponibile mentre lavori.
- Gli errori di scarico indicano il documento (es. *Non è stato possibile scaricare la ricevuta.*).

Le convenzioni comuni (spinner, notifiche verdi, finestra **Attenzione**) sono descritte in [Interfaccia e convenzioni](interfaccia-e-convenzioni.html).
