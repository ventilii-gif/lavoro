# Lavoro ed energia

Web app didattica interattiva su **lavoro ed energia** per il liceo (biennio e
triennio), pensata *senza integrali*: dove servirebbe un'integrazione (per
esempio l'energia potenziale elastica) si usa l'**area sotto il grafico
forza–spostamento**.

Fa parte della serie di app pubblicate su [ventilii.ai](https://ventilii.ai).

## Contenuti

Un'introduzione con nota storica e cinque sezioni tematiche. Ogni sezione
contiene **teoria**, una **simulazione** interattiva, **esercizi guidati** con
suggerimenti progressivi e soluzione, e un **quiz** a risposta multipla.

1. Il lavoro di una forza — `L = F·s·cosθ`, lavoro motore/resistente/nullo.
2. Energia cinetica e teorema dell'energia cinetica — `Eₒ = ½mv²`, `L = ΔEₒ`.
3. Energia potenziale — gravitazionale `mgh` ed elastica `½kx²`, forze conservative.
4. Conservazione dell'energia meccanica — con e senza attrito (dissipazione in calore).
5. Potenza — `P = L/t`, `P = F·v`, watt e cavallo vapore.

## Caratteristiche tecniche

- **File unico** `index.html` (HTML + CSS + JS inline), nessuno step di build.
- Formule con **KaTeX** incluso localmente nella cartella `katex/` (nessuna
  dipendenza da CDN per la matematica).
- Tema **chiaro/scuro** con selettore, palette accessibile ai daltonici
  (nessuna coppia rosso/verde), layout responsive fino a smartphone.
- Simulazioni su `<canvas>`, ridisegnate in tempo reale al variare dei cursori.

## Pubblicazione

Online tramite **GitHub Pages** (Settings → Pages → *Deploy from a branch*,
selezionando il branch di pubblicazione e la cartella root). Il file `CNAME`
imposta il dominio `lavoro.ventilii.ai`.

## Uso in locale

Basta aprire `index.html` in un browser, oppure servire la cartella con un
server statico:

```bash
python3 -m http.server 8000
# poi apri http://localhost:8000
```
