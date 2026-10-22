---
title: Dettaglio della notifica preliminare
nav_order: 70
parent: Gestione pratiche
description: Spiega come consultare il dettaglio di una notifica preliminare trasmessa a MUDE Piemonte, scaricarne istanza, allegati, archivio e ricevute, e leggerne la tracciabilità.
keywords: [dettaglio notifica preliminare, MUDE, SPRESAL, numero istanza MUDE, protocollazione, ricevute, archivio zip, allegati, tracciabilità, Piemonte]
IDRegione: 99
IDTipoPratica: 9999
Fonte: Manuale Enti
---

# Dettaglio della notifica preliminare

Questa sezione spiega come consultare il dettaglio di una **notifica preliminare**, la comunicazione di avvio cantiere che il professionista trasmette tramite GeoTecSUE a MUDE Piemonte e allo SPRESAL (vedi [Notifiche preliminari](notifiche-preliminari.html)).

Il dettaglio è una versione semplificata del [Dettaglio della pratica](dettaglio-pratica.html): la notifica non è gestita dall'Ente, quindi non ci sono protocollazione, istruttoria, richieste di integrazione, comunicazioni, pagamenti né voltura. Puoi consultare i dati, scaricare i documenti e le ricevute e, se serve, rigenerare una ricevuta.

## Accedere alla pagina

1. Dal menu in alto scegli **Gestione Pratiche › Notifiche Preliminari**.
2. Clicca sul numero della notifica o sul pulsante con la lente.

Se apri una notifica preliminare da un altro elenco, ad esempio [Pratiche e comunicazioni trasmesse](pratiche-trasmesse.html), il sistema ti porta comunque a questa pagina.

Se la notifica non esiste o non appartiene al tuo Ente, compare il riquadro **Notifica preliminare non trovata** ("La notifica richiesta non esiste oppure non appartiene a questo Ente.") con il solo pulsante **Ritorna**.

{: .schermata }
> `assets/images/dettaglio-notifica-preliminare-panoramica.png` — L'intestazione con il badge "MUDE" e la scheda Pratica con le card "Trasmissione a MUDE" e "Protocollazione su MUDE".

## Intestazione

In alto trovi:

- la dicitura **Dettaglio notifica preliminare**;
- il tipo di pratica (Notifica preliminare);
- il numero della notifica in GeoTecSUE ("n. …");
- il badge colorato dello **stato**: arancione per **Inviata SPRESALWEB (via MUDE)**, verde per **Protocollata SPRESALWEB**;
- il badge **MUDE**, che indica che la notifica è transitata da MUDE;
- a destra i pulsanti **Ritorna** e **Archivio della pratica**.

### Ritorna

Ti riporta sempre all'elenco [Notifiche preliminari](notifiche-preliminari.html), con i filtri che avevi impostato.

### Archivio della pratica

Scarica un file **.zip** con tutti i documenti della notifica.

