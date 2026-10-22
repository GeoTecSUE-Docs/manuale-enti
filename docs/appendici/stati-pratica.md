---
title: Stati delle pratiche
nav_order: 1
parent: Appendici
description: Elenca gli stati che una pratica può assumere su GeoTecSUE visti dal back office dell'Ente, con significato, chi li imposta, colore del badge e operazioni possibili.
keywords: [stati pratica, ciclo di vita, inviata, protocollata, registrata, esecutiva, archiviata, diniego, integrazioni, revoca delegato, colori badge, verificata]
IDRegione: 99
IDTipoPratica: 9999
Fonte: Manuale Enti
---

# Stati delle pratiche

Questa appendice spiega gli stati che una pratica può assumere su GeoTecSUE visti dal back office dell'Ente: cosa significano, chi li imposta, con quale colore compaiono e cosa puoi fare dal back office in ciascuno.

## Chi imposta gli stati

- **Professionista**: compila, firma e trasmette dal proprio portale; trasmette integrazioni e richieste di archiviazione.
- **Sistema**: esegue in automatico alcuni passaggi, come la protocollazione automatica o gli stati delle notifiche preliminari.
- **Ente**: lavora la pratica. Dal back office puoi protocollare manualmente (se attivo) e riportare una pratica allo stato precedente; gli altri stati di istruttoria (registrazione, richiesta integrazioni, provvedimento, archiviazione, diniego…) sono aggiornati dalle procedure dell'Ente collegate a GeoTecSUE e qui si consultano. <!-- DA VERIFICARE: gli stati di istruttoria arrivano dal gestionale dell'Ente collegato (la pagina Mail parla di registrazione "su Sequoia"); non si impostano da questo back office -->

## Stati prima dell'invio

Queste pratiche sono ancora presso il professionista. Non compaiono in [Pratiche e comunicazioni trasmesse](../pratiche-trasmesse.html); puoi vederle in [Pratiche in corso](../pratiche-in-corso.html).

| Stato | Significato | Chi lo imposta | Badge |
|-------|-------------|----------------|-------|
| **In Creazione** | Istanza appena creata, non ancora salvata | Professionista | — |
| **In Compilazione** | Istanza salvata ma incompleta | Professionista | — |
| **Completata** | Istanza validata, pronta per la firma o l'invio | Professionista; oppure l'Ente quando riporta indietro una pratica **Inviata** | — |
| **Firmata** | Istanza firmata digitalmente e ricaricata | Professionista; oppure l'Ente quando riporta indietro una pratica **Inviata**, se l'Ente richiede il p7m | — |

## Stati di lavorazione

Sono gli stati che trovi nel filtro **Stato pratica** di [Pratiche e comunicazioni trasmesse](../pratiche-trasmesse.html).

| Stato | Significato | Chi lo imposta | Badge | Cosa puoi fare dal back office |
|-------|-------------|----------------|-------|--------------------------------|
| **Inviata** | Trasmessa all'Ente, in attesa di protocollo | Professionista (invio) | Arancione | Protocollare manualmente, se attivo ([Gestione protocollazione](../gestione-protocollazione.html)); riportarla allo stato precedente con una motivazione ([Dettaglio della pratica](../dettaglio-pratica.html#riporta-la-pratica-allo-stato-precedente)) |
| **Protocollata** | Ha numero e data di protocollo | Sistema (protocollazione automatica) oppure Ente (protocollazione manuale) | Azzurro | Consultare e attendere la registrazione |
| **Registrata** | Presa in carico dall'ufficio, con numero di pratica dell'Ente | Ente | Neutro | Consultare i dati di istruttoria nella scheda **Ente** |
| **Richiesta Integrazioni** | L'Ente ha chiesto documenti al professionista | Ente | Giallo | Seguire la richiesta nel riquadro **Da fare su questa pratica** e nella scheda **Ente** |
| **Invio Integrazioni** | Il professionista ha trasmesso le integrazioni | Professionista | Giallo | Protocollare l'integrazione, se la protocollazione manuale è attiva: la pratica torna **Registrata** (o **Esecutiva** se ha già un provvedimento) |
| **Richiesta Archiviazione** | Il professionista ha chiesto di archiviare la pratica | Professionista | Giallo | Consultare la richiesta |
| **Esecutiva** | Provvedimento favorevole rilasciato | Ente | Verde | Consultare il provvedimento nella scheda **Ente**; la pratica resta operativa per comunicazioni e integrazioni |
| **Verificata** (non usato) | Pratica controllata dall'Ente (es. SCIA, CILA) | Ente | Verde | Non viene trasmesso questo stato al professionista ma rimane un concetto inetrno all'Ente (solo su Sequoia) |

## Stati finali

| Stato | Significato | Chi lo imposta | Badge | Cosa puoi fare dal back office |
|-------|-------------|----------------|-------|--------------------------------|
| **Archiviata** | Pratica chiusa definitivamente | Ente | Rosso | Consultare e scaricare i documenti |
| **Diniego** | Pratica respinta dopo l'istruttoria | Ente | Rosso | Consultare e scaricare i documenti |
| **Rifiutata** | Respinta prima della protocollazione (procedura in disuso) | Ente | Rosso | Consultare |
| **Revoca Delegato** | Il titolare ha revocato il professionista | Ente | Rosso | Volturare la pratica a un altro professionista: torna allo stato che aveva prima della revoca ([Dettaglio della pratica](../dettaglio-pratica.html#professionista-e-voltura)) |

## Stati delle notifiche preliminari (Piemonte)

Riguardano solo le notifiche preliminari dei Comuni piemontesi, consultabili in [Notifiche preliminari](../notifiche-preliminari.html).

| Stato | Significato | Chi lo imposta | Badge |
|-------|-------------|----------------|-------|
| **Inviata SPRESALWEB (via MUDE)** | Notifica trasmessa a MUDE per SPRESALWEB | Sistema | Arancione |
| **Protocollata SPRESALWEB** | Notifica protocollata da SPRESAL; è lo stato finale | Sistema | Verde |

## Operazioni possibili in qualsiasi stato

Su una pratica trasmessa, qualunque sia lo stato, dal [Dettaglio della pratica](../dettaglio-pratica.html) puoi sempre:

- consultare dati, soggetti, documenti, comunicazioni e storico;
- scaricare l'archivio .zip e le ricevute disponibili, e rigenerare le ricevute mancanti;
- volturare la pratica a un altro professionista;
- indicare il referente dei pagamenti PagoPA tra i titolari dopo voltura e aggiornare lo stato dei pagamenti;
- consentire o revocare l'invio libero di integrazioni, se l'Ente non lo ha attivato per tutte le pratiche.

{: .note }
> Il professionista vede gli stessi stati nel proprio portale. Per lo stato **Verificata** il manuale dei professionisti indica che non viene mostrato al professionista, che continua a vedere **Registrata** o **Esecutiva** (è un concetto interno all'Ente)
