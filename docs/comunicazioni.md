---
title: Comunicazioni
nav_order: 50
parent: "Impostazioni dell'Ente"
description: Come stabilire in quali tipi di pratica ogni comunicazione (inizio lavori, fine lavori, agibilità e altre) può essere presentata dal professionista e come ripristinare i collegamenti predefiniti.
keywords: [comunicazioni, inizio lavori, fine lavori, agibilità, collegamento pratiche, attivazione, disattivazione, impostazioni predefinite, ripristino, professionisti]
IDRegione: 99
IDTipoPratica: 9999
Fonte: Manuale Enti
---

# Comunicazioni

Questa sezione spiega come scegliere, per ogni tipo di comunicazione, in quali tipi di pratica il professionista può presentarla.

## A cosa serve

Le comunicazioni (ad esempio Inizio Lavori, Fine Lavori, Segnalazione Certificata di Agibilità) vengono presentate dal professionista a partire dal dettaglio di una pratica, con il pulsante **Nuova Comunicazione**.

Dal punto di vista del professionista, il menu **Seleziona il tipo di Comunicazione** di una pratica propone solo le comunicazioni che in questa pagina sono attive per quel tipo di pratica. Se una comunicazione manca, il manuale dei professionisti li invita a contattare l'Ente, che può abilitarla da qui.

## Accedere alla pagina

Dal menu in alto scegli **Impostazioni › Comunicazioni**.

Si apre la pagina **Gestione Comunicazioni**.

## Scegliere la comunicazione

Nella card **Comunicazione**:

1. Apri il menu **Tipo di comunicazione** (**-- Seleziona una comunicazione --**).
2. Scrivi parte del nome per filtrare l'elenco, oppure scorrilo.
3. Seleziona la comunicazione.

Sotto compare la card **Pratiche in cui è disponibile:** seguita dal nome della comunicazione.

Il menu elenca, in ordine alfabetico, i tipi attivi per l'Ente con tipologia **Comunicazione** (vedi [Tipi pratiche](tipi-pratiche.html#tipologia)). <!-- DA VERIFICARE: il filtro sulla tipologia Comunicazione è dedotto dai parametri della lettura, non esplicito --> Se non ce ne sono compare il messaggio **Nessuna comunicazione attiva: le comunicazioni si attivano da Gestione Tipologie Pratiche.**

Per svuotare la scelta clicca sulla **x** nel menu: la card delle pratiche scompare.

{: .schermata }
> `assets/images/comunicazioni-pratiche-collegate.png` — La pagina Gestione Comunicazioni con una comunicazione selezionata e l'elenco delle pratiche con i badge Attiva.

## Pratiche in cui è disponibile la comunicazione

La card mostra tutti i tipi di pratica attivi per l'Ente, in ordine alfabetico. In alto a destra un badge verde indica quante pratiche hanno la comunicazione attiva sul totale (ad esempio **5 su 12**).

| Colonna | Contenuto |
|---------|-----------|
| **Tipo pratica** | Nome del tipo di pratica |
| **Attiva** | Badge **Sì** (verde): la comunicazione è disponibile in questa pratica. Badge **No** (grigio): non è disponibile |

{: .note }
> La Notifica Preliminare non compare in questo elenco.

Se l'Ente non ha pratiche attive compare il messaggio **Nessuna pratica attiva.**

### Attivare o disattivare la comunicazione in una pratica

1. Clicca sul badge **No** per rendere disponibile la comunicazione in quel tipo di pratica.
2. Clicca sul badge **Sì** per toglierla.

La modifica è salvata subito: compare la notifica **Comunicazione attivata** oppure **Comunicazione disattivata** con il nome della pratica, e il conteggio nel badge si aggiorna.

{: .warning }
> Le modifiche hanno effetto subito sul portale dei professionisti: togliendo una comunicazione da un tipo di pratica, i professionisti non potranno più avviarla da quelle pratiche.

L'effetto della disattivazione sulle comunicazioni dello stesso tipo già in compilazione non è indicato in questa pagina. <!-- DA VERIFICARE: cosa succede alle comunicazioni già avviate dal professionista quando l'Ente disattiva il collegamento -->

## Ripristinare le impostazioni predefinite

Il pulsante **Ripristina predefinite**, in alto a destra nella card **Comunicazione**, ricollega tutte le comunicazioni alle pratiche come previsto dalla configurazione di base.

1. Clicca su **Ripristina predefinite**.
2. Si apre la finestra **Ripristinare le impostazioni predefinite?**
3. Clicca su **Ripristina** per confermare, oppure su **Annulla**.

La pagina si ricarica e compare la notifica **Impostazioni predefinite ripristinate**.

{: .warning }
> Il ripristino riguarda **tutte** le comunicazioni, non solo quella selezionata: come indica la finestra di conferma, **le personalizzazioni fatte da questa pagina andranno perse**.

{: .note }
> Quando attivi un tipo di pratica dalla pagina [Tipi pratiche](tipi-pratiche.html), le comunicazioni previste dalla configurazione di base vengono collegate automaticamente. Usa questa pagina per adattare poi i collegamenti alle esigenze dell'Ente.

## Messaggi e notifiche

Le notifiche verdi di conferma e la finestra **Attenzione** per gli errori seguono le convenzioni comuni del back office, descritte in [Interfaccia e convenzioni](interfaccia-e-convenzioni.html).
