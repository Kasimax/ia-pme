# 🤖 Assistant IA PME — 49€/mois

**Votre assistant IA d'entreprise, opérationnel en 24h.**

> Rédigez vos emails, générez vos devis, répondez à vos clients — automatiquement.

## 🌐 Demo

👉 **[Voir la landing page](https://kasimax.github.io/ia-pme/)**  
👉 **[Tester le chat](https://kasimax.github.io/ia-pme/chat.html?demo=true)**  
👉 **[Souscrire — 49€/mois](https://buy.stripe.com/dRm4gt5Ha3P0fZkcNtdIA02)**

## ✨ Fonctionnalités

- ✉️ Rédaction d'emails professionnels
- 📄 Génération de devis
- 💬 FAQ client automatique
- 📝 Résumé de réunions et rapports
- 🎯 Rédaction commerciale (posts, fiches produits)

## 🛠️ Architecture

```
ia-pme/
├── index.html          # Landing page
├── chat.html           # Interface de chat
├── merci.html          # Page post-paiement
└── clients/            # Profils IA clients (JSON)

automation/
├── ia-pme-provisioner.js   # Serveur port 3341 (webhook Stripe + API chat)
└── ia-pme-campaign.js      # Campagne email (50/jour)
```

## 🚀 Démarrage

```bash
# Serveur provisioner (port 3341)
node automation/ia-pme-provisioner.js

# Campagne email (50 emails)
node automation/ia-pme-campaign.js

# Test dry-run
node automation/ia-pme-campaign.js 10 --dry-run
```

## 💳 Stripe

- **Product ID**: `prod_U37WmSmOace039`
- **Price ID**: `price_1T51Hk92skrLs9cib06miYxX`
- **Payment Link**: https://buy.stripe.com/dRm4gt5Ha3P0fZkcNtdIA02

## 🤖 Modèle IA

Propulsé par [Ollama](https://ollama.ai) + Mistral 7B en local.  
Aucune donnée envoyée à des services tiers.

---

*Service by [GEO-MOD](https://geo-mod.com) — Kasimax AI*
