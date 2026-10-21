---
title: Configurazione PagoPA
nav_order: 30
parent: "Impostazioni dell'Ente"
description: Come collegare i servizi PagoPA dell'Ente ai tipi di pratica, stabilendo importo, obbligatorietà, obbligatorietà in sanatoria ed eventuale elenco di valori ammessi.
keywords: [PagoPA, servizi PagoPA, associazioni, tipo pratica, qualificazione intervento, importo, valori ammessi, obbligatorio, sanatoria, IUV]
IDRegione: 99
IDTipoPratica: 9999
Fonte: Manuale Enti
---

# Configurazione PagoPA

Questa sezione spiega come stabilire quali pagamenti PagoPA vengono richiesti al professionista nelle pratiche, collegando i servizi PagoPA dell'Ente ai tipi di pratica e impostandone importo e obbligatorietà.

## A cosa serve

Ogni **servizio PagoPA** dell'Ente (ad esempio "Diritti di segreteria" o "Sanzioni") può essere **associato** a uno o più tipi di pratica. Ogni associazione stabilisce:

- per quale **tipo di pratica** (ed eventualmente per quale qualificazione dell'intervento o Comune) il pagamento è previsto;
- l'**importo**: fisso, libero oppure da scegliere in un elenco di valori ammessi;
- se il pagamento è **obbligatorio**, facoltativo, oppure obbligatorio solo per le pratiche in sanatoria.

Dal punto di vista del professionista, le associazioni attive determinano i pagamenti che compaiono nella sezione **PagoPA** della pratica in compilazione e nell'elenco dei pagamenti obbligatori mostrato quando crea una nuova istanza:

- un pagamento **obbligatorio** deve essere completato prima di poter validare l'istanza; uno **facoltativo** può essere ignorato;
- con un **importo** maggiore di zero, l'importo è già compilato quando il professionista crea lo IUV su GeoTecSUE;
- con importo **0** l'importo è "da valorizzare": il professionista lo indica lui stesso oppure, se hai definito un elenco di valori ammessi, lo sceglie tra quelli. 

## Accedere alla pagina

Dal menu in alto scegli **Impostazioni › PagoPA**.

Si apre la pagina **Gestione PagoPA**.

## Servizi PagoPA dell'Ente

Nella prima card, **Servizi PagoPA dell'ente**, trovi i servizi PagoPA configurati per il tuo Ente. Da questa pagina non puoi aggiungere né modificare i servizi: puoi solo gestirne le associazioni. 
Se un pagamento è mancante, contatta la nostra assistenza per avere indicazioni su come aggiungere il tipo di pagamento.

Se non ci sono servizi compare il messaggio **Nessun servizio PagoPA configurato per l'ente.**

| Colonna | Contenuto |
|---------|-----------|
| **Codice** | Codice del servizio PagoPA |
| **Descrizione** | Descrizione del servizio |
| **ID sotto ente** | Identificativo tecnico del sotto ente, se presente |
| **ID M.E. fittizio** | Identificativo tecnico multi-ente, se presente |
| *(pulsante)* | **Associazioni**: apre l'elenco delle associazioni del servizio |

La tabella ha la casella **Cerca**, l'ordinamento per colonna e la paginazione descritti in [Interfaccia e convenzioni](interfaccia-e-convenzioni.html).

{: .schermata }
> `assets/images/pagopa-configurazione-servizi.png` — La card Servizi PagoPA dell'ente con l'elenco dei servizi e il pulsante Associazioni.

## Associazioni di un servizio

1. Nella riga del servizio clicca su **Associazioni**.
2. Sotto l'elenco dei servizi compare la card **Associazioni del servizio:** seguita dalla descrizione del servizio, e la pagina scorre fino a essa.

Se il servizio non ha ancora associazioni compare il messaggio **Nessuna associazione: usa Nuova associazione per collegare il servizio ai tipi di pratica.**

| Colonna | Contenuto |
|---------|-----------|
| **Tipo pratica** | Tipo di pratica a cui si applica il pagamento |
| **Qualificazione intervento** | Qualificazione dell'intervento a cui è limitato il pagamento; vuota (—) se vale per tutte |
| **Comune** | Comune a cui è limitato il pagamento (solo Enti con più Comuni); vuota (—) se non indicato |
| **Importo** | Importo in euro; **libero / elenco** se l'importo è 0 |
| **Attiva** | Badge **Sì** (verde) / **No** (grigio) cliccabile |
| **Obbligatorio** | Badge **Sì** / **No** cliccabile: **No** significa facoltativo |
| **Obbl. sanatoria** | Badge **Sì** / **No** cliccabile: obbligatorio per le pratiche in sanatoria |
| *(pulsanti)* | Matita (**Modifica l'associazione**) e cestino (**Elimina l'associazione**) |

{: .schermata }
> `assets/images/pagopa-configurazione-associazioni.png` — La card Associazioni del servizio con le colonne Importo, Attiva, Obbligatorio e Obbl. sanatoria.

### Cambiare rapidamente attivazione e obbligatorietà

Clicca su un badge per invertirne il valore; la modifica viene salvata subito. Le notifiche sono:

| Badge cliccato | Notifica |
|----------------|----------|
| **Attiva** | **Associazione attivata** / **Associazione disattivata** |
| **Obbligatorio** | **Pagamento reso obbligatorio** / **Pagamento reso facoltativo** |
| **Obbl. sanatoria** | **Obbligatorio per le pratiche in sanatoria** / **Facoltativo per le pratiche in sanatoria** |

{: .warning }
> Le modifiche hanno effetto sulle pratiche che i professionisti andranno a compilare. Una pratica nata in precedenza ad una modifica non cambierà lo stato del pagamento.

## Creare un'associazione

1. Nella card delle associazioni clicca su **Nuova associazione**.
2. Si apre la finestra **Nuova associazione**: compila i campi (vedi la tabella sotto).
3. Clicca su **Salva**.

Compare la notifica **Associazione creata** e l'associazione si aggiunge all'elenco.

| Campo | Obbligatorio | Note |
|-------|--------------|------|
| **Tipo pratica** | ✅ | Scegli il tipo di pratica (**--- Seleziona ---** non è ammesso) |
| **Qualificazione intervento** | ❌ | **--- Tutte ---** se il pagamento vale per qualsiasi qualificazione dell'intervento |
| **Comune** | ❌ | Presente solo se l'Ente comprende più Comuni; **--- Nessun comune ---** se non va limitato a un Comune |
| **Attiva** | ❌ | Interruttore; **spento** per le nuove associazioni |
| **Obbligatorio** | ❌ | Interruttore; spento = pagamento facoltativo |
| **Obbligatorio se in sanatoria** | ❌ | Interruttore; rende il pagamento obbligatorio per le pratiche in sanatoria |
| **Importo** | ✅ | Importo in euro (es. `50,00`); **0** per un importo libero o da elenco |

{: .warning }
> Nelle nuove associazioni l'interruttore **Attiva** è spento. Se non lo accendi, il pagamento non sarà richiesto al professionista: puoi attivarlo anche in seguito con il badge **Attiva** nell'elenco.

Il campo **Importo** si formatta da solo quando esci dal campo (ad esempio `12` diventa `12,00`). Sotto il campo è ricordato che con importo **0** il professionista indica liberamente l'importo, oppure lo sceglie da un elenco di valori ammessi.

Se indichi una **Qualificazione intervento** o un **Comune**, il pagamento viene richiesto solo per le pratiche con quella qualificazione dell'intervento o relative a quel Comune.

Possibili messaggi di errore (finestra **Attenzione**; alla chiusura si torna alla finestra dell'associazione):

| Messaggio | Causa |
|-----------|-------|
| **Selezionare un tipo pratica.** | Tipo pratica non scelto |
| **Importo non valido.** | Importo non numerico o negativo |

### Associazione con importo 0: valori ammessi

Se salvi una **nuova** associazione con importo **0**, la finestra resta aperta e mostra il messaggio **L'associazione è stata salvata con importo 0. Aggiungi i valori ammessi uno alla volta, oppure chiudi la finestra per lasciare l'importo libero.**

Per creare l'elenco dei valori ammessi:

1. Scrivi un importo nel campo in euro.
2. Clicca su **Aggiungi valore**. Compare la notifica **Valore aggiunto**.
3. Ripeti per ogni valore.
4. Clicca su **Chiudi** quando hai finito.

Se non aggiungi alcun valore, l'importo resta libero.

{: .note }
> In questa fase i valori aggiunti non vengono elencati nella finestra: per controllarli riapri l'associazione con la matita.

Ogni valore deve essere maggiore di zero; altrimenti compare il messaggio **Inserire un valore maggiore di zero.**

## Modificare un'associazione

1. Clicca sulla matita della riga.
2. Si apre la finestra **Modifica associazione** con i dati salvati.
3. Modifica i campi.
4. Clicca su **Salva**.

Compare la notifica **Associazione salvata**.

{: .note }
> In modifica, scegliere **--- Nessun comune ---** non toglie il Comune già associato. Per togliere il Comune, elimina l'associazione e creala di nuovo.

{: .schermata }
> `assets/images/pagopa-configurazione-finestra-associazione.png` — La finestra Modifica associazione con importo 0 e la sezione Valori ammessi attiva.

### Gestire i valori ammessi

Quando l'associazione ha importo **0**, nella finestra di modifica compare l'interruttore **Usa un elenco di valori ammessi**:

- se l'associazione ha già dei valori, l'interruttore è acceso e al posto del campo **Importo** compare la sezione **Valori ammessi** con la tabella **Valore ammesso**;
- se non ha valori, l'interruttore è spento e l'importo è libero.

Per **aggiungere** un valore: accendi l'interruttore, scrivi l'importo nel campo sotto la tabella e clicca su **Aggiungi valore**.

Per **modificare** un valore:

1. Clicca sulla matita (**Modifica il valore**) a destra del valore.
2. Modifica l'importo.
3. Esci dal campo (clicca altrove o premi Tab): il valore viene salvato da solo e compare la notifica **Valore aggiornato**.

Per **eliminare** un valore:

1. Clicca sul cestino (**Elimina il valore**).
2. Nella finestra **Conferma eliminazione** (**Eliminare questo valore ammesso?**) clicca su **Elimina**. Con **Annulla** torni alla finestra dell'associazione.

Per **tornare all'importo libero**, spegni l'interruttore **Usa un elenco di valori ammessi**. Se ci sono valori, si apre la finestra **Disattivare l'elenco dei valori?** con il messaggio **Tutti i valori ammessi di questa associazione verranno eliminati e l'importo tornerà libero.**:

- **Elimina i valori** cancella tutti i valori (notifica **Valori ammessi eliminati**);
- **Annulla** lascia tutto com'era.

{: .warning }
> **Elimina i valori** cancella definitivamente tutti i valori ammessi dell'associazione.

Se modifichi un'associazione esistente portandone l'importo a **0** e salvi, la finestra resta aperta per permetterti di gestire i valori ammessi.

## Eliminare un'associazione

1. Clicca sul cestino della riga.
2. Nella finestra **Conferma eliminazione** (**Eliminare definitivamente questa associazione?**) clicca su **Elimina**, oppure su **Annulla**.

Compare la notifica **Associazione eliminata**.

{: .warning }
> L'eliminazione è definitiva: il pagamento non sarà più richiesto per quel tipo di pratica. Se vuoi sospenderlo temporaneamente, usa il badge **Attiva**.

## Collegamenti utili

- [Tipi pratiche](tipi-pratiche.html): i tipi di pratica attivi per l'Ente.
- [Gestione PagoPA](gestione-pagopa.html): la pagina del menu **Gestione PagoPA**, dedicata ai pagamenti delle pratiche.
- [Pagamenti](pagamenti.html): le schede informative sui pagamenti.
