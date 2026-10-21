---
title: Tipi pratiche
nav_order: 40
parent: "Impostazioni dell'Ente"
description: Come attivare e disattivare i tipi di pratica disponibili ai professionisti e come impostarne bollo, tipologia, trasmissione al cittadino, tipi di intervento, descrizione e attivazione per Comune.
keywords: [tipi pratiche, attivazione pratica, disattivazione pratica, bollo, tipi di intervento, qualificazione intervento, comunicazione, cittadino, multi-ente, comuni]
IDRegione: 99
IDTipoPratica: 9999
Fonte: Manuale Enti
---

# Tipi pratiche

Questa sezione spiega come scegliere quali tipi di pratica l'Ente rende disponibili sul portale e come impostarne le caratteristiche principali.

## A cosa serve

Dal punto di vista del professionista, solo i tipi di pratica **attivi** compaiono nel menu **Seleziona il tipo di Pratica** quando crea una nuova istanza: se un procedimento non è attivo, il professionista non lo trova e deve rivolgersi all'Ente. Allo stesso modo, i **tipi di intervento** attivi per una pratica sono quelli che il professionista può scegliere nel menu **Tipo Intervento**.

## Accedere alla pagina

Dal menu in alto scegli **Impostazioni › Tipi Pratiche**.

Si apre la pagina **Gestione Tipologie Pratiche**, divisa in due card: **Pratiche attive** e **Pratiche disattive**. Accanto a ogni titolo un badge indica quante pratiche contiene.

Entrambe le tabelle hanno la casella **Cerca**, l'ordinamento per colonna e la paginazione descritti in [Interfaccia e convenzioni](interfaccia-e-convenzioni.html).

{: .schermata }
> `assets/images/tipi-pratiche-elenco.png` — La pagina Gestione Tipologie Pratiche con le card Pratiche attive e Pratiche disattive.

## Pratiche attive

| Colonna | Contenuto |
|---------|-----------|
| **Tipo pratica** | Nome del tipo di pratica |
| **Descrizione** | Descrizione estesa del tipo di pratica (normalmente comprende anche la Regione di appartenenza) |
| **Acronimo** | Sigla della pratica (es. CILA, SCIA) |
| **Tipologia** | Badge **Pratica** e/o **Comunicazione** (o entrambi) |
| **Cittadino** | Icona verde se il cittadino può trasmettere la pratica; trattino se no |
| **Bollo** | Importo del bollo, se la pratica è in bollo |
| *(pulsanti)* | Matita (**Impostazioni della pratica**) e cerchio barrato (**Disattiva la pratica**) |

{: .note }
> La riga evidenziata in giallo indica una pratica che è trasmissibile da un cittadino.

### Disattivare una pratica

1. Clicca sul cerchio barrato (**Disattiva la pratica**) nella riga.
2. Si apre la finestra **Disattivare la pratica?** con il nome della pratica.
3. Clicca su **Disattiva** per confermare, oppure su **Annulla**.

La pagina si ricarica, compare la notifica **Pratica disattivata** e la pratica passa nella card **Pratiche disattive**.
Se un professionista aveva in compilazione quella tipologia, può comunque ancora procedere con la trasmissione.

{: .warning }
> Dopo la disattivazione la pratica non è più disponibile per i professionisti. Come indica la finestra di conferma, se la riattivi in seguito le impostazioni personalizzate (bollo, descrizione, tipi di intervento) potrebbero dover essere reimpostate.

## Pratiche disattive

La card elenca i tipi di pratica che l'Ente può attivare ma che al momento non sono attivi.

| Colonna | Contenuto |
|---------|-----------|
| **Tipo pratica** | Nome del tipo di pratica |
| **Descrizione** | Descrizione estesa |
| **Acronimo** | Sigla della pratica |
| **Pratiche presentate** | Numero di pratiche di questo tipo già presenti per l'Ente |
| *(pulsante)* | **Attiva**, oppure il badge **Non attivabile** |

### Pratiche non attivabili

Il badge **Non attivabile** (con il lucchetto) indica che manca un prerequisito. Passa con il mouse sul badge per leggerne il motivo:

| Motivo | Cosa fare |
|--------|-----------|
| **Occorre prima impostare la zona UNESCO dell'ente.** | Imposta la zona UNESCO nella [Scheda Ente](scheda-ente.html) |
| **Occorre prima attivare la trasmissione al MUDE.** | Attiva la trasmissione al MUDE per l'Ente (da definire con assistenza **SISCOM** |

### Attivare una pratica

1. Clicca su **Attiva** nella riga della pratica.
2. Si apre la finestra **Attivare la pratica?** con il nome della pratica.
3. Clicca su **Attiva** per confermare, oppure su **Annulla**.

La pagina si ricarica, compare la notifica **Pratica attivata** e la pratica passa nella card **Pratiche attive**.

All'attivazione la pratica riceve le impostazioni previste dalla configurazione di base:

- tipologia (pratica e/o comunicazione), possibilità di trasmissione da parte del cittadino e descrizione;
- bollo, se previsto;
- allegati richiesti e relativi modelli;
- tipi di intervento;
- comunicazioni collegate (vedi [Comunicazioni](comunicazioni.html)).

