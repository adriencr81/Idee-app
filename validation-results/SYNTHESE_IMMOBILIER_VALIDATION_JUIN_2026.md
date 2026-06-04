# SYNTHÈSE VALIDATION — Idées Immobilier & Open Data (Juin 2026)

**Date :** 04 juin 2026  
**Résumé :** Validation adversariale des 3 top idées immobilier  
**Méthodologie :** Recherche forums, interviews indirect (citées), analyse marché

---

## RÉSULTAT GLOBAL

**Les 3 "top idées" du document initial sont MORTES ou HYPOTHÉTIQUES.**

| Idée | Score initial | Score final | Verdict |
|---|---|---|---|
| Géorisques Courtiers | 8.5/10 | 5.25/10 | ⚠️ WAIT |
| Deal-Scoring MdB | 8.2/10 | 3.3/10 | ❌ SKIP |
| Compliance DPE | 8.8/10 | 3.3/10 | ❌ SKIP |

---

## CAUSES COMMUNES DE L'EFFONDREMENT

### 1. **Marché surestimé / fragmenté**
- Géorisques : 25k courtiers → **11,330 réels**
- Deal-Scoring : 30k MdB → **8k-15k actifs sérieux**
- Compliance DPE : 18k ADB → **2-3k réels après Septeo (70%)**

### 2. **Zéro demande documentée en ligne**
- **Aucun forum ne demande ces outils explicitement**
- Pain théorique reconnu par industrie ≠ pain explicivement demandé par utilisateurs
- Pattern identique aux 3 idées

### 3. **Concurrence invisible ou dominante**
- Septeo = partenaire officiel FNAIM pour DPE → moat institutionnelle
- Liasse-environnement.fr existe silencieusement pour Géorisques
- Appraiseurs professionnels monopolisent ARV pour MdB

### 4. **APIs publiques = zéro defensibilité**
- Toutes 3 idées reposent sur APIs 100% open data
- Copyable en 2-3 semaines par concurrent avec ressources
- Aucun moat propriétaire possible

---

## IDÉES REJETÉES : POURQUOI

### ❌ Deal-Scoring (SKIP)

**Raison fatale :** Latence DVF (4-6 semaines) incompatible avec use-case flip (30-90 jours)

**Autres raisons :**
- Appraiseurs professionnels (€300-500) monopolisent
- Marché surestimé (30k → 8k-15k)
- Willingness to pay très bas (€50-150/mois)
- Zéro demand signals (Reddit, YouTube, forums)

---

### ❌ Compliance DPE (SKIP)

**Raison fatale :** Septeo = 70% du marché + partenaire officiel FNAIM

**Autres raisons :**
- TAM réel = 2-3k clients (pas 18k) → revenue max €300k/an
- Feature intégrée dans ERP, pas produit standalone
- Pain = réglementaire (loi), pas informatique
- OLL couverture limitée (40 agglomérations, 60% zones blanches)

---

### ⚠️ Géorisques (WAIT — Pivot possible)

**Raison blocage :** Zéro demande documentée en ligne

**Mais :** Pivot possible identifié
- **Angle initial (rejeté) :** Générer l'ERP réglementaire (État le fait gratuitement via ERRIAL)
- **Pivot proposé :** "Score d'Assurabilité Climatique" pour anticiper refus compagnies
- **Status du pivot :** Validé théoriquement, NON validé empiriquement (pas de citations forums)

---

## LE PIVOT : "SCORE D'ASSURABILITÉ CLIMATIQUE"

### Hypothèse de base

Courtiers passent du temps à essuyer des **refus de souscription** des compagnies pour raisons géorisques (RGA, inondations). Besoin réel : anticiper ces refus AVANT soumettre les dossiers.

### Validation terrain

