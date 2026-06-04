# Immobilier Data France — Idées B2B SaaS

**Recherche effectuée :** 04 juin 2026
**Statut :** Analyse approfondie — 3 idées prioritaires identifiées
**Marché :** France B2B / données publiques immobilières
**Catégorie :** SaaS · PropTech · Open Data

---

## Contexte : Les données disponibles

La France dispose d'un écosystème de données immobilières publiques exceptionnel et sous-exploité commercialement :

| Base | Nature | Accès |
|---|---|---|
| DVF (DGFiP/Etalab) | Toutes les transactions immobilières, 5 ans glissants | Open data |
| DPE (ADEME) | 9M+ diagnostics énergétiques, +35 000/semaine | Open data |
| BDNB/RNB (CSTB) | 32M bâtiments, 400+ variables chacun | Open data partiel |
| RPLS | Parc locatif social logement par logement | Open data |
| SITADEL | Tous les permis de construire | Open data |
| LOVAC (CEREMA) | 1,35M logements vacants 2+ ans avec profil propriétaire | Restreint (public) |
| Fichiers Fonciers MAJIC | Parcelles, propriétaires, droits de propriété | Accès organismes publics |
| OLL / ANIL | Loyers de référence, 37 observatoires, 67 agglos | Open data |
| PLU / GPU | Règles d'urbanisme, zonages constructibles | Open data |
| PERVAL / BIEN | 100% des transactions notariales (pro) | Payant professionnel |

---

## IDÉE #1 — Compliance Réglementaire pour Gestionnaires Locatifs

### Elevator Pitch
**"Le tableau de bord de risque réglementaire pour administrateurs de biens : DPE, encadrement des loyers, interdictions de location — tout croisé automatiquement avec les données publiques sur leur portefeuille."**

### Problème résolu
Un ADB (administrateur de biens) gérant 200–2 000 logements jongle avec une pile de conformités changeantes. Les logiciels existants (Rentila, BailFacile, Smartloc, Septeo) gèrent la compta locative mais **ne croisent pas les données publiques DPE/OLL avec le portefeuille du client**. Résultat : erreurs, pertes de mandats, risque de responsabilité civile professionnelle.

**Pains concrets :**
- Bailleur mécontent : "Pourquoi mon logement G est encore en location depuis janvier 2025 ?"
- Loyer proposé 20% au-dessus du loyer de référence OLL en zone encadrée = litige locataire
- Renouvellement de bail sans vérifier que la commune a rejoint l'encadrement depuis 6 mois
- Audit révèle 15% du portefeuille en infraction DPE

### Pour qui
- **Priorité 1 :** Administrateurs de biens professionnels (ADB) — 18 000 agences avec activité gestion locative (FNAIM), 2 300+ accompagnés par Septeo seul
- **Priorité 2 :** Bailleurs particuliers multi-biens (3+ logements) — 150 000+ en France

### Ce que les outils existants font et ne font PAS

**Outils actuels (Rentila, BailFacile, Smartloc, Vilogi, Powimo) :**
- ✅ Baux conformes ALUR
- ✅ Quittances automatiques + indexation IRL
- ✅ Alertes expiration diagnostics (saisie manuelle)
- ✅ État des lieux mobile

**Ce qu'aucun ne fait :**
- ❌ Croisement auto avec DPE ADEME (9M records) sans saisie manuelle
- ❌ Alerte proactive "votre bien au 12 rue Voltaire est classé G — interdit à la location depuis le 01/01/2025"
- ❌ Coût estimé de mise en conformité (isolation, chauffage) via BDNB + barèmes ANAH
- ❌ Loyer de référence OLL par adresse (69 villes en encadrement en 2026, en expansion : Marseille, Rennes, Nantes...)
- ❌ Score de risque portefeuille (% biens à risque, horizon calendaire des interdictions)

