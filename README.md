# App Playbook 🚀

Un framework complet pour créer des apps rentables en 20 jours, identifiées sur des tendances émergentes.

**Basé sur l'étude de cas de Pepai :** 50 000$ de revenus en 7 semaines après lancement.

---

## 📚 Le Flux Complet

```
1. Identifier une tendance émergente
   ↓
2. Valider la demande marché (/market-validation)
   ↓
3. Construire l'app en 20 jours (/create-app-playbook)
   ↓
4. Lancer avec marketing organique
   ↓
5. Générer des revenus
```

---

## 🔍 Phase 1 : Identifier la Tendance

**Playbook Pepai** (`playbooks/pepai-playbook.md`)

Les 5 étapes pour trouver une opportunité :

1. **Scruter les réseaux sociaux** — TikTok, Instagram (ce qui explose)
2. **Vérifier la concurrence** — Apps existent = marché validé
3. **Analyser les reviews** — Identifier les gaps
4. **Améliorer le concept** — Faire mieux que les concurrents
5. **Pré-valider** — Influenceurs + waitlist avant de coder

✅ **Succès = 50 waitlist signups + accord influenceur**

---

## ✅ Phase 2 : Valider le Marché

**Utiliser le skill `/market-validation`**

Accès au workflow structuré qui scanne :
- Reddit, forums (pain points réels)
- TikTok, Instagram (demande sociale)
- Google Trends (tendance montante)
- Competitors (features manquantes)
- Reviews (G2, Trustpilot, App Store)

**Output :** Score de marché /10

- 8-10 → **GO BUILD**
- 6-7 → Valider davantage
- <6 → Pivot ou kill

---

## 🏗️ Phase 3 : Construire en 20 Jours

**Utiliser le skill `/create-app-playbook`**

4 phases structurées :

### Phase 1 : Design "Zéro Dev" (Jours 1-5)
- Benchmark 20 competitors
- Frankenstein design en Figma
- Output : Maquettes prêtes pour coder

### Phase 2 : Data & IA Setup (Jours 6-8)
- Schéma de données JSON
- Briefing IA (Claude) avec contexte fixe
- Output : IA ne hallucine plus

### Phase 3 : Dev Flash (Jours 9-20)
- Figma-to-Code (React Native Expo)
- Core feature d'abord, onboarding après
- RevenueCat + Mixpanel
- Output : App stable déployée

### Phase 4 : Marketing Organique (Jours 21+)
- Creator UGC d'abord (pas de pubs)
- Industrialiser les vidéos qui convertissent
- Ensuite Facebook Ads
- Output : Croissance organique → payante

---

## 🎯 Comment Utiliser Ce Repo

### Pour une nouvelle idée :

1. **Dupliquer le template** (`templates/idea-template.md`)
2. **Remplir avec ton idée**
3. **Lancer la validation** (`/market-validation`)
4. **Si score ≥ 7, construire** (`/create-app-playbook`)

### Pour suivre la progression :

- `ideas/` — Idées en cours de validation
- `validated-ideas/` — Idées avec score ≥ 7
- `in-progress/` — Apps en construction (jours 1-20)
- `launched/` — Apps en production

---

## 📁 Structure du Repo

```
app-playbook/
├── README.md                          # Ce fichier
├── playbooks/
│   ├── pepai-playbook.md             # Comment identifier une tendance
│   └── app-creation-20days.md        # Framework 20 jours en détail
├── skills-guide/
│   ├── market-validation.md          # Guide du skill de validation
│   └── create-app-playbook.md        # Guide du skill de construction
├── templates/
│   ├── idea-template.md              # Template pour valider une idée
│   └── validation-report.md          # Template de rapport de marché
├── ideas/
│   └── .gitkeep
├── validated-ideas/
│   └── .gitkeep
├── in-progress/
│   └── .gitkeep
└── launched/
    └── .gitkeep
```

---

## 🚀 Quickstart

**Tu as une idée en tête ?**

1. Ouvre `/templates/idea-template.md`
2. Remplis les champs
3. Sauvegarde dans `/ideas/`
4. Lance la commande :
   ```bash
   /market-validation
   ```
5. Si score ≥ 7 :
   ```bash
   /create-app-playbook
   ```

---

## 💡 Points Clés

| Phase | Timing | Focus | Success Signal |
|-------|--------|-------|-----------------|
| **Identify** | Pre-launch | Tendance + pain | Waitlist 50+ |
| **Validate** | 15 min | Marché + concurrence | Score 7+ |
| **Design** | Days 1-5 | UX + Figma | Maquettes locked |
| **Data** | Days 6-8 | Schema + IA | IA briefée |
| **Dev** | Days 9-20 | Core feature | Stable deploy |
| **Marketing** | Days 21+ | Creator UGC | 5+ videos convert |

---

## ⚠️ Red Flags (Stop & Rethink)

- ❌ Can't get 50 waitlist signups → Market signal weak
- ❌ Market score <6 → Pivot or kill before coding
- ❌ Creator video gets <5% CTR → Product has friction
- ❌ Core feature buggy on Day 19 → Over-scoped, cut features

---

## 📖 Ressources

- **Playbook Pepai complet** → `playbooks/pepai-playbook.md`
- **Framework 20 jours détaillé** → `playbooks/app-creation-20days.md`
- **Market Validation workflow** → `skills-guide/market-validation.md`
- **App Creation workflow** → `skills-guide/create-app-playbook.md`

---

## 💬 Exemple : Peptide Tracker

**Tendance identifiée :** Peptides explosent sur TikTok (500k+ posts)

**Marché validé :** Score 7.8/10
- Real pain: "No app for peptide protocols"
- Demand size: 2M+ TikTok views
- No dominant competitor
- French market undefended

**Construction :** 20 jours
- Days 1-5: Figma design (onboarding + dashboard + logging)
- Days 6-8: JSON schema + Claude briefing
- Days 9-14: React Native app
- Days 15-18: Core feature (log doses, view results)
- Days 19-20: Deploy to TestFlight
- Days 21+: Creator videos → Facebook Ads

**Résultat :** $10k en revenues dans les 2 premières semaines via un post influenceur

---

## 🎓 Auteur

Basé sur le playbook de Cédric (Pepai founder) et optimisé pour la France/Belgique/Quebec.

---

**Prêt à créer ta première app rentable ? Commençons !** 🚀