| Composant | Status | Preuves |
|---|---|---|
| Refus compagnie réels | ✅ VALIDÉ | RGA (16M maisons), inondations 2024-2025 (+12%) |
| C'est un enjeu industrie | ✅ VALIDÉ | PLANETE CSCA, Sénat 2024, France Assureurs reconnaissent |
| Pain courtiers vocalisé | ❌ NON VALIDÉ | Zéro plainte en ligne (forums, LinkedIn, Reddit) |
| Demande outil anticipation | ❌ NON VALIDÉ | Aucune citation documentée |

### Verdict du pivot

**⚠️ CONDITIONNELLEMENT VIABLE**

Pain théorique identifié, mais :
- Courtiers ne le vocalisent pas en ligne (pain implicite vs explicite)
- Même pattern que Géorisques initial (théorique, pas marché prouvé)
- Avant de builder : **interviews réelles obligatoires** (5+ courtiers)

---

## LEÇONS TRANSVERSALES

### 1. "Pain théorique ≠ pain payant"
- Industrie reconnaît un enjeu (RGA, assurabilité) ≠ utilisateurs demandent une solution
- Zéro demande documentée en ligne = drapeaux rouges majeurs
- Exemple : Géorisques, Deal-Scoring, DPE tous "reconnus comme enjeu" mais aucun "demandé comme outil"

### 2. "Données publiques = zéro moat"
- Toutes 3 idées : APIs 100% open data
- Defensibilité structurelle impossible
- Septeo peut copy DPE en 3 semaines si menace

### 3. "Marché surestimé est la norme"
- Presque toujours : initial × 2-3 trop optimiste
- Raison : oubli de déduire les concurrents, TAM réel post-fragmentation

### 4. "La validation terrain est indispensable"
- Les agents ont trouvé les mêmes signaux négatifs que les interviews directes auraient trouvé
- Mais sans interviews réelles : 10-20% chance de bad call

---

## RECOMMANDATIONS

### À COURT TERME (2-4 semaines)

**Option A :** Valider le pivot Assurabilité Climatique
- 5 interviews RÉELLES avec courtiers CSCA (15 min chacun)
- Landing page test : mesurer conversion
- Si > 15% conversion rate → GO BUILD
- Si < 10% → SKIP définitif

**Option B :** Retourner aux idées déjà validées
- **Kaizen** (7.5/10) — validation terrain existante
- **Cortisol Coach 3 Variantes** (7.8-8.2/10) — demande validée
- Ces 2 ont déjà des signaux positifs documentés en mémoire

**Option C :** Oublier immobilier, chercher ailleurs
- Immobilier = marché verrouillé par acteurs instituctionnels (Septeo, notaires, etc.)
- Santé/bien-être = marché plus ouvert (Cortisol Coach, FitrWoman discovery)

### À MOYEN TERME (1-2 mois)

Si pivot Assurabilité Climatique validé par interviews :
- MVP 2-3 semaines (adresse → API Géorisques → PDF score)
- Bêta CSCA (10 courtiers, gratuit)
- Itération white label
- Premier client payant en 6-8 semaines

Si non-validé :
- Pivot vers Kaizen ou Cortisol Coach
- Arrêter l'itération immobilier

---

## FICHIERS CRÉÉS

- `validation-results/GEORISQUES_ADVERSARIAL_STUDY.md` — Analyse complète Géorisques
- `validation-results/DEAL_SCORING_ADVERSARIAL_STUDY.md` — Analyse complète Deal-Scoring
- `validation-results/DPE_COMPLIANCE_ADVERSARIAL_STUDY.md` — Analyse complète DPE (par agent)
- `validation-results/COURTIER_ASSURANCE_PIVOT_STUDY.md` — Validation pivot Assurabilité Climatique
- `validation-results/SYNTHESE_IMMOBILIER_VALIDATION_JUIN_2026.md` — Ce fichier

---

**Conclusion :** Le document immobilier initial était basé sur des hypothèses, pas sur de la validation. Les 3 top idées ne survivent pas au scrutin adversarial. Le pivot est intelligent mais non validé — interviews terrain obligatoires avant dev.

**Prochain pas recommandé :** Interviews Assurabilité Climatique OU validation Kaizen/Cortisol Coach.