### Données mobilisées
| Source | Usage |
|---|---|
| DPE ADEME (open data API) | Classement énergie automatique par adresse |
| OLL / observatoires-des-loyers.org | Loyer de référence €/m² par zone, type, époque |
| data.gouv.fr encadrement loyers | Zones et plafonds par quartier (69 villes + extensions) |
| BDNB / RNB (CSTB) | Âge bâtiment, surface, type chauffage → coût réno estimé |
| Barèmes MaPrimeRénov' ANAH | Aides disponibles selon profil et localisation |
| Registre copropriétés ANAH | État syndicat, charges |

### Calendrier réglementaire (la douleur s'accélère)
- **Depuis 01/01/2025** : Interdiction de louer les logements G
- **2028** : Interdiction pour les F
- **2034** : Interdiction pour les E
- **Depuis août 2022** : Gel des loyers pour F et G (pas d'indexation IRL)
- **2026** : 69 villes en encadrement des loyers, +Marseille, Rennes, Nantes en cours

### Score de validation
| Dimension | Score |
|---|---|
| Douleur réelle | 9/10 |
| Taille du marché | 8/10 |
| Timing réglementaire | 10/10 |
| Concurrence directe | 8/10 (gap confirmé) |
| Données disponibles | 9/10 (100% open data) |
| **Total** | **8.8/10** |

**Verdict : GO BUILD**

### Taille de marché
- Scénario conservateur : 1 000 ADB pro × 200 €/mois = **2,4 M€ ARR**
- + 10 000 bailleurs particuliers × 30 €/mois = **3,6 M€ ARR** supplémentaires
- Potentiel de rachat : Septeo, Thetrawin, assureurs PNO

### Revenue Model
- **Pro ADB :** 150–300 €/mois selon taille de portefeuille
- **Bailleurs particuliers :** 19–49 €/mois
- **Freemium :** Diagnostic portefeuille gratuit (hook), payant pour alertes + export PDF

### MVP (3 mois)
1. Moteur de matching adresse → DPE (API ADEME) → classement réglementaire
2. Upload CSV du portefeuille
3. Dashboard feux rouges / orange / vert + calendrier interdictions + loyer OLL
4. 10 clients pilotes ADB en bêta payante (500 €/mois)
5. Export PDF "rapport de conformité portefeuille"

### Canaux d'acquisition
| Phase | Canal | Approche |
|---|---|---|
| Phase 1 | LinkedIn B2B | Cibler "administrateur de biens", "directeur gestion locative" |
| Phase 1 | Cold email | Hook : "Combien de biens de votre portefeuille sont en infraction DPE depuis le 1er janvier ?" + outil de diagnostic gratuit |
| Phase 1 | FNAIM / UNIS | Partenariat / sponsoring newsletters professionnelles |
| Phase 2 | Septeo / Thetrawin | Intégration marketplace plugins (distribution via leader du marché) |
| Phase 2 | SEO | "DPE location interdit 2025", "encadrement loyer [ville]", "logiciel gestion locative DPE" |
| Phase 3 | Assureurs PNO | Distribuer comme service à valeur ajoutée (Pacifica, April, Leocare) |

---

## IDÉE #2 — Deal-Scoring pour Marchands de Biens et Investisseurs Flip

### Elevator Pitch
**"Entrez une adresse. Obtenez en 30 secondes : l'ARV réelle basée sur les comparables DVF, le coût de rénovation estimé, la fiscalité MdB optimisée, et la marge nette."**

### Problème résolu
Les marchands de biens et investisseurs flip calculent leur rentabilité manuellement ou avec des simulateurs déconnectés du marché réel. La première cause de perte sur une opération flip : **surestimer l'ARV (After Renovation Value)**. Une erreur de 10% sur un bien à 300 000 € = 30 000 € de perte.

### Pour qui
- **Marchands de biens professionnels** : 30 000 en France, 6 000+ nouvelles immatriculations en 2023
- **Investisseurs semi-pro (flip/BRRR)** : 150 000+ en France, 1-3 opérations par an
- **Lotisseurs et petits promoteurs** : opérations de division foncière ou bâtie

### Ce que les outils existants font et ne font PAS

| Outil | Ce qu'il fait | Ce qui manque |
|---|---|---|
| MaBrik Immo | Simulation rentabilité MdB | Saisie manuelle, pas de DVF connecté |
| Aprilyos | Gestion projet MdB A-Z | Pas de valorisation marché auto |
| LeBonFlip | Simulateur flip | Pas de comparables réels |
| LyBox | Investissement locatif | Orienté location, pas flip |
| Fintae / MDB Academy | Simulateurs Excel gratuits | Aucune donnée marché |

**Le gap commun** : aucun outil ne va chercher automatiquement les comparables DVF réels, l'état DPE, le coût de rénovation BDNB, le potentiel PLU, ni les aides ANAH.

### Le cœur du produit : l'ARV automatique par comparables DVF

> Pour un appartement 65 m², 3ème étage, rue Victor Hugo, Lyon 7ème, rénové (DPE C/B), DVF montre que les 12 dernières ventes comparables ont fait en moyenne 4 200 €/m² (médiane 4 050 €). ARV estimée : 265 000–273 000 €.

Puis l'outil calcule automatiquement :
- Prix d'achat cible maximum (backward from ARV)
- Coût de rénovation estimé (BDNB + grille lots de travaux)
- Fiscalité MdB (TVA sur marge, IS/IR, droits enregistrement réduits)
- Aides ANAH mobilisables (MaPrimeRénov', Copro fragile...)
- Marge nette + taux de rendement
- Délai de revente estimé (DVF : durée médiane achat→revente dans ce secteur)
- Potentiel PLU : surélévation possible ? division ? changement d'usage ?

### Données mobilisées
| Source | Usage |
|---|---|
| DVF (open data) | Comparables de vente réels par adresse, surface, DPE |
| DPE ADEME | Classement actuel + projection post-réno |
| BDNB / RNB (CSTB) | Âge, matériaux, chauffage → coût réno estimé |
| PLU / GPU | Constructibilité, surélévation, division |
| Barèmes ANAH / MaPrimeRénov' | Aides disponibles selon profil |
| Fiscalité MdB | TVA sur marge, délai 2 ans, droits réduits |

### Score de validation
| Dimension | Score |
|---|---|
| Douleur réelle | 9/10 |
| Taille du marché | 8/10 |
| Timing marché | 8/10 |
| Concurrence directe | 7/10 (outils existent mais sans data) |
| Données disponibles | 9/10 (100% open data) |
| **Total** | **8.2/10** |

**Verdict : GO BUILD**

### Taille de marché
- Scénario conservateur : 2 000 MdB × 200 €/mois = **4,8 M€ ARR**
- + 10 000 investisseurs semi-pro × 49 €/mois = **5,9 M€ ARR** supplémentaires

### Revenue Model
- **Pro MdB :** 150–400 €/mois selon volume d'opérations
- **Semi-pro / particulier :** 49–99 €/mois
- **Pay-per-report :** 9–19 € par fiche d'opération (non-abonnés)
- **Freemium :** 3 rapports gratuits, puis payant

### MVP (2-3 mois)
1. Moteur DVF : pour une adresse → top 10 comparables (type ±, surface ±20%, rayon 500m, 18 mois, filtrable par DPE post-réno)
2. Calculateur de marge : saisie prix achat + ARV auto + grille travaux + fiscalité MdB
3. Export PDF "fiche d'opération" (ce que les MdB envoient à leur banquier)
4. Bêta payante 99 €/mois, 50 clients via communautés

### Canaux d'acquisition
| Canal | Approche | Audience |
|---|---|---|
| **Communautés MdB** | Partenariat / sponsoring | Vie de Marchand de Biens, MDB Academy, ImmoFlip France |
| **Formations MdB** | Affiliation outil + formation | MDB Academy (20 000+ inscrits) |
| **SEO ciblé** | "Calculer rentabilité MdB", "ARV immobilier France", "DVF comparables rénovation" | Intention d'achat max |
| **Notaires enchères** | Partenariat direct | Acheteurs aux enchères = principal sourcing MdB |
| **Experts-comptables immo** | Référencement | Conseillent les MdB sur le fiscal → prescripteurs naturels |
| **YouTube / contenu** | Tutoriels "comment calculer un flip" avec l'outil | Investisseurs semi-pro |

---

## IDÉE #3 — Remobilisation Logements Vacants (PIVOT B2G)

### Elevator Pitch
**"SaaS de pilotage des campagnes de remobilisation des logements vacants pour collectivités — segmentation LOVAC, courriers personnalisés, tracking propriétaires, tableau de bord municipal."**

### Problème résolu
Les communes reçoivent les données LOVAC (1,35M logements vacants 2+ ans en France) mais n'ont ni les outils ni les ressources pour les exploiter correctement. L'outil beta.gouv Zéro Logement Vacant existe mais reste basique : il identifie les biens, il n'orchestre pas les campagnes.

### Contrainte légale importante
Les données LOVAC individuelles (adresse + profil propriétaire) sont **réservées aux organismes publics**. Usage commercial direct interdit. Le modèle viable est donc B2G : la collectivité est cliente et détient les données légalement. Toi tu es leur outil opérationnel.

### Pour qui
- Communes et EPCI en zone tendue (1 500+ ayant accès à LOVAC)
- Services de l'État (DDT, préfectures)
- ANAH et opérateurs conventionnés

### Ce que ZLV (beta.gouv) fait et ne fait pas
- ✅ Identification et cartographie des logements vacants
- ✅ Affichage des données propriétaire
- ❌ Segmentation avancée (par ancienneté, profil, zone, potentiel)
- ❌ Génération de courriers personnalisés à grande échelle
- ❌ Tracking des réponses et relances
- ❌ Dashboard KPI de campagne (taux de contact, taux de retour au marché)
- ❌ Intégration CRM des propriétaires contactés

### Angle complémentaire : proxy de vacance open data
Sans accès à LOVAC, un score de probabilité de vacance peut être construit sur données 100% publiques :
- DVF : bien non vendu depuis 10+ ans en zone tendue
- DPE : absence totale de DPE (jamais loué récemment)
- BDNB : indicateurs de vétusté
- Légalement vendable et utilisable commercialement

### Score de validation
| Dimension | Score |
|---|---|
| Douleur réelle | 8/10 |
| Taille marché B2G | 6/10 (cycles longs) |
| Contrainte légale | ⚠️ Pivot requis |
| Concurrence | Quasi nulle |
| Données disponibles | 7/10 (restreint + proxy) |
| **Total** | **6.5/10** |

**Verdict : CAUTIOUS — intéressant en combinaison avec #1 (Compliance), pas en standalone**

### Taille de marché
- 1 500 communes × 5 000 €/an moyen = **7,5 M€ adressable**
- Cycles de vente longs (6-9 mois), procurement public

### Revenue Model
- Abonnement annuel SaaS B2G : 3 000–15 000 €/an selon taille commune
- Prestations de déploiement / formation : 2 000–5 000 €/commune

### Canaux d'acquisition B2G
| Canal | Approche |
|---|---|
| Banque des Territoires | Partenariat / labellisation |
| AMF (Association des Maires de France) | Présence congrès, newsletter |
| ADCF (intercommunalités) | Référencement chez les EPCI |
| DGALN / CEREMA | Partenariat institutionnel |
| Réseau ADIL | Prescripteurs locaux |

---

## Synthèse et Recommandations

### Priorisation

| Critère | #1 Compliance DPE | #2 Deal-scoring MdB | #3 LOVAC B2G |
|---|---|---|---|
| Faisabilité technique | ✅ Simple | ✅ Simple | ⚠️ Légal B2G |
| Données légalement accessibles | ✅ 100% open data | ✅ 100% open data | ⚠️ Restreint |
| Douleur client prouvée | ✅ Très forte | ✅ Forte | ✅ Modérée |
| Concurrence directe | Faible | Faible-modérée | Quasi nulle |
| Ticket moyen | 150–300 €/mois | 150–400 €/mois | 5–15 k€/an |
| Délai avant revenus | 2–3 mois | 1–2 mois | 6–9 mois |
| Canal le plus rapide | LinkedIn ADB + FNAIM | Communautés MdB | Banque des Territoires |
| Score global | **8.8/10** | **8.2/10** | **6.5/10** |

### Recommandation
1. **Lancer #2 en premier** : cycle de vente le plus court, MVP le plus simple, communautés déjà structurées
2. **Lancer #1 en parallèle ou juste après** : plus grand marché, réglementation qui s'accélère, potentiel de rachat
3. **#3 en option** : combiner avec #1 (module "vacance potentielle portefeuille" basé sur proxy DVF)

### Combinaison possible
Un même produit peut couvrir #1 + #3 :
> *Outil de compliance pour gestionnaires* qui inclut un module "Logements vacants dans votre portefeuille" + scoring de vacance voisine pour les communes partenaires → une base technique, deux marchés.

---

## Prochaines étapes

- [ ] Interviews : 5 ADB professionnels (pain point #1)
- [ ] Interviews : 5 marchands de biens actifs (pain point #2)
- [ ] Prototype DVF comparables : requête sur une adresse test
- [ ] Prototype DPE matching : adresse → classement auto
- [ ] Landing page avec hook "testez votre portefeuille DPE" (mesure intérêt)
- [ ] Rejoindre communautés MdB (Vie de MdB, MDB Academy) pour observer
- [ ] Décision build : #2 ou #1 en premier ?

---

*Recherche effectuée le 04/06/2026 via deep research multi-sources (CEREMA, ADEME, FNAIM, data.gouv.fr, ANIL, communautés proptech)*

---

---

# Open Data France — 10 Idées Micro-SaaS B2B

**Recherche effectuée :** 04 juin 2026
**Statut :** Analyse approfondie avec vérification adversariale — verdicts documentés
**Marché :** France B2B / micro-entrepreneurs / artisans / secteurs de niche
**Catégorie :** Boring SaaS · Data-as-a-Service · Open Data
**Contrainte :** Rythme d'1h/jour — architecture légère, API publiques, email-first

---

## Tableau de synthèse rapide

| # | Idée | Score | Verdict |
|---|---|---|---|
| 8 | Géorisques pour courtiers assurance | **8.5/10** | **GO** ⭐ |
| 9 | Planificateur bornes recharge IRVE | **8/10** | **GO** ⭐ |
| 6 | Alertes marchés publics artisans | **7.5/10** | **GO** |
| 1 | Radar BODACC cessions fonds de commerce | **7/10** | **GO si hyper-vertical** |
| 3 | Optimiseur tournées foodtruck | **6.5/10** | **WAIT** |
| 10 | Agrégateur allergènes cantines EGalim | **6.5/10** | **WAIT** |
| 2 | Leads PMR accessibilité BTP | **6/10** | **WAIT** |
| 7 | Score d'implantation commerces | **5.5/10** | **WAIT** |
| 5 | Détecteur opportunités solaire | **4.5/10** | **SKIP** |
| 4 | Moniteur subventions associations | **2.5/10** | **SKIP** |

---

## Idée 8 — Traqueur Géorisques pour Courtiers Assurance · **8.5/10** · GO ⭐

### Le problème
Les ~25 000 courtiers indépendants en France passent 5–15 min par dossier sur georisques.gouv.fr, un site conçu pour le grand public. Les logiciels de back-office assurance (Youdge, Assurly, Souscri) gèrent la souscription mais n'intègrent pas le scoring environnemental à l'adresse. Le secteur tourne sur des outils vieillissants.

### Les données
L'API Géorisques est la mieux notée du benchmark : gratuite, Swagger UI, **1 000 req/min**, couverture nationale (inondations, argiles, cavités, ICPE, radon, avalanches…). Seul bémol : les communes sans PPR approuvé apparaissent "sans risque" alors qu'elles sont "non encore étudiées" — à signaler dans l'interface.

### La faisabilité 1h/jour
MVP résumé : adresse → API Géorisques → PDF "Score de Risque" aux couleurs du courtier. Un weekend de développement. Modèle de revenus immédiat à **€29–€79/mois** ou **€1–€3 par rapport**.

### Concurrence
Aucun SaaS moderne identifié pour les courtiers indépendants. Les vieux back-offices ne se sont pas modernisés. Distribution via PLANETE CSCA ou CSCA (syndicats de courtiers) = des milliers de clients instantanément.

---

## Idée 9 — Planificateur Bornes Recharge IRVE · **8/10** · GO ⭐

### Le problème
154 000 points de charge en France fin 2024 (+31 % en un an), objectif gouvernemental 7 millions d'ici 2030. Hôtels, supermarchés, restaurants, copropriétés se posent tous la question "est-ce rentable chez moi ?". MyTraffic EV Connect est le seul outil crédible — à **€750/mois minimum**, enterprise-only. EVpin (US) ne couvre pas la France.

### Les données
Fichier IRVE sur `transport.data.gouv.fr` — quotidien, libre, bien documenté (3,8 % d'erreurs, acceptable). Immatriculations VE par commune (Ministère Transition Écologique) disponibles annuellement.

### La faisabilité 1h/jour
Algorithme central : pour une adresse, compter les bornes IRVE dans un rayon de 1/5/10 km, croiser avec le stock VE immatriculés, calculer un ratio "bornes pour N véhicules". Stack : PostgreSQL + PostGIS + Next.js.

### L'angle de distribution
Cibler les **électriciens certifiés IRVE** (~30 000 professionnels en France) qui conseillent leurs clients sur l'installation : ils ont besoin d'un outil de ROI à présenter. Prix : **€29–€49/mois**.

---

## Idée 6 — Alertes Marchés Publics Simplifiées pour Artisans · **7.5/10** · GO

### Le problème
414 000 artisans BTP en France, tous éligibles aux marchés publics locaux. Vecteur Plus facture **€209/mois** — hors de portée d'un micro-entrepreneur. BOAMP.fr est gratuit mais en langue administrative, sans simplification, et ne couvre pas les petits marchés.

### La nuance critique des données
L'API DECP (data.economie.gouv.fr) couvre les marchés **> €40 000 HT** proprement. Les contrats entre €5 000 et €40 000 sont sur les profils d'acheteurs décentralisés — des centaines de plateformes (scraping complexe).

**MVP recommandé :** se concentrer d'abord sur les marchés > €40K via DECP, filtre géo (département) + secteur (codes CPV BTP), email hebdomadaire en langage simplifié. Prix : **€19/mois**. La différence avec BOAMP.fr gratuit = lisibilité et résumé en 3 lignes.

### Concurrence
BOAMP.fr (gratuit, basique > €40K), Vecteur Plus (€209/mois, trop cher), E-marchespublics.com (a une page artisans mais sans confirmation sub-€40K). Gap clair sur la tranche €15–€49/mois avec UX simplifiée.

---

## Idée 1 — Radar BODACC Cessions Fonds de Commerce · **7/10** · GO si hyper-vertical

### Le concurrent public à ne pas ignorer
`bodacc.fr` propose déjà un **service d'alertes email gratuit** (10 recherches sauvegardées par compte). Un outil générique ne survit pas face à ça.

### Le bon positionnement
La valeur ajoutée doit être radicalement différente : monitorer **toutes** les cessions d'un secteur géographique + NAF (ex : tous les restaurants/bars d'Île-de-France), enrichissement SIRENE automatique (SIRET, téléphone, raison sociale nouvelle société), export CSV/CRM. Cible : **courtiers en cession de fonds de commerce**, réseaux franchise, directions développement enseigne. Abonnement **€49–€99/mois par département**.

### Les données
API BODACC (OpenDataSoft v2.1) : gratuite, quotidienne, excellente qualité, bien documentée. Exclusion Alsace-Moselle à documenter. bodacc.io propose déjà une API enrichie — la valeur ajoutée doit être le packaging commercial-ready, pas la donnée brute.

---

## Idée 3 — Optimiseur Tournées Foodtruck · **6.5/10** · WAIT

### Le gap est réel
Aucun outil d'intelligence de localisation pour les food trucks en France. Les concurrents (AirKitchen, Connectill) sont des POS/caisse. Marché en croissance (+30 % 2022–2024, ~700–3 500 trucks actifs).

### Pourquoi attendre
Les données de fréquentation des marchés sont fragmentées (autorisations mairie = décentralisées, pas de base nationale). La distribution est difficile : les gérants de food truck sont hyper-price-sensitifs, sans budget logiciel structuré.

**Si tu avances :** MVP freemium — liste hebdo des événements par région (gratuit), puis route optimizer **€9/mois**. Distribution via groupes Facebook food truck et AFTR.

---

## Idée 10 — Agrégateur Allergènes / Cantines EGalim · **6.5/10** · WAIT

### Le marché en haut est saturé
Datameal (25 ans, 30 employés), Easilys (racheté par Mapal OS), Salamandre, VICI AidoMenu couvrent les grandes cantines. `ma-cantine.agriculture.gouv.fr` (gratuit, open source beta.gouv) gère la déclaration de conformité EGalim — la partie obligatoire est déjà couverte gratuitement.

### Le créneau potentiel
Petites cantines de crèches, écoles associatives, traiteurs artisanaux (< 100 repas/jour) : pas les moyens d'un Datameal, bricolent avec Excel. Outil à **€29–€49/mois** avec saisie ingrédients → allergènes auto (Open Food Facts API) + export conforme EGalim.

### Le frein technique
Open Food Facts couvre bien les produits industriels mais les ingrédients frais (viande, légumes en vrac) ont une couverture partielle — lacunes dans les calculs d'allergènes, ce qui crée un risque légal réel pour le client.

---

## Idée 2 — Leads PMR Accessibilité pour Artisans BTP · **6/10** · WAIT

### Le gap concurrentiel est le plus flagrant
**Zéro concurrent direct identifié.** Handibat (label BTP) et Handinorme (advisory ERP owners) sont adjacents. 32 % des ERP non-conformes post-septembre 2024, amendes jusqu'à €45 000.

### Le point bloquant non résolu
La description suppose que le registre national ERP sur `data.gouv.fr` **indique le statut de conformité PMR par établissement**. Cette hypothèse n'a pas pu être confirmée ou infirmée par la recherche.

**Action avant tout build :** 30 minutes sur `data.gouv.fr` à chercher "ERP accessibilité conformité PMR" pour vérifier si le champ conformité existe et est renseigné à l'échelle nationale. Si oui → **GO immédiat**, le gap concurrentiel est trop large pour ignorer.

---

## Idée 7 — Score d'Implantation Commerces · **5.5/10** · WAIT

### La concurrence existe
Smappen (**€79–€199/mois**) et Isocarto (**€99–€199/mois**) sont deux concurrents réels avec des features comparables. La différenciation "Sirene-natif à €29/mois" est possible mais le positionnement est à construire.

### Le problème Filosofi est structurellement bloquant
La promesse "revenus médians par quartier (IRIS)" repose sur Filosofi. Or : **le vintage 2022 n'existe pas** (suppression de la taxe d'habitation a détruit la source géo-localisée), et Filosofi 2 (nouveau système) publie ses premières données 2023 en 2025–2026 avec une rupture de série méthodologique. Les données utilisables datent de **2021** — soit 5 ans d'écart en 2026.

**Recommandation :** attendre Filosofi 2 (vintage 2023) pour la couche revenus. En attendant, une v0 basée uniquement sur la densité concurrentielle SIRENE est honnête commercialement mais moins différenciante.

---

## Idée 5 — Détecteur Opportunités Solaire via BD TOPO · **4.5/10** · SKIP

### La concurrence spécialisée est déjà là
Cadastre-Solaire.fr (Cythelia Energy) couvre toute la France avec un module Prospection B2B sur les mêmes données IGN. Planno.io a levé en janvier 2026 pour exactement ce use case. Inicio a levé **€1,5M** pour la variante terrain agricole.

### La donnée est plus complexe que présentée
BD TOPO donne la hauteur des bâtiments (fiable en zone urbaine) mais l'orientation précise de la toiture (azimut, pente) pour le calcul solaire requiert le **LiDAR HD de l'IGN** — plusieurs centaines de Go par région, dataset séparé. La jointure BD TOPO + LiDAR + SIRENE sur une infrastructure solo est un chantier de data engineering incompatible avec 1h/jour.

---

## Idée 4 — Moniteur Subventions pour Associations · **2.5/10** · SKIP

### Deux kill factors cumulés

**Kill 1 — Donnée clé inaccessible :** L'API Data.Subvention est **légalement réservée aux seuls agents publics** (État, collectivités, opérateurs). Un développeur privé ne peut pas y accéder. La promesse "matching RNA + Data Subventions" est techniquement impossible en tant que produit commercial.

**Kill 2 — Concurrence gouvernementale et B2B établie :** Aides-territoires (beta.gouv, gratuit), Le Compte Asso (gratuit, 18 schémas), Finance Active Optim (**20 employés**, 17 000 schémas mis à jour quotidiennement). Il est impossible d'out-data une équipe éditoriale de 20 personnes ni de compétir avec des outils gouvernementaux gratuits sur le même cas d'usage.

---

## Trois enseignements transversaux

### 1. Le modèle Pappers est la référence
Pappers (données SIRENE/INPI/BODACC) : 3 M d'utilisateurs, **€492K de bénéfice net 2024**, zéro investisseur externe, ~100 clients B2B API (AXA, Crédit Agricole, EDF). La formule : données publiques + UX radicalement meilleure que le site gouvernemental + 99 % gratuit + 1 % B2B qui finance tout. Réplicable sur n'importe quel domaine avec des datasets riches.

### 2. La fourchette de prix validée pour les artisans et micro-entrepreneurs
Le marché converge sur **€9–€50/mois** avec un sweet spot à **€15–€29/mois**. Au-delà de €50/mois, le ROI doit être justifiable explicitement. Référence : 1,59 M de micro-entrepreneurs économiquement actifs en France (49,8 % des 3,18 M inscrits déclarent un CA positif).

### 3. Les alertes gratuites gouvernementales = le concurrent n°1
Avant de construire quoi que ce soit sur une API publique, vérifier si le gouvernement propose déjà une version gratuite basique du même service (BODACC.fr → alertes gratuites, BOAMP.fr → alertes gratuites, Ma Cantine → déclaration EGalim gratuite). La valeur ajoutée commerciale doit être sur l'enrichissement, la simplification et l'intégration B2B — pas sur l'accès à la donnée brute.

---

*Recherche effectuée le 04/06/2026 via deep research multi-sources adversariale (5 agents parallèles : concurrents, qualité APIs, marché SaaS France, cas d'usage documentés)*
