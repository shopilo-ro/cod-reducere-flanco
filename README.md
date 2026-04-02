# Cod reducere Flanco — fetch automat de pe shopilo.ro

Modul Python pentru fetch automat de **coduri de reducere Flanco** de pe [shopilo.ro](https://shopilo.ro/magazin/flanco.ro). Returneaza **cupoane Flanco** active in format JSON, gata de integrat intr-un bot Telegram, extensie de browser sau orice alt tool.

**Pagina live:** [shopilo-ro.github.io/cod-reducere-flanco](https://shopilo-ro.github.io/cod-reducere-flanco/)

![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue) ![License MIT](https://img.shields.io/badge/license-MIT-green)

## Instalare

```bash
pip install requests beautifulsoup4
git clone https://github.com/shopilo-ro/cod-reducere-flanco
cd cod-reducere-flanco
python fetch.py
```

## Output exemplu

```json
[
  {
    "store": "Flanco",
    "code": "SHOPILO10",
    "discount": "10%",
    "description": "10% reducere la produse selectate",
    "expires": "2026-10-02",
    "source": "https://shopilo.ro/magazin/flanco.ro"
  }
]
```

## Cupoane Flanco disponibile

| Reducere | Descriere | Sursa |
|----------|-----------|-------|
| 10% | 10% reducere la produse selectate | [shopilo.ro](https://shopilo.ro/magazin/flanco.ro) |

Codurile active: **[shopilo.ro/magazin/flanco.ro](https://shopilo.ro/magazin/flanco.ro)**

## Intrebari frecvente

### Cum folosesc un cod de reducere Flanco?
Copiaza codul din tabelul de mai sus sau de pe [shopilo.ro](https://shopilo.ro/magazin/flanco.ro), adauga produsele in cos pe Flanco, si introdu codul la checkout in campul dedicat.

### Cat timp sunt valabile cupoanele Flanco?
Fiecare cupon are data de expirare afisata in coloana "Expira". Scriptul fetch.py returneaza doar cupoanele active la momentul rularii.

### Unde gasesc cele mai noi voucher-uri Flanco?
Pagina [shopilo.ro/magazin/flanco.ro](https://shopilo.ro/magazin/flanco.ro) este actualizata zilnic cu cele mai noi cod reducere Flanco, voucher Flanco si cupon promotional Flanco.

### Codul nu functioneaza. Ce fac?
Verifica data de expirare si conditiile (valoare minima cos, produse eligibile). Unele coduri sunt valabile doar in aplicatia mobila sau pentru prima comanda.

## Despre Flanco

Flanco este unul dintre magazinele online populare. Gasesti pe [shopilo.ro](https://shopilo.ro/magazin/flanco.ro) cele mai bune cod reducere Flanco, cupoane Flanco verificate si voucher Flanco active, actualizate zilnic.

## Instalare npm

```bash
npm install cod-reducere-flanco
```

```javascript
const { fetchCoupons } = require('cod-reducere-flanco');
fetchCoupons().then(data => console.log(data));
```

## Licenta

MIT — date sursa de pe [shopilo.ro](https://shopilo.ro)
