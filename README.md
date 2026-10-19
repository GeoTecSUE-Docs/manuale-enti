# Manuale Enti GeoTecSUE

Manuale operativo del **back office di GeoTecSUE** per gli uffici degli Enti, pubblicato con GitHub Pages
(Jekyll + tema [Just the Docs](https://just-the-docs.com/)), con la stessa impostazione del
[manuale per i professionisti](https://github.com/GeoTecSUE-Docs/manuale).

## Struttura

- `index.md` – pagina iniziale con l'indice
- `introduzione.md`, `impostazioni.md`, `gestione-pratiche.md`, `altre-funzioni.md` – sezioni del menu laterale
- `docs/` – una pagina per ogni voce di menu del back office
- `docs/appendici/` – stati delle pratiche e glossario
- `assets/images/` – schermate
- `CHANGELOG.md` – cronologia delle versioni

## Schermate da inserire

Nei punti in cui serve un'immagine c'è un riquadro viola **Schermata da inserire** con il nome del file previsto, ad esempio:

```markdown
{: .schermata }
> `assets/images/news-elenco.png` — elenco delle news con i pulsanti di modifica
```

Per inserirla: salva la cattura in `assets/images/` con quel nome e sostituisci il riquadro con

```markdown
![Elenco delle news](../assets/images/news-elenco.png)
```

(da `docs/appendici/` il percorso è `../../assets/images/...`).

## Punti da verificare

Nel sorgente delle pagine ci sono commenti `<!-- DA VERIFICARE: ... -->` (non visibili nel sito) dove il comportamento
dipende da servizi esterni o non è deducibile dal codice del back office. Per elencarli:

```bash
grep -rn "DA VERIFICARE" docs
```

## Anteprima in locale

```bash
bundle install
bundle exec jekyll serve
```