1. Clicca su **Archivio della pratica**.
2. Attendi qualche istante (compare lo spinner mentre l'archivio viene preparato).
3. Il browser scarica il file, che ha come nome il numero della notifica e la sigla del tipo di pratica.

Se l'archivio non si riesce a creare si apre la finestra **Attenzione** ("Non è stato possibile creare l'archivio della pratica…"). L'archivio è temporaneo: viene eliminato dopo lo scarico.

### Ente non più attivo

Se il Comune della notifica è confluito in un altro Ente, sotto l'intestazione compare il riquadro rosso **Questo ente non è più attivo** con l'indicazione del nuovo Ente.

## Le schede

Il contenuto è diviso in cinque schede, sempre presenti: **Pratica**, **Soggetti**, **Documenti** (con il numero di allegati nel badge), **Ricevute** e **Storico**. La pagina ricorda l'ultima scheda che hai aperto per ogni notifica.

### Scheda Pratica

**Dati generali**

| Campo | Contenuto |
|---|---|
| **Numero pratica** | Il numero della notifica in GeoTecSUE. |
| **Anno** | L'anno. |
| **Tipo** | Il tipo di pratica. |
| **Stato** | Lo stato attuale. |
| **Descrizione dell'intervento** | Descrizione dell'intervento così come inserito dal professionista nella notifica. |
| **Registrata il**, **Ultima modifica**, **Inviata il** | Data e ora di creazione, ultima modifica e invio da parte del professionista. |

Sotto ci sono i pulsanti **Istanza (PDF)** e **Istanza firmata (P7M)** per scaricare il documento della notifica. Sono disattivati (grigi) se il file non è disponibile.

**Trasmissione a MUDE**

| Campo | Contenuto |
|---|---|
| **Numero istanza MUDE** | Il codice a 22 cifre assegnato da MUDE. È anche il codice che il professionista usa come "istanza di primo invio" per un eventuale aggiornamento della notifica. |
| **Trasmessa il** | Data e ora della trasmissione a MUDE. |

**Protocollazione su MUDE**

Compare solo quando la notifica ha superato lo stato di invio, cioè dopo la protocollazione.

| Campo | Contenuto |
|---|---|
| **Numero protocollo** | Il protocollo SPRESAL. |
| **Data protocollo** | La data del protocollo. |
| **Variazione di stato** | Data e ora in cui MUDE ha comunicato il cambio di stato. |
| **Oggetto della notifica MUDE** | L'oggetto comunicato da MUDE. |
| **Messaggio della notifica MUDE** | L'eventuale messaggio comunicato da MUDE. |

{: .warning }
> Il numero di protocollo di questa card non è un protocollo del tuo Ente: non usarlo come riferimento per le pratiche edilizie collegate.

### Scheda Soggetti

Contiene la card **Titolare**, con **Cognome e nome**, **Codice fiscale**, **Nascita**, **Residenza** ed **E-mail** del titolare, letti dai dati della notifica.

- Se il titolare rappresenta una ditta, una società o un ente compare il riquadro **Ditta / Società / Ente rappresentato** con **Denominazione**, **Partita IVA / C.F.**, **Sede**, **E-mail** e **PEC**.
- Se ci sono altri titolari compare la tabella **Altri titolari** con **Cognome**, **Nome**, **Codice fiscale** e **Data di nascita**.

Rispetto al dettaglio standard non c'è la card del professionista e non è possibile la voltura.

### Scheda Documenti

Tabella degli allegati della notifica, ordinata per data di inserimento:

| Colonna | Contenuto |
|---|---|
| **Inserito il** | Data e ora di caricamento. |
| **Documento** | La descrizione e, sotto, il nome del file. |
| **Disponibile fino al** | La data fino alla quale il file è scaricabile. Se è passata compare il badge "Scaduto il …". |
| *(ultima colonna)* | Il pulsante di scarico, disattivato se il documento è scaduto. |

Se non ci sono allegati la tabella mostra "Nessun documento allegato alla notifica.".

### Scheda Ricevute

Contiene la card **Ricevute della notifica** con due righe: **Ricevuta di invio** e **Ricevuta di protocollazione**.

| Badge | Significato | Pulsanti |
|---|---|---|
| **Disponibile** (verde) | La ricevuta è pronta. | **Rigenera**, **Scarica** |
| **In generazione** (giallo) | La notifica è stata inviata da meno di un'ora: ricarica la pagina tra qualche minuto. | **Rigenera** |
| **Non generata** (rosso) | La ricevuta manca. | **Rigenera** |
| **Non ancora prevista** | La notifica non è ancora protocollata: la ricevuta di protocollazione non esiste ancora. | Nessuno |

- Clicca su **Scarica** per scaricare il PDF della ricevuta.
- Clicca su **Rigenera** per crearla di nuovo. La pagina si ricarica e compare la notifica verde "Ricevuta di invio rigenerata" (o "di protocollazione"). Se la notifica non è ancora protocollata, la rigenerazione della ricevuta di protocollazione viene rifiutata con il messaggio "La notifica non è ancora stata protocollata su MUDE.".
  
### Scheda Storico

La card **Tracciabilità** elenca, dalla più recente, ogni operazione registrata sulla notifica, con **Data** e **Operazione** (ad esempio l'invio a MUDE e la protocollazione SPRESAL).

## Messaggi di errore

Se una parte della pagina non si riesce a caricare (ad esempio i dati MUDE), le altre vengono mostrate comunque e si apre la finestra **Attenzione** con l'elenco delle parti mancanti. Se il problema si ripete, segnala il numero della pratica all'assistenza.
