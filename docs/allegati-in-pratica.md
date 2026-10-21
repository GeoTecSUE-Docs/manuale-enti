---
title: Allegati in pratica
nav_order: 70
parent: "Impostazioni dell'Ente"
description: Come scegliere quali allegati richiedere in ciascun tipo di pratica e come impostarne obbligatorietà, firma digitale, tipo di file e condizione di obbligatorietà.
keywords: [allegati in pratica, allegati obbligatori, firma digitale, tipo di file, PDF, condizione di obbligatorietà, attivare allegato, disattivare allegato, tipi di pratica, impostazioni ente]
IDRegione: 99
IDTipoPratica: 9999
Fonte: Manuale Enti
---

# Allegati in pratica

Questa sezione spiega come decidere, per ogni tipo di pratica, quali allegati richiedere al professionista e con quali regole: obbligatorio o facoltativo, con o senza firma digitale, in quale formato di file.

## Accedere alla pagina

Dal menu in alto scegli **Impostazioni › Allegati in Pratica**. Si apre la pagina **Gestione Allegati in Pratica**.

## Differenza con la pagina Allegati

- Nella pagina [Allegati](allegati.html) gestisci il **catalogo** dell'Ente: titolo, descrizione e categoria di ogni tipo di allegato.
- In questa pagina **associ** gli allegati del catalogo ai tipi di pratica e ne imposti le regole, che valgono solo per la pratica scelta.

Lo stesso allegato può quindi essere obbligatorio e firmato in una pratica e facoltativo in un'altra. Se un allegato che ti serve non compare in nessuna delle due tabelle, crealo prima nella pagina [Allegati](allegati.html).

## Scegliere il tipo di pratica

1. Nel riquadro **Pratica** apri il menu **Tipo di pratica** (puoi scrivere per cercare).
2. Seleziona la pratica: la pagina si aggiorna e mostra le due tabelle degli allegati.

L'elenco contiene i tipi di pratica attivati per il tuo Ente (vedi [Tipi pratiche](tipi-pratiche.html)). Quando cambi pratica, i filtri e le ricerche delle tabelle vengono azzerati.

{: .schermata }
> `assets/images/allegati-in-pratica-tabelle.png` — La pagina con una pratica selezionata: tabella Allegati attivi con i badge Sì/No di Obbligatorio e Firma digitale e, sotto, la tabella degli allegati non attivi.

## Allegati attivi

Il riquadro **Allegati attivi** elenca gli allegati richiesti al professionista in questa pratica; il numero verde accanto al titolo ne indica il totale. Gli obbligatori sono elencati per primi, poi in ordine di titolo.

| Colonna | Contenuto |
|---------|-----------|
| **Titolo** | Nome dell'allegato |
| **Descrizione** | Descrizione (due righe; il testo completo passando il mouse sopra) |
| **Categoria** | Categoria dell'allegato |
| **Tipo file** | Formato di file accettato |
| **Obbligatorio** | Badge **Sì** (verde) o **No** (grigio), cliccabile; un'icona "i" blu indica che è stata scritta una condizione di obbligatorietà, che leggi passando il mouse sopra |
| **Firma digitale** | Badge **Sì** (verde) o **No** (grigio), cliccabile |
| (pulsanti) | Matita per tipo di file e condizione, pulsante rosso per disattivare |

### Filtrare gli allegati attivi

Sopra la tabella trovi:

- un menu di **categoria** ("Tutte le categorie" se vuoto);
- l'interruttore **Solo obbligatori**;
- l'interruttore **Solo con firma digitale**.

I filtri agiscono subito, senza ricaricare la pagina, e si sommano alla casella **Cerca** della tabella. La ricerca e la pagina della tabella restano memorizzate dopo ogni operazione (vedi [Interfaccia e convenzioni](interfaccia-e-convenzioni.html)).

### Rendere un allegato obbligatorio o facoltativo

