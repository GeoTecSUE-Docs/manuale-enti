---
title: Trasmissioni Regione Lombardia
nav_order: 100
parent: Gestione pratiche
description: Spiega come consultare e filtrare le trasmissioni delle pratiche a Regione Lombardia e come aprire il riepilogo di ogni trasmissione.
keywords: [Regione Lombardia, interoperabilità, trasmissioni, fase di aggiornamento, codice pratica R.L., procedimento R.L., integrazioni, aggiornamento finale, filtri, riepilogo]
IDRegione: 99
IDTipoPratica: 9999
Fonte: Manuale Enti
---

# Trasmissioni Regione Lombardia

Questa sezione spiega come consultare le trasmissioni delle pratiche del tuo Ente verso Regione Lombardia, filtrarle e aprirne il riepilogo o il dettaglio della pratica.

La pagina è di sola consultazione: da qui non si avviano né si ripetono trasmissioni. <!-- DA VERIFICARE: le trasmissioni a Regione Lombardia sono eseguite in automatico dal sistema -->

## Accedere alla pagina

Dal menu in alto scegli **Gestione Pratiche › Trasmissioni Regione Lombardia**.

{: .note }
> La voce di menu compare solo per gli Enti della Regione Lombardia.

La pagina si intitola **Trasmissioni a Regione Lombardia**.

{: .schermata }
> `assets/images/trasmissioni-regione-lombardia-elenco.png` — La card "Ultime trasmissioni" con i filtri, la tabella con i badge di fase colorati e i pulsanti riepilogo e dettaglio.

## Ultime trasmissioni e ricerca

All'apertura, senza filtri, la card si intitola **Ultime trasmissioni** e mostra solo le **ultime 10 trasmissioni** (lo ricorda la nota *Senza filtri sono mostrate solo le ultime 10 trasmissioni.*). Quando applichi almeno un filtro il titolo diventa **Trasmissioni trovate** e vengono mostrate tutte quelle che corrispondono.

Accanto al titolo trovi il numero di trasmissioni e, se ci sono filtri attivi, il badge giallo con il loro numero.

### Filtri

| Filtro | Cosa cerca |
|--------|-----------|
| **Fase di aggiornamento** | **Tutte**, **Primo aggiornamento**, **Integrazioni**, **Aggiornamento finale** |
| **Tipo procedimento R.L.** | Il tipo di procedimento regionale (**Tutti** per non filtrare) |
| **Tipo pratica** | Il tipo di pratica GeoTecSUE (**Tutti** per non filtrare) |
| **Codice pratica R.L.** | Il codice attribuito da Regione Lombardia |
| **# Pratica** | Il numero della pratica GeoTecSUE |
| **Data di trasmissione** dal / al | Intervallo della data di trasmissione |

1. Compila uno o più filtri.
2. Clicca su **Filtra** (oppure premi Invio in un campo).
3. Per tornare alle ultime 10 trasmissioni clicca su **Rimuovi filtri**.

Se una data non è valida o l'intervallo è invertito si apre la finestra **Attenzione** con il motivo (es. *Nell'intervallo della data di trasmissione la data iniziale è successiva a quella finale.*).

I filtri vengono conservati quando apri il dettaglio di una pratica e torni con **Ritorna**; riaprendo la pagina dal menu ripartono vuoti.

## La tabella

La tabella è ordinata per data di trasmissione, dalla più recente, e ha ricerca libera, ordinamento e paginazione (vedi [Interfaccia e convenzioni](interfaccia-e-convenzioni.html)).

| Colonna | Contenuto |
|---------|-----------|
| **Trasmessa il** | Data e ora della trasmissione |
| **Ente** | Compare solo se nell'elenco ci sono trasmissioni di più Enti |
| **Fase** | Badge della fase di aggiornamento |
| **# Pratica** | Numero della pratica (link al dettaglio) e, sotto, il tipo di pratica |
| **Codice pratica R.L.** | Codice regionale della pratica |
| **ID R.L.** | Identificativo regionale; per la fase **Integrazioni** è l'identificativo dell'integrazione |
| **Procedimento R.L.** | Tipo di procedimento regionale |
| (pulsanti) | Riepilogo della trasmissione e dettaglio della pratica |

| Badge di fase | Colore |
|---------------|--------|
| **Primo aggiornamento** | Azzurro |
| **Integrazioni** | Giallo |
| **Aggiornamento finale** | Verde |

## Riepilogo di una trasmissione

1. Clicca sul pulsante grigio (scheda) a destra della riga.
2. Si apre la finestra con titolo Ente e fase, divisa in tre parti:
   - **Trasmissione**: **Trasmessa il**, **Procedimento R.L.**, **ID pratica R.L.**, **ID integrazione R.L.**, **Codice pratica R.L.**;
   - **Pratica**: **Numero pratica**, **Stato**, **Inviata il**, **Tipo pratica**, **Protocollo**, **Registrazione**;
   - **Soggetti**: **Titolare**, **Codice fiscale titolare**, **Professionista**, **Codice fiscale professionista**.
3. Clicca su **Apri la pratica** per andare al dettaglio, oppure su **Chiudi**.

## Aprire il dettaglio della pratica

Clicca sul numero della pratica, sulla lente a destra della riga o su **Apri la pratica** nel riepilogo. Si apre il [Dettaglio della pratica](dettaglio-pratica.html); se la trasmissione riguarda una comunicazione si apre la pratica a cui la comunicazione si riferisce. Nel dettaglio, la scheda **Storico** riporta la card **Interoperabilità con Regione Lombardia** con tutte le trasmissioni di quella pratica.

Con **Ritorna** torni a questa pagina con gli stessi filtri.
