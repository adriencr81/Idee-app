# Booking SaaS — Coachs-Formateurs Qualiopi

**Statut :** 🔬 À valider  
**Date :** Juin 2026  
**Score provisoire :** Non scoré — validation requise avant décision

---

## Elevator Pitch

"Le seul outil de booking pensé pour les coachs-formateurs solopreneurs : prise de RDV, paiement, et génération automatique des documents Qualiopi."

---

## Problème ciblé

Les coachs-formateurs Qualiopi solopreneurs gèrent à la main une pile de documents administratifs :
- Convention de formation
- Feuille d'émargement
- Attestation de présence
- Bilan de fin de formation
- Programme pédagogique / livret d'accueil

Aujourd'hui ils combinent Calendly + Word + Excel + outil de facturation séparés.

---

## Hypothèses à valider

- [ ] Combien de solopreneurs Qualiopi en France ? (vs. organismes collectifs) — chercher sur registre data.gouv.fr
- [ ] Est-ce que Digiforma (~€50-100/mois) répond bien ou laisse un gap ? — lire les avis Capterra/G2
- [ ] Est-ce qu'ils paient vraiment ou font avec Word/Excel ? — interviews directes
- [ ] Taille réelle du marché solopreneur Qualiopi

---

## Concurrent principal identifié

**Digiforma** — LMS + docs Qualiopi, €50-100/mois  
Gap potentiel : trop complexe pour solopreneurs, orienté organismes structurés

---

## Comment valider (48h)

1. Filtrer le registre Qualiopi sur data.gouv.fr → compter les "organisme individuel"
2. Lire les avis Digiforma sur Capterra → identifier les lacunes
3. Poster dans un groupe Facebook "coachs certifiés" ou r/entrepreneurfr : *"Comment vous gérez vos docs Qualiopi ?"*

---

## Ce qui est excluant

- Thérapeutes : **Qualiopi ne s'applique pas** (pas organisme de formation)
- Grandes structures : déjà sur Digiforma / 360Learning

---

## Si validé — ce qu'on build

- Booking + paiement (Stripe)
- Génération automatique des docs Qualiopi en PDF
- Facturation OPCO/CPF intégrée
- Simple, solopreneur-first

**Stack :** Next.js + Supabase + Stripe + PDF generation  
**Timeline estimée :** 4-5 semaines MVP

---

## Acquisition (si marché validé)

- Scraping Google Maps "coach certifié Qualiopi" + cold email
- Groupes Facebook coachs-formateurs
- Hook : *"Tu génères encore tes docs Qualiopi à la main ?"*