Clicca sul badge nella colonna **Obbligatorio**: il valore si inverte subito (da **No** a **Sì** o viceversa) e compare la notifica "Allegato reso obbligatorio" o "Allegato reso facoltativo".

### Richiedere o togliere la firma digitale

Clicca sul badge nella colonna **Firma digitale**: il valore si inverte e compare la notifica "Firma digitale richiesta" o "Firma digitale non più richiesta".

{: .note }
> I badge non chiedono conferma: se clicchi per errore, clicca di nuovo per tornare al valore precedente.

### Impostare tipo di file e condizione di obbligatorietà

1. Clicca sulla **matita** nella riga dell'allegato.
2. Si apre una finestra con il titolo dell'allegato e, sotto, il nome della pratica.
3. Compila i campi:

   | Campo | Contenuto |
   |-------|-----------|
   | **Tipo di file accettato** | Il formato che il professionista deve caricare, scelto dall'elenco |
   | **Condizione di obbligatorietà** | Testo libero: indica quando l'allegato è obbligatorio, se lo è solo in alcuni casi (es. "Solo se l'intervento riguarda la facciata") |

4. Clicca su **Salva**: compare la notifica **Allegato salvato**.

### Disattivare un allegato per la pratica

1. Clicca sul pulsante rosso (cerchio barrato) nella riga dell'allegato.
2. Nella finestra **Disattivare l'allegato?** clicca su **Disattiva**.

L'allegato non verrà più richiesto in questa pratica e passa nella tabella sotto. Resta nel catalogo e nelle altre pratiche.

{: .warning }
> Disattivando un allegato perdi le sue impostazioni per questa pratica: se lo riattivi, obbligatorietà, firma e tipo di file andranno reimpostati.

### Azioni su tutti gli allegati della pratica

Nell'intestazione del riquadro **Allegati attivi** trovi due pulsanti che agiscono su **tutti** gli allegati attivi della pratica scelta (non solo su quelli visibili con i filtri):

| Pulsante | Effetto |
|----------|---------|
| **Tutti in PDF** | Imposta a PDF il tipo di file di tutti gli allegati attivi |
| **Tutti firmati digitalmente** | Richiede la firma digitale su tutti gli allegati attivi |

1. Clicca sul pulsante desiderato.
2. Leggi la domanda di conferma ("Richiedere tutti gli allegati in PDF?" oppure "Richiedere la firma digitale su tutti gli allegati?").
3. Clicca su **Conferma**.

{: .note }
> Non esiste un'azione inversa di massa: per togliere la firma o cambiare formato a singoli allegati usa i badge o la matita riga per riga.

## Allegati disponibili, non attivi in questa pratica

Il secondo riquadro elenca gli allegati del catalogo che **non** sono richiesti nella pratica scelta, con le colonne **Titolo**, **Descrizione** e **Categoria** e un menu per filtrare per categoria.

### Attivare un allegato nella pratica

1. Clicca su **Attiva** nella riga dell'allegato.
2. Nella finestra **Attivare l'allegato?** clicca su **Attiva**.

L'allegato passa tra gli **Allegati attivi** come **facoltativo** e **senza firma digitale**, con un tipo di file predefinito. Compare la notifica "Allegato attivato – Ora puoi impostare obbligatorietà, firma e tipo di file.": completa quindi le impostazioni come descritto sopra.

{: .warning }
> Le modifiche di questa pagina cambiano subito gli allegati richiesti ai professionisti per quel tipo di pratica, ma per una pratica in compilazione vale la regola di sempre: le impostazioni con cui è partito NON vengono modificate

## Pagine collegate

- [Allegati](allegati.html): il catalogo dei tipi di allegato (titolo, descrizione, categoria).
- [Modulistica](modulistica.html): modelli scaricabili collegati agli allegati.
- [Scheda Ente](scheda-ente.html): nel riquadro **Stampa allegati** generi il PDF della lista allegati per pratica.
