# Code promo easyJet, recuperation automatique depuis shopilo.fr

Module Python pour la recuperation automatique de **codes promo easyJet** depuis [shopilo.fr](https://shopilo.fr/reductions/easyjet.com). Renvoie les **coupons easyJet** actifs au format JSON, pret a etre integre dans un bot Telegram, une extension de navigateur ou tout autre outil.

**Page live :** [shopilo-fr.github.io/code-promo-easyjet](https://shopilo-fr.github.io/code-promo-easyjet/)

![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue) ![License MIT](https://img.shields.io/badge/license-MIT-green)

## Installation

```bash
pip install requests beautifulsoup4
git clone https://github.com/shopilo-fr/code-promo-easyjet
cd code-promo-easyjet
python fetch.py
```

## Exemple de sortie

```json
[
  {
    "store": "easyJet",
    "code": "SHOPILO10",
    "discount": "10%",
    "description": "10% de reduction sur les vols en Europe",
    "expires": "2026-10-13",
    "source": "https://shopilo.fr/reductions/easyjet.com"
  }
]
```

## Coupons easyJet disponibles

| Reduction | Description | Source |
|----------|-----------|-------|
| 10% | 10% de reduction sur les vols en Europe | [shopilo.fr](https://shopilo.fr/reductions/easyjet.com) |

Codes actifs : **[shopilo.fr/reductions/easyjet.com](https://shopilo.fr/reductions/easyjet.com)**

## Questions frequentes

### Comment utiliser un code promo easyJet ?
Copiez le code depuis le tableau ci-dessus ou depuis [shopilo.fr](https://shopilo.fr/reductions/easyjet.com), ajoutez les produits a votre panier sur easyJet et saisissez le code au moment du paiement dans le champ prevu.

### Combien de temps durent les coupons easyJet ?
Chaque coupon a une date d'expiration indiquee dans la colonne "Expiration". Le script fetch.py renvoie uniquement les coupons actifs au moment de l'execution.

### Ou trouver les bons de reduction easyJet les plus recents ?
La page [shopilo.fr/reductions/easyjet.com](https://shopilo.fr/reductions/easyjet.com) est mise a jour quotidiennement avec les codes promo easyJet, bons de reduction easyJet et coupons promotionnels easyJet les plus recents.

### Le code ne fonctionne pas. Que faire ?
Verifiez la date d'expiration et les conditions (montant minimum de commande, produits eligibles). Certains codes sont valables uniquement sur l'application mobile ou pour la premiere commande.

## A propos de easyJet

easyJet est l'une des boutiques en ligne les plus populaires. Sur [shopilo.fr](https://shopilo.fr/reductions/easyjet.com), retrouvez les meilleurs codes promo easyJet, coupons easyJet verifies et bons de reduction easyJet actifs, mis a jour chaque jour.

## Installation npm

```bash
npm install code-promo-easyjet
```

```javascript
const { fetchCoupons } = require('code-promo-easyjet');
fetchCoupons().then(data => console.log(data));
```

## Licence

MIT, donnees extraites de [shopilo.fr](https://shopilo.fr)