{: .warning }
> Se riattivi una pratica disattivata in precedenza, gli allegati e i modelli della pratica vengono reimpostati come da configurazione di base: le personalizzazioni fatte in passato sugli allegati di quella pratica non vengono recuperate. Dopo l'attivazione controlla le pagine [Allegati](allegati.html) e [Modulistica](modulistica.html).

Se la configurazione di base è incompleta compare il messaggio **Nel file di configurazione mancano il tipo pratica o il tipo attivazione: impossibile attivare la pratica.** In questo caso rivolgiti all'assistenza.

## Impostazioni di una pratica

1. Nella card **Pratiche attive** clicca sulla matita (**Impostazioni della pratica**).
2. Si apre una finestra con il nome della pratica come titolo.
3. Modifica le impostazioni (descritte sotto).
4. Clicca su **Salva**.

La pagina si ricarica e compare la notifica **Impostazioni salvate**. Con **Chiudi** esci senza salvare.

{: .note }
> Le modifiche ai **Tipi di intervento** vengono salvate subito, al clic sul badge. Tutte le altre impostazioni vengono salvate solo con **Salva**.

{: .schermata }
> `assets/images/tipi-pratiche-impostazioni.png` — La finestra delle impostazioni di una pratica con le sezioni Bollo, Tipologia, Trasmissione, Tipi di intervento e Descrizione.

### Bollo

| Campo | Note |
|-------|------|
| **Pratica in bollo** | Interruttore. Acceso: la pratica è soggetta a bollo |
| Importo (€) | Valore del bollo; modificabile solo se l'interruttore è acceso. Si formatta da solo (es. `16` diventa `16,00`) |

Se l'interruttore è acceso l'importo deve essere maggiore di zero, altrimenti compare il messaggio **Indicare un valore del bollo valido (maggiore di zero).** Se spegni l'interruttore e salvi, il bollo viene tolto dalla pratica.

Dal punto di vista del professionista, il bollo indica che la pratica è soggetta all'imposta di bollo per l'importo impostato.

### Tipologia

| Interruttore | Significato |
|--------------|-------------|
| **Pratica** | Il tipo è utilizzabile come pratica autonoma |
| **Comunicazione** | Il tipo è utilizzabile come comunicazione collegata a una pratica; compare nell'elenco della pagina [Comunicazioni](comunicazioni.html) |

Almeno uno dei due deve essere acceso, altrimenti compare il messaggio **Selezionare almeno una tipologia: Pratica e/o Comunicazione.**
Se entrambi vengono selezionati la pratica comparirà sia nell'elenco delle *Nuove istanze* che nelle comunicazioni impostate.

### Trasmissione

L'interruttore **Consenti la trasmissione della pratica al cittadino** indica che la pratica può essere trasmessa anche da un cittadino; nell'elenco delle pratiche attive la colonna **Cittadino** mostra l'icona verde.
La trasmissione **del cittadino** significa che non richiede la firma digitale su allegati ed istanza.

### Tipi di intervento

La tabella elenca tutti i tipi di intervento (ad esempio Manutenzione straordinaria, Ristrutturazione edilizia) con il badge **Attivo**:

1. Clicca su **No** per rendere disponibile il tipo di intervento per questa pratica.
2. Clicca su **Sì** per toglierlo.

La modifica è salvata subito e compare la notifica **Tipo di intervento attivato** oppure **Tipo di intervento disattivato**.

Dal punto di vista del professionista, sono i valori proposti nel menu **Tipo Intervento** quando crea una nuova istanza di questo tipo. Se nessun tipo di intervento è attivo, il campo non viene richiesto.

### Descrizione

Campo di testo libero con la descrizione della pratica per il tuo Ente. Alla prima attivazione è proposta la descrizione della configurazione di base.

{: .note }
> Se un salvataggio non va a buon fine, alla chiusura della finestra **Attenzione** torni alla finestra delle impostazioni con i dati che stavi inserendo.

## Attivazioni per Comune

Per gli Enti che comprendono più Comuni (ad esempio le Unioni), nella card **Pratiche attive** compare il pulsante **Attivazioni per comune**, che permette di disattivare una pratica solo per alcuni Comuni. 

1. Clicca su **Attivazioni per comune**.
2. Nella finestra **Attivazioni per comune** scegli il **Comune** dal menu (**--- Seleziona il comune ---**).
3. Compare l'elenco delle pratiche attive dell'Ente con il badge **Attiva** per quel Comune.
4. Clicca su **Sì** per disattivare la pratica in quel Comune, su **No** per riattivarla.

Le modifiche vengono salvate subito; compare la notifica **Pratica disattivata per il comune** oppure **Pratica attivata per il comune**, con il nome della pratica e del Comune. Clicca su **Chiudi** quando hai finito.

Dal punto di vista del professionista, una pratica disattivata per un Comune non è selezionabile per gli interventi in quel Comune. 
## Collegamenti utili

- [Comunicazioni](comunicazioni.html): in quali pratiche è disponibile ogni comunicazione.
- [Allegati](allegati.html) e [Allegati in pratica](allegati-in-pratica.html): i documenti richiesti per ogni pratica.
- [Configurazione PagoPA](pagopa-configurazione.html): i pagamenti richiesti per ogni pratica.
