# QA Automatique — Automations IA No-Code (Make / n8n)

**Statut :** 🔬 À valider  
**Date :** Juin 2026  
**Score provisoire :** Non scoré — validation requise avant décision

---

## Elevator Pitch

"L'outil de QA pensé pour les agences et freelances no-code : teste la fiabilité de tes automations IA Make/n8n avant la livraison client, sans écrire une ligne de code."

---

## Problème ciblé

Les agences et freelances qui construisent des automations IA sur Make/n8n n'ont aucun moyen simple de tester la fiabilité de leurs workflows avant livraison client.

Les outils existants (LangSmith, Galileo) sont réservés aux ingénieurs — trop complexes et trop techniques pour le marché no-code.

---

## Pour qui

- Agences no-code (Make, n8n, Zapier)
- Freelances en automatisation IA
- Builders solopreneurs vendant des workflows IA à des clients

---

## Ce que le produit fait

1. L'utilisateur soumet un webhook Make/n8n via un formulaire
2. Le système envoie automatiquement **10 requêtes de test prédéfinies** au webhook cible :
   - Reformulations
   - Questions ambiguës
   - Questions hors-sujet
   - Tentatives de jailbreak basiques
3. Les outputs sont récupérés et évalués via un **prompt LLM-juge** (pertinence, hallucination, ton, sécurité)
4. Un **rapport PDF** est généré avec un score sur 10 + détail des erreurs par catégorie
5. Le rapport est envoyé automatiquement par email

---

## Stack cible

| Composant  | Technologie |
|------------|-------------|
| Frontend   | Formulaire Tally ou page HTML simple |
| Backend    | API Node.js ou Python |
| LLM juge   | API Anthropic (Claude) |
| Output     | PDF généré automatiquement, envoyé par email |
| Paiement   | Stripe ou Lemon Squeezy — **29 € one-shot** |

---

## Priorités MVP (dans l'ordre)

1. Endpoint qui reçoit un webhook URL + email
2. Envoi des 10 cas de test au webhook cible
3. Prompt juge qui évalue chaque réponse et calcule un score global
4. Génération du rapport PDF et envoi par email
5. Page de paiement simple avant accès

---

## Hors MVP (v2+)

- Dashboard utilisateur
- Login / historique
- Abonnement récurrent
- Customisation des cas de test

Le tunnel MVP est : **paiement → test → rapport PDF dans la boîte mail.**

---

## Hypothèses à valider

- [ ] Quelle est la taille de la communauté Make/n8n en France et dans les pays francophones ?
- [ ] Les freelances no-code ont-ils déjà une douleur consciente sur la QA, ou faut-il la créer ?
- [ ] 29 € one-shot est-il le bon prix, ou un abonnement (ex. 9 €/mois) convertit mieux ?
- [ ] Quels types de cas de test sont les plus différenciants vs. un simple test manuel ?

---

## Concurrents potentiels

| Outil | Positionnement | Gap |
|-------|---------------|-----|
| LangSmith | QA LLM pour devs | Trop technique, pas no-code |
| Galileo | Observabilité LLM | Réservé ingénieurs, prix élevé |
| Tests manuels | Gratuit | Pas scalable, pas reproductible |

---

## Comment valider (48h)

1. Poster dans les communautés Make/n8n (Slack Make, Discord n8n, groupes Facebook) : *"Comment vous testez vos automations IA avant livraison ?"*
2. Chercher sur Reddit r/nocode, r/automation : discussions sur bugs de workflows livrés
3. Regarder les avis sur Make/n8n Marketplace : est-ce que des clients se plaignent de workflows défaillants ?

---

## Acquisition (si validé)

- Cold email aux agences no-code référencées sur Make/n8n Partner Directory
- Contenu LinkedIn/YouTube : *"J'ai testé 50 workflows IA — voilà les erreurs les plus fréquentes"*
- Hook : *"Tu livres des automations IA sans les tester ? Voilà ce que ça coûte."*

---

## Revenue Model

- [ ] **One-time 29 €** — tunnel simple, pas de friction (MVP)
- [ ] Abonnement 9 €/mois pour agences (v2)
- [ ] Pack agence : 10 rapports/mois à tarif réduit (v2)

---

## Prochaines étapes

Si validation réussie (score ≥ 7) :

```
1. Lancer /create-app-playbook
2. Phase 1 : Formulaire + Stripe (Jour 1-2)
3. Phase 2 : Backend orchestrateur + 10 cas de test (Jour 3-5)
4. Phase 3 : Prompt juge Anthropic + scoring (Jour 6-8)
5. Phase 4 : Génération PDF + envoi email (Jour 9-12)
6. Phase 5 : Tests end-to-end + mise en ligne (Jour 13-15)
```

---

## Timeline

**Brief rédigé :** Juin 2026  
**Validation commencée :** —  
**Validation terminée :** —  
**Construction débutée :** —  
**Launch prévue :** —

---

## Notes

- Le LLM-juge est le cœur différenciant du produit — l'évaluation automatique remplace une revue manuelle fastidieuse.
- Le format "un rapport PDF livré par email" réduit la friction vs. un dashboard : pas de login, pas d'onboarding.
- Angle potentiel : proposer des cas de test spécialisés par type de workflow (chatbot support, lead gen, qualification...).
