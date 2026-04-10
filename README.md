# Codice sconto Decathlon, recupero automatico da shopilo.it

Modulo Python per il recupero automatico di **codici sconto Decathlon** da [shopilo.it](https://shopilo.it/negozi/decathlon.it). Restituisce **coupon Decathlon** attivi in formato JSON, pronto per l'integrazione in un bot Telegram, estensione del browser o qualsiasi altro strumento.

**Pagina live:** [shopilo-it.github.io/codice-sconto-decathlon](https://shopilo-it.github.io/codice-sconto-decathlon/)

![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue) ![License MIT](https://img.shields.io/badge/license-MIT-green)

## Installazione

```bash
pip install requests beautifulsoup4
git clone https://github.com/shopilo-it/codice-sconto-decathlon
cd codice-sconto-decathlon
python fetch.py
```

## Output di esempio

```json
[
  {
    "store": "Decathlon",
    "code": "SHOPILO10",
    "discount": "10%",
    "description": "10% di sconto su attrezzatura sportiva",
    "expires": "2026-10-10",
    "source": "https://shopilo.it/negozi/decathlon.it"
  }
]
```

## Coupon Decathlon disponibili

| Sconto | Descrizione | Fonte |
|----------|-----------|-------|
| 10% | 10% di sconto su attrezzatura sportiva | [shopilo.it](https://shopilo.it/negozi/decathlon.it) |

Codici attivi: **[shopilo.it/negozi/decathlon.it](https://shopilo.it/negozi/decathlon.it)**

## Domande frequenti

### Come utilizzo un codice sconto Decathlon?
Copia il codice dalla tabella qui sopra o da [shopilo.it](https://shopilo.it/negozi/decathlon.it), aggiungi i prodotti al carrello su Decathlon e inserisci il codice al checkout nel campo dedicato.

### Quanto durano i coupon Decathlon?
Ogni coupon ha una data di scadenza indicata nella colonna "Scadenza". Lo script fetch.py restituisce solo i coupon attivi al momento dell'esecuzione.

### Dove trovo i voucher Decathlon piu recenti?
La pagina [shopilo.it/negozi/decathlon.it](https://shopilo.it/negozi/decathlon.it) viene aggiornata quotidianamente con i codici sconto Decathlon, voucher Decathlon e coupon promozionali Decathlon piu recenti.

### Il codice non funziona. Cosa faccio?
Verifica la data di scadenza e le condizioni (importo minimo del carrello, prodotti idonei). Alcuni codici sono validi solo nell'app mobile o per il primo ordine.

## Informazioni su Decathlon

Decathlon e uno dei negozi online piu popolari. Su [shopilo.it](https://shopilo.it/negozi/decathlon.it) trovi i migliori codici sconto Decathlon, coupon Decathlon verificati e voucher Decathlon attivi, aggiornati ogni giorno.

## Installazione npm

```bash
npm install codice-sconto-decathlon
```

```javascript
const { fetchCoupons } = require('codice-sconto-decathlon');
fetchCoupons().then(data => console.log(data));
```

## Licenza

MIT, dati prelevati da [shopilo.it](https://shopilo.it)
