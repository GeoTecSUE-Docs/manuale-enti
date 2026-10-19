---
title: Gestione protocollazione
nav_order: 80
parent: Gestione pratiche
description: Spiega come protocollare manualmente le istanze trasmesse quando l'Ente non ha un protocollo informatico collegato a GeoTecSUE.
keywords: [protocollazione manuale, istanze da protocollare, numero di protocollo, data di protocollo, archivio zip, comunicazioni, integrazioni, pratica di riferimento, notifica professionista]
IDRegione: 99
IDTipoPratica: 9999
Fonte: Manuale Enti
---

# Gestione protocollazione

Questa sezione spiega come protocollare manualmente le istanze trasmesse dai professionisti (pratiche, comunicazioni e integrazioni) quando il tuo Ente non ha un protocollo informatico collegato a GeoTecSUE.

## Accedere alla pagina

Dal menu in alto scegli **Gestione Pratiche › Gestione Protocollazione**.

{: .note }
> La voce di menu è visibile solo se per il tuo Ente è attiva la protocollazione manuale. <!-- DA VERIFICARE: l'opzione non si imposta dal back office; indicare chi la attiva e se serve rientrare o aprire la Scheda Ente perché la voce compaia --> Negli Enti con protocollazione automatica le pratiche passano da **Inviata** a **Protocollata** senza intervento dell'ufficio.

La pagina si intitola **Gestione protocollazione**.

{: .schermata }
> `assets/images/gestione-protocollazione-elenco.png` — Il riquadro azzurro "Protocollazione" aperto su un'istanza, con i campi numero e data di protocollo, e sotto l'elenco "Istanze da protocollare" con la riga selezionata evidenziata.

## Elenco delle istanze da protocollare

La card **Istanze da protocollare** mostra, con un contatore, tutte le istanze del tuo Ente in attesa di protocollo. L'elenco parte dalle più vecchie, cioè quelle in attesa da più tempo. Ha la ricerca libera (**Cerca**), l'ordinamento per colonna e la paginazione (vedi [Interfaccia e convenzioni](interfaccia-e-convenzioni.html)).

| Colonna | Contenuto |
|---------|-----------|
| **# Pratica** | Numero dell'istanza; cliccandolo apri il riquadro di protocollazione |
| **Tipo** | Tipo di pratica, comunicazione o integrazione |
| **Inviata il** | Data e ora di trasmissione |
| **Titolare** | Titolare; per le integrazioni è quello della pratica di riferimento |
| **Professionista** | Professionista che ha trasmesso l'istanza |
| **Protocolla** | Apre il riquadro di protocollazione |

Se non ci sono istanze compare *Nessuna istanza da protocollare.*

## Protocollare un'istanza

1. Clicca su **Protocolla** (o sul numero) nella riga dell'istanza.
2. In alto si apre il riquadro **Protocollazione: …** con tipo e numero; la riga scelta è evidenziata nell'elenco.
3. Controlla i dati: **Tipo pratica**, **Numero pratica**, **Inviata il**, **Titolare**, **Professionista**.
4. Se ti serve il materiale da caricare nel tuo protocollo, clicca su **Scarica .zip per il protocollo** (vedi sotto).
5. Inserisci il **Numero di protocollo** (obbligatorio, numero intero positivo).
6. Controlla la **Data di protocollo** (obbligatoria): è proposta la data di oggi; dal calendario non puoi scegliere date future.
7. Clicca su **Protocolla**.
8. Nella finestra **Protocollare la pratica?** verifica istanza, numero e data e clicca su **Protocolla**.

La pagina si ricarica: l'istanza esce dall'elenco e compare la notifica verde *Pratica n. … protocollata (n. … del …)*.

{: .warning }
> La protocollazione non si annulla dal back office e ha effetto verso il professionista. Riceve nel portale una notifica (**Pratica Protocollata**, **Comunicazione Protocollata** o **Integrazioni Protocollate**, secondo il tipo di istanza) con numero e data di protocollo. Se nella pagina [Mail](mail.html) l'evento **Protocollazione pratica** è abilitato per il professionista, riceve anche un messaggio via mail normale, PEC o entrambe, secondo il **Tipo notifica** della [Scheda Ente](scheda-ente.html).

Per chiudere il riquadro senza protocollare clicca su **Chiudi**: numero e data inseriti vengono cancellati.

### Comunicazioni e integrazioni

Se l'istanza è una comunicazione o un'integrazione, nel riquadro compare anche **Pratica di riferimento** con **Tipo pratica**, **Numero pratica**, **Numero pratica dell'Ente** e **Protocollo** della pratica a cui si riferisce (anche se si tratta di una pratica importata).

Dopo la protocollazione di un'integrazione la pratica di riferimento torna allo stato **Registrata**, oppure **Esecutiva** se ha già un provvedimento. Dopo la protocollazione di una comunicazione la pratica di riferimento resta nel suo stato. <!-- DA VERIFICARE: il cambio di stato è eseguito dal server; nel back office si vede solo la registrazione nella tracciabilità -->

### Scarica .zip per il protocollo

1. Clicca su **Scarica .zip per il protocollo**.
2. Attendi la preparazione (compare lo spinner).
3. Il browser scarica il file `<numero pratica> - <acronimo>.zip`.

L'archivio contiene la documentazione dell'istanza da caricare nel tuo sistema di protocollo. <!-- DA VERIFICARE: il contenuto dello zip per il protocollo è preparato dal server e non è visibile nel codice --> È temporaneo e viene eliminato dopo lo scarico. Se non riesce compare *Non è stato possibile creare l'archivio per il protocollo* oppure *L'archivio per il protocollo non è disponibile: riprova a generarlo.*

### Consultare il dettaglio prima di protocollare

Clicca su **Dettaglio della pratica**: si apre il [Dettaglio della pratica](dettaglio-pratica.html) (per comunicazioni e integrazioni, quello della pratica di riferimento). Con **Ritorna** torni a questa pagina con la stessa istanza già aperta nel riquadro.

Puoi anche protocollare direttamente dal dettaglio, nel riquadro **Da fare su questa pratica**: al termine torni a questa pagina.

## Messaggi di errore

| Messaggio | Causa |
|-----------|-------|
| *Inserisci il numero di protocollo (un numero intero).* | Numero vuoto o non numerico |
| *Inserisci la data di protocollo nel formato gg/mm/aaaa.* | Data vuota o scritta male |
| *La data di protocollo non può essere futura.* | Data successiva a oggi |
| *La pratica non è più da protocollare: ricarica la pagina.* | L'istanza è già stata protocollata o non è più nello stato **Inviata** |
| *Pratica non trovata: ricarica la pagina.* | L'istanza non è più disponibile |
| *Non è stato possibile protocollare la pratica.* | Il server non ha accettato l'operazione (segue l'eventuale dettaglio dell'errore) |
