---
title: Gestione professionisti
nav_order: 20
parent: PagoPA, professionisti e assistenze
description: Come consultare l'elenco dei professionisti che operano con l'Ente e copiare o scaricare i loro indirizzi e-mail e PEC
keywords: [professionisti, elenco professionisti, e-mail, PEC, indirizzi, copia indirizzi, scarica indirizzi, codice fiscale, comunicazioni ai professionisti, Ccn]
IDRegione: 99
IDTipoPratica: 9999
Fonte: Manuale Enti
---

# Gestione professionisti

Questa sezione spiega come consultare l'elenco dei professionisti che operano con il tuo Ente e come raccogliere in un colpo solo i loro indirizzi e-mail o PEC, per esempio per inviare un avviso a tutti.

## Accedere alla pagina

Clicca sulla voce **Gestione Professionisti** nella barra di menu in alto.

La pagina si intitola **Gestione professionisti** e contiene il riquadro **Professionisti che operano con l'Ente**. Accanto al titolo un badge grigio indica quanti professionisti sono presenti.
I professionisti che vengono mostrati sono tutti quelli che hanno fatto almeno una volta un accesso al portale GeoTecSUE (anche senza aver mai inviato un'istanza all'Ente)

{: .schermata }
> `assets/images/gestione-professionisti-elenco.png` — La pagina Gestione professionisti con l'elenco e, in alto a destra, i pulsanti Copia e-mail e Copia PEC con i relativi pulsanti di scarico.

## L'elenco dei professionisti

L'elenco è una tabella con ricerca, ordinamento e paginazione (vedi [Interfaccia e convenzioni](interfaccia-e-convenzioni.html)). All'apertura è ordinato per **Cognome** e poi per **Nome**. Pagina, ordinamento e ricerca vengono ricordati se torni sulla pagina durante la stessa sessione del browser.

| Colonna | Contenuto |
|---------|-----------|
| **Cognome** | Cognome del professionista, in maiuscolo |
| **Nome** | Nome del professionista, in maiuscolo |
| **Codice fiscale** | Codice fiscale, in maiuscolo |
| **E-mail** | Indirizzo e-mail; clicca sull'indirizzo per aprire il tuo programma di posta con un nuovo messaggio indirizzato al professionista |
| **PEC** | Indirizzo PEC; anche questo si apre nel programma di posta |

Se un dato non è presente compare un trattino (—).

Usa il campo **Cerca** per trovare rapidamente un professionista per cognome, codice fiscale o indirizzo.

{: .note }
> La pagina è di sola consultazione: da qui non puoi modificare i dati dei professionisti.

## Copiare gli indirizzi e-mail o PEC

In alto a destra nel riquadro trovi due gruppi di pulsanti, uno per le e-mail e uno per le PEC.

Per copiare gli indirizzi:
1. Clicca su **Copia e-mail** (oppure su **Copia PEC**).
2. Compare la notifica verde, ad esempio "**42 indirizzi e-mail copiati**", con il suggerimento "Puoi incollarli nel campo Ccn di una mail.".
3. Apri il tuo programma di posta e incolla gli indirizzi nel campo del destinatario che preferisci.

Gli indirizzi vengono copiati:
- separati da punto e virgola e spazio ("; "), il formato accettato dai programmi di posta;
- senza doppioni (due indirizzi uguali, anche con maiuscole diverse, vengono copiati una sola volta);
- saltando i professionisti che non hanno l'indirizzo.

{: .warning }
> I pulsanti copiano **tutti** gli indirizzi dell'elenco, anche se hai usato il campo **Cerca** per restringere la tabella. Incolla gli indirizzi nel campo **Ccn** (copia nascosta): così ogni professionista non vede gli indirizzi degli altri.

## Scaricare gli indirizzi in un file

Accanto a ciascun pulsante di copia c'è un pulsante con l'icona di download:
- quello accanto a **Copia e-mail** scarica il file `lista_email.txt`;
- quello accanto a **Copia PEC** scarica il file `lista_PEC.txt`.

Il file di testo contiene gli stessi indirizzi della copia (tutti, senza doppioni, separati da "; "). È utile quando la copia negli appunti non funziona o quando vuoi conservare l'elenco.

## Messaggi di errore

I messaggi compaiono nella finestra **Attenzione**.

| Messaggio | Quando compare |
|-----------|----------------|
| "Nessun indirizzo e-mail da copiare." / "Nessun indirizzo PEC da copiare." | Nessun professionista dell'elenco ha quel tipo di indirizzo |
| "Nessun indirizzo e-mail da scaricare." / "Nessun indirizzo PEC da scaricare." | Come sopra, quando usi il pulsante di scarico |
| "Non è stato possibile copiare gli indirizzi: usa il pulsante di scarico." | Il browser non ha consentito la copia negli appunti; scarica il file di testo |
| "Si è verificato un errore durante la lettura/elaborazione dei dati" | Errore generico durante il caricamento dell'elenco |
| "Errore API: …" | Il servizio che fornisce i dati ha restituito un errore; il messaggio ne riporta il codice |
