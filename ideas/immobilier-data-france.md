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
