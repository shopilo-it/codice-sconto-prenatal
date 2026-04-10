# Codice sconto Prenatal, recupero automatico da shopilo.it

Modulo Python per il recupero automatico di **codici sconto Prenatal** da [shopilo.it](https://shopilo.it/negozi/prenatal.it). Restituisce **coupon Prenatal** attivi in formato JSON, pronto per l'integrazione in un bot Telegram, estensione del browser o qualsiasi altro strumento.

**Pagina live:** [shopilo-it.github.io/codice-sconto-prenatal](https://shopilo-it.github.io/codice-sconto-prenatal/)

![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue) ![License MIT](https://img.shields.io/badge/license-MIT-green)

## Installazione

```bash
pip install requests beautifulsoup4
git clone https://github.com/shopilo-it/codice-sconto-prenatal
cd codice-sconto-prenatal
python fetch.py
```

## Output di esempio

```json
[
  {
    "store": "Prenatal",
    "code": "SHOPILO10",
    "discount": "10%",
    "description": "10% di sconto su abbigliamento neonato e bambino",
    "expires": "2026-10-10",
    "source": "https://shopilo.it/negozi/prenatal.it"
  }
]
```

## Coupon Prenatal disponibili

| Sconto | Descrizione | Fonte |
|----------|-----------|-------|
| 10% | 10% di sconto su abbigliamento neonato e bambino | [shopilo.it](https://shopilo.it/negozi/prenatal.it) |

Codici attivi: **[shopilo.it/negozi/prenatal.it](https://shopilo.it/negozi/prenatal.it)**

## Domande frequenti

### Come utilizzo un codice sconto Prenatal?
Copia il codice dalla tabella qui sopra o da [shopilo.it](https://shopilo.it/negozi/prenatal.it), aggiungi i prodotti al carrello su Prenatal e inserisci il codice al checkout nel campo dedicato.

### Quanto durano i coupon Prenatal?
Ogni coupon ha una data di scadenza indicata nella colonna "Scadenza". Lo script fetch.py restituisce solo i coupon attivi al momento dell'esecuzione.

### Dove trovo i voucher Prenatal piu recenti?
La pagina [shopilo.it/negozi/prenatal.it](https://shopilo.it/negozi/prenatal.it) viene aggiornata quotidianamente con i codici sconto Prenatal, voucher Prenatal e coupon promozionali Prenatal piu recenti.

### Il codice non funziona. Cosa faccio?
Verifica la data di scadenza e le condizioni (importo minimo del carrello, prodotti idonei). Alcuni codici sono validi solo nell'app mobile o per il primo ordine.

## Informazioni su Prenatal

Prenatal e uno dei negozi online piu popolari. Su [shopilo.it](https://shopilo.it/negozi/prenatal.it) trovi i migliori codici sconto Prenatal, coupon Prenatal verificati e voucher Prenatal attivi, aggiornati ogni giorno.

## Installazione npm

```bash
npm install codice-sconto-prenatal
```

```javascript
const { fetchCoupons } = require('codice-sconto-prenatal');
fetchCoupons().then(data => console.log(data));
```

## Licenza

MIT, dati prelevati da [shopilo.it](https://shopilo.it)
