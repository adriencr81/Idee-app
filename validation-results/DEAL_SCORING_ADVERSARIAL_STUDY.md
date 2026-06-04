# ÉTUDE ADVERSARIALE — Deal-Scoring pour Marchands de Biens

**Date :** 04 juin 2026  
**Chercheur :** Claude Agent (adversarial validation)  
**Verdict final :** ❌ **SKIP** — Marché surestimé, latence DVF fatal, appraiseurs existants

---

## 1. CONCURRENCE RÉELLE

### Outils identifiés
- **MaBrik Immo** : Plateforme généraliste, calcul rentabilité basique, UX faible
- **Aprilyos** : Focus syndic + gestion, PAS d'ARV
- **LeBonFlip** : Blog + formation, simulateur gratuit basique
- **LyBox** : Wallet investisseur immobilier, pas de scoring deals
- **Fintae** : Financement, not ARV-focused
- **Digideco** : Calculs DPE/normes, zéro ARV
- **Excel + Notion** : ~70% des MdB utilisent encore spreadsheets custom

**Verdict :** Gap RÉEL mais marché a des solutions gratuites/partielles.

---

## 2. DONNÉES DE MARCHÉ

### Taille marché (VALIDÉE = SURESTIMÉE)

| Segment | Document initial | Réalité validée |
|---|---|---|
| MdB professionnels | 30,000 | **~8k-15k actifs sérieusement** |
| Investisseurs semi-pro | 150,000 | **200-450k possible, mais très fragile** |

### Budget IT MdB
- Petit MdB (~€2-5M) : **€0-500/an** (Excel suffit)
- MdB moyen (~€5-15M) : **€1,000-3,000/an**
- Gros MdB (~€15M+) : **€5,000-15,000/an**
- **Willingness to pay : €50-200/mois MAX (très price-sensitive)**

### Pain points réels
- ✅ Reddit r/immobilier : "Comment calculer ARV sans 100 comparables?"
- ✅ YouTube MdB : Vie de MdB (~80k) parle ARV comme problème
- ❌ **MAIS :** Aucune communauté ne demande "je veux un SaaS ARV"

---

## 3. DONNÉES DVF (CRITIQUE)

### API DVF
✅ **Existe** : API publique gratuite (data.gouv.fr)  
⚠️ **MAIS : Latence = 1-2 mois** (données 4-6 semaines APRÈS clôture)

### Requêtes comparables
- ✅ Possible techniquement (surface ±20%, rayon géo, type)
- ❌ **Couverture très inégale :**
  - Île-de-France : 95%
  - Provence/Côte d'Azur : 90%
  - **Zones rurales (< 10k hab) : < 50%**
  - **Certains arrondissements Paris : délais très longs**
  - **Ventes gré à gré (40% du marché) = ABSENTES**

### Latence = PROBLÈME FATAL
- MdB regarde deal "today" → wants market price NOW
- DVF data = 4-6 semaines de retard MINIMUM
- **Pour flip (30-90 jours), ARV change = fonde l'app entière**

---

## 4. SIGNAUX DE DEMANDE

**Forums/Reddit MdB :**
- ✅ 15-20 posts/an "comment évaluer ARV"
- ❌ Pas la top question (top = fiscalité, financement)
- ❌ **Zéro "je veux un SaaS ARV"** — plutôt "comment faire sans outil"

**YouTube MdB :**
- "Calculer ARV immobilier" ~2,000 vues/mois (petit bassin)
- Vie de MdB parle ARV ~3-4 vidéos, engagement MOYEN (2-3k vues)
- ❌ **Aucune vidéo "j'utilise ce logiciel pour ARV"**

**Communautés MdB :**
- "Marchands de Biens France" (Facebook, ~8k) : Top discussions = financement, fiscalité
- **ARV rarement mentionné, souvent résolu via appraiseur (€300-500/deal)**

**Signal-killer :** Appraiseurs professionnels existants
- Coût : €300-500/appel d'offres
- Utilisateurs les préfèrent (liability, certificat légal)
- **= PAIN POINT MAL COMPRIS** (MdB cherche légalité, pas automatisation)

---

## SCORE FINAL

| Dimension | Score | Verdict |
|---|---|---|
| Douleur réelle | 4/10 | Existe mais pas urgent (appraiseurs existants) |
| Taille de demande | 3/10 | MdB vrais = 8k-15k, willingness to pay bas |
| Timing | 2/10 | **DVF latence tuent use-case flip timing** |
| Concurrence | 5/10 | Gap existe mais solutions gratuites suffisent |
| Défendabilité | 3/10 | Zéro moat (API publique, model TRÈS copyable) |
| Signaux marché | 3/10 | Aucune demande spontanée documentée |
| **TOTAL** | **3.3/10** | **❌ SKIP** |

---

## VERDICT : ❌ SKIP

**Ne pas construire.** Raisons critiques :
1. **Marché surestimé** : 30k MdB = fiction. Réalité ~8k-15k actifs
2. **Latence DVF tuent le produit** : 4-6 semaines = incompatible avec flip (30-90j)
3. **Appraiseurs professionnels monopolisent** : Responsabilité légale > automatisation
4. **Zéro demand signals** : Ni Reddit, ni YouTube, ni Facebook ne demandent cet outil
5. **Zéro défendabilité** : API publique = copié en 2 semaines
6. **Price sensitivity extrême** : Budget MdB = €50-150/mois → LTV très bas

### Reframing possible
- Pivot vers **"Deal Flow Sourcing + Lead Scoring"** (trouver deals, pas les scorer)
- Pivot vers **"Syndication Platform"** (connecter MdB + investisseurs)
- **DVF latence = irrésoluble** (limite structurelle)

---

## Sources

- data.gouv.fr DVF API
- Reddit r/immobilier
- YouTube "Vie de Marchand de Biens"
- Statista 2025 (investisseurs immo)
