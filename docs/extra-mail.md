---
title: Extra Mail
nav_order: 150
parent: "Impostazioni dell'Ente"
description: Spiega come aggiungere indirizzi email ulteriori che ricevono in copia le mail automatiche destinate all'Ente, anche per singolo Comune nelle Unioni.
keywords: [extra mail, altre email, destinatari aggiuntivi, copia mail, comune, unione, multiente, notifiche ente, indirizzo email]
IDRegione: 99
IDTipoPratica: 9999
Fonte: Manuale Enti
---

# Extra Mail

Questa sezione spiega come gestire gli indirizzi email aggiuntivi dell'Ente, cioè i destinatari che ricevono in copia le mail automatiche rivolte all'Ente.

## Differenza tra Mail ed Extra Mail

| Pagina | Cosa decide | Destinatari |
|--------|-------------|-------------|
| [Mail](mail.html) | **Per quali eventi** parte una mail automatica, e se verso l'Ente e/o verso il professionista. | L'indirizzo dell'Ente e il professionista della pratica. |
| **Extra Mail** | **A chi altro** inviare le mail rivolte all'Ente. | Gli indirizzi elencati in questa pagina (es. un tecnico istruttore, l'ufficio tributi, la casella di un singolo Comune dell'Unione). |

Gli indirizzi di Extra Mail:

- ricevono le stesse mail che partono **verso l'Ente** (colonna **All'ente** della pagina [Mail](mail.html)), solo per gli eventi attivati lì;
- **non** ricevono le mail rivolte al professionista;
- ricevono solo le mail delle pratiche del **Comune** a cui sono associati.

<!-- DA VERIFICARE: nel codice esaminato la copia agli Extra Mail è visibile solo per l'evento "Invio IUV da portale a ente"; confermare quali altri eventi "All'ente" (es. Invio pratica) la prevedono -->

{: .note }
> Le mail agli indirizzi aggiuntivi sono mail normali, non PEC.

## Accedere alla pagina

Dal menu in alto scegli **Impostazioni › Extra Mail**. La pagina si intitola **Gestione altre e-mail per Ente**.

## Elenco dei destinatari

La scheda **Destinatari abilitati** mostra gli indirizzi configurati; il badge accanto al titolo ne riporta il numero.

{: .schermata }
> `assets/images/extra-mail-elenco.png` — La scheda "Destinatari abilitati" con alcuni indirizzi, la colonna Comune e i pulsanti di modifica ed eliminazione.

| Colonna | Contenuto |
|---------|-----------|
| **Comune** | Comune a cui è associato l'indirizzo. Visibile solo se l'Ente gestisce più Comuni (ad esempio un'Unione). |
| **Indirizzo e-mail** | L'indirizzo del destinatario. Cliccandolo si apre il programma di posta per scrivergli. |
| (pulsanti) | **Modifica** (matita) ed **Elimina** (cestino). |

L'elenco è ordinato per Comune e indirizzo (per indirizzo negli Enti con un solo Comune) e ha **Cerca**, ordinamento e paginazione da 25 righe: vedi [Interfaccia e convenzioni](interfaccia-e-convenzioni.html). Se non ci sono destinatari compare *"Nessun destinatario: usa Nuovo destinatario per aggiungerne uno."*

## Aggiungere un destinatario

1. Clicca su **Nuovo destinatario**.
2. Si apre la finestra **Nuovo destinatario**.
3. Se l'Ente gestisce più Comuni, scegli il **Comune** dall'elenco (*"-- Seleziona il comune --"*). Se l'Ente ha un solo Comune il campo non compare: l'indirizzo è associato automaticamente al Comune dell'Ente.
4. Inserisci l'**Indirizzo e-mail**.
5. Clicca su **Salva** (o premi Invio).
6. Compare la notifica verde **Destinatario aggiunto** con l'indirizzo.

Per uscire senza salvare clicca su **Chiudi**.

### Controlli al salvataggio

Se qualcosa non va compare la finestra **Attenzione**; chiudendola si torna alla finestra del destinatario con i dati inseriti.

| Messaggio | Causa |
|-----------|-------|
| *"Selezionare il comune."* | Ente con più Comuni e nessun Comune scelto. |
| *"Inserire l'indirizzo e-mail."* | Indirizzo vuoto. |
| *"L'indirizzo e-mail non è valido."* | Indirizzo scritto in modo non corretto. |
| *"Questo indirizzo e-mail è già presente per il comune selezionato."* | Lo stesso indirizzo è già associato a quel Comune. |

{: .note }
> Lo stesso indirizzo può essere associato a più Comuni: aggiungilo una volta per ciascun Comune di cui deve ricevere le mail.

## Modificare un destinatario

1. Clicca sulla matita nella riga del destinatario.
2. Si apre la finestra **Modifica destinatario** con i dati attuali.
3. Cambia l'**Indirizzo e-mail** e, se presente, il **Comune**.
4. Clicca su **Salva**: compare la notifica **Destinatario salvato**.

## Eliminare un destinatario

1. Clicca sul cestino nella riga del destinatario.
2. Si apre la finestra **Eliminare il destinatario?** con l'indirizzo (e il Comune) e l'avviso *"Non riceverà più le e-mail."*
3. Clicca su **Elimina** per confermare, oppure su **Annulla**.
4. Compare la notifica **Destinatario eliminato**.

{: .warning }
> L'eliminazione è immediata: da quel momento l'indirizzo non riceve più le mail dell'Ente.
