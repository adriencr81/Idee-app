# ÉTUDE ADVERSARIALE — Géorisques pour Courtiers Assurance

**Date :** 04 juin 2026  
**Chercheur :** Claude Agent (adversarial validation)  
**Verdict final :** ⚠️ **WAIT** — Condition: interviews terrain obligatoires

---

## 1. CONCURRENCE RÉELLE

### Acteurs trouvés
- **Fathom Global** (acquis Swiss Re 2023) : Flood mapping + risk scores, **pour assureurs/réassureurs uniquement**
- **Previsico** : Flood intelligence 48h, partenariats avec Liberty/Zurich/Generali, **zéro mention courtiers**
- **Descartes Underwriting** : Modèles paramétriques IA + satellite, **clients = entreprises grandes seulement**
- **Liasse-environnement.fr** : Solution silencieuse BASOL/BASIAS/ICPE/Géorisques, sauve 30 min/dossier, **zéro visibilité marketing**
- **Outils généralistes** (Custy, Lya, CourtiGo) : CRM courtiers, **zéro module géorisques intégré**

**Insight :** Pas de concurrent direct pour courtiers. Marché orphelin mais limité = faible barrière, peu d'exemples de réussite.

---

## 2. DONNÉES DE MARCHÉ

| Dimension | Trouvé | Réalité |
|---|---|---|
| Courtiers en France | ~25,000 initial | **~11,330 courtiers actifs (SURESTIMÉ)** |
| Petites structures | | **~90% TPE < 11 salariés** |
| Budget IT moyen | | **25-50k€/an (petit), 43-114k€/an (intermédiaire)** |
| Pain points | "Géorisques lent" | **Conformité DORA + IA = priorité #1, pas géorisques** |
| Syndicats | PLANETE CSCA | **Bien structuré (2,400 membres, 75% CA) = canal réel** |

**Signal critique :** Pas de evidence que courtiers "demandent" un outil géorisques. Pain point documenté ≠ pain point payant.

---

## 3. QUALITÉ API GÉORISQUES

✅ **Points forts :**
- API existe réellement : v1 (sans token) + v2 (FranceConnect/Cerbère)
- Rate limits : **1,000 requêtes/min par IP** = suffisant
- Couverture : Toutes communes INSEE + données naturelles/technologiques/minières
- Docs : Swagger accessible

⚠️ **Points faibles :**
- **Absence de SLA** = opacité complète
- Qualité données "Non communiqué" = taux d'erreurs opaque
- Couverture inégale par région
- Données manquantes zones reculées

---

## 4. SIGNAUX DE MARCHÉ (DEMAND)

**Recherches effectuées :**
- YouTube : Playlist géorisques (13 vidéos) = contenu gouvernemental, **pas communauté utilisateurs**
- Blogs/YouTubers assurance : Zéro mention "besoin urgent géorisques"
- Reddit/Forums : **Zéro discussion courtiers + géorisques** (recherche blanche)
- Producteurs de contenu : Aucun YouTubeur assurance n'a identifié ce pain point

**Signal-killer :** Demande explicite absente = pas de PMF (Product-Market Fit) validé.

---

## SCORE FINAL

| Dimension | Score | Justification |
|---|---|---|
| Concurrence directe | 6/10 | Existe ailleurs, zéro pour courtiers |
| Taille marché réel | 4/10 | 11,330 courtiers, pain point non-documenté |
| Tech faisable | 9/10 | API solide, qualité données opaque |
| **Demande réelle** | **2/10** | **ABSENT — critical blocker** |
| **TOTAL** | **5.25/10** | **⚠️ WAIT** |

---

## VERDICT : ⚠️ WAIT

**Ne pas builder maintenant.** Raisons :
1. Absence totale de demande documentée
2. Pain point non-payant (courtiers priorisent DORA/IA)
3. Compétition silencieuse (Liasse-environnement.fr existe)
4. Opacité API Géorisques (pas de SLA)

**Conditions pour GO :**
- Interviewer **5-10 courtiers CSCA** pour valider demande réelle
- Tester API Géorisques sur 100+ communes
- Créer PMV (landing page) + acquisition CSCA
- Si < 10% conversion = SKIP définitif

**Alternative :** Intégrer géorisques dans Custy/Lya/CourtiGo comme feature (partnership), pas standalone.

---

## Sources

- PLANETE CSCA (https://www.planetecsca.fr/)
- API Géorisques Documentation (https://www.georisques.gouv.fr/doc-api)
- Fathom Global Insurance
- Previsico Flood Risk
- Descartes Underwriting
