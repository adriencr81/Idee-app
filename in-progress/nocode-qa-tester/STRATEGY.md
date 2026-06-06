# Stratégie de lancement — nocode-qa-tester

**Approche :** Build in public → Validation GitHub → Pre-sell → Build MVP  
**Horizon :** 8 semaines avant de coder quoi que ce soit

---

## Vue d'ensemble

```
Semaine 1-2         Semaine 3-4          Semaine 5-6         Semaine 7-8
──────────          ───────────          ───────────         ───────────
Publication         Amplification        Pre-sell            Décision
GitHub              contenu              waitlist            GO / NO GO
     │                   │                   │                   │
  50 stars           100 étoiles        20 pre-sales        Builder MVP
  5 issues           200 followers      à €29               ou pivoter
```

**Règle d'or :** pas une ligne de code avant 20 pre-sales confirmées.

---

## Phase 1 — Publication GitHub (Semaine 1-2)

### Objectif
Mesurer l'intérêt passif : est-ce que des inconnus starrent le repo sans qu'on leur demande directement ?

### Actions

**Jour 1 — Publication**
- Créer le repo public `nocode-qa-tester` sur GitHub
- Publier le README (déjà prêt)
- Ajouter les topics GitHub : `make`, `n8n`, `automation`, `qa`, `testing`, `nocode`, `llm`, `webhook`

**Jour 2-3 — Premier cercle**
- Partager dans les communautés directement liées au produit :
  - Discord officiel n8n (`#show-and-tell`)
  - Slack officiel Make (`#ideas` ou `#general`)
  - Subreddit r/n8n et r/nocode
- Format du post : *"Je build un outil de QA pour workflows Make/n8n. Voilà le problème que j'essaie de résoudre [lien]. Est-ce que vous testez vos automations avant livraison, et comment ?"* — pas de vente, juste une question.

**Jour 4-7 — Contenu LinkedIn (1 post/jour pendant 4 jours)**

Post 1 — Le problème (storytelling)
> *"J'ai vu un workflow IA livré à un client planter sur une question hors-sujet basique. Le chatbot a répondu n'importe quoi. Personne n'avait testé avant livraison. Voilà ce que ça coûte..."*

Post 2 — La découverte (curiosité)
> *"J'ai cherché un outil pour tester mes automations Make/n8n avant de les livrer. LangSmith existe. Galileo existe. Aucun n'est fait pour les builders no-code. Alors je construis quelque chose."*

Post 3 — Le concept (engagement)
> Schéma du pipeline avec la question : *"Si tu pouvais envoyer ton webhook et recevoir un rapport PDF avec un score sur 10 et les erreurs détectées — est-ce que tu l'utiliserais ?"*

Post 4 — L'appel à validation (CTA direct)
> *"Je valide la demande avant de coder. Si tu build des workflows IA pour des clients, ton avis m'intéresse. 2 questions dans les commentaires."*

**Métriques à atteindre en fin de phase 1**
- [ ] 50 stars GitHub
- [ ] 5 issues ouvertes avec du contenu
- [ ] 3 conversations directes avec des builders no-code (DM ou commentaires)

---

## Phase 2 — Amplification (Semaine 3-4)

### Objectif
Sortir du premier cercle, toucher des builders qui ne te connaissent pas.

### Actions

**Indie Hackers**
- Poster un "I'm building" thread sur indiehackers.com — la communauté répond bien aux produits en validation avec des chiffres concrets.
- Format : *"Day 0: building a QA tool for Make/n8n — here's the problem, here's what I'm measuring before I write code"*
- Mettre à jour le thread chaque semaine (Day 7, Day 14) — l'algorithme IH favorise les threads qui progressent.

**Product Hunt "Upcoming"**
- Créer une page "Upcoming" sur Product Hunt pour collecter des abonnés email avant le vrai launch.
- Objectif : 100 abonnés = signal fort.

**Contenu YouTube / Loom (optionnel mais puissant)**
- Vidéo de 3 min : *"Je teste manuellement un workflow Make — voilà pourquoi c'est insuffisant"*
- Montrer concrètement un chatbot qui plante sur une question ambiguë
- CTA : lien GitHub + waitlist

**Twitter/X**
- Thread technique : *"Les 5 façons dont un workflow IA no-code plante en prod (et comment les détecter avant livraison)"*
- Cibler les hashtags `#nocode` `#makecom` `#n8n` `#buildinpublic`

**Métriques à atteindre en fin de phase 2**
- [ ] 100 stars GitHub
- [ ] 200 followers sur le profil GitHub ou une newsletter
- [ ] 50 inscrits sur la page Product Hunt Upcoming

---

## Phase 3 — Pre-sell (Semaine 5-6)

### Objectif
Transformer l'intérêt en argent. 20 paiements avant de coder = GO.

### Actions

**Ajouter une waitlist au README**
```markdown
## 👉 Join the waitlist

Early access — €19 instead of €29 for the first 50 users.
[Join the waitlist →](https://tally.so/r/xxx)
```

**Page Tally (5 min à créer)**
- Champ : email
- Champ : "Quel outil utilises-tu ? (Make / n8n / autre)"
- Champ : "À quelle fréquence livres-tu des workflows IA ?"
- Bouton Stripe pour pré-payer €19 (optionnel mais différenciant)

**Email aux inscrits Product Hunt Upcoming**
- 1 email : *"La waitlist est ouverte — founding member price €19"*

**DM direct aux personnes qui ont commenté ou liké**
- Pas de masse, juste les gens qui ont montré un signal fort
- Message court : *"Tu avais commenté sur le projet — la waitlist est ouverte avec un tarif early. Tu veux ?"*

**Métriques GO / NO GO**
| Signal | NO GO | MAYBE | GO |
|--------|-------|-------|----|
| Stars GitHub | < 30 | 30-80 | 80+ |
| Issues avec feedback | 0-2 | 3-7 | 8+ |
| Waitlist inscrits | < 10 | 10-30 | 30+ |
| Pre-sales (€19) | 0-5 | 5-15 | 20+ |

**→ 20 pre-sales = on build. En dessous : on pivote ou on abandonne.**

---

## Phase 4 — Décision (Semaine 7-8)

### Si GO

Timeline de build :
```
Semaine 9-10   : Backend — orchestrateur webhook + 10 cas de test
Semaine 11     : Prompt juge Claude API + scoring
Semaine 12     : Génération PDF + envoi email
Semaine 13     : Stripe + formulaire frontend
Semaine 14     : Tests end-to-end + livraison aux early adopters
```

Livrer aux pre-sellers en priorité, collecter leurs feedbacks, itérer.

### Si NO GO ou MAYBE

Analyser les retours :
- Le problème n'est pas assez douloureux → chercher un angle différent (ex. focus sécurité/jailbreak uniquement)
- Le prix bloque → tester un modèle freemium (1 rapport gratuit/mois)
- Le marché est trop petit → élargir à Zapier, Voiceflow, Botpress
- Les gens veulent un outil différent → pivoter sur le feedback le plus récurrent

---

## Canaux par ordre de priorité

| Canal | Effort | Signal attendu | Priorité |
|-------|--------|---------------|----------|
| Discord n8n | Faible | Très ciblé | ⭐⭐⭐⭐⭐ |
| Slack Make | Faible | Très ciblé | ⭐⭐⭐⭐⭐ |
| LinkedIn posts | Moyen | Large reach | ⭐⭐⭐⭐ |
| Indie Hackers | Moyen | Builders motivés | ⭐⭐⭐⭐ |
| Reddit r/nocode | Faible | Volume | ⭐⭐⭐ |
| Product Hunt Upcoming | Faible | Pre-launch email | ⭐⭐⭐ |
| Twitter/X | Moyen | Variable | ⭐⭐ |
| YouTube / Loom | Élevé | Fort si ça décolle | ⭐⭐ |

---

## Messages qui convertissent

**Ce qui marche :**
- Montrer le problème concret (screenshot, vidéo, anecdote client)
- Poser une question ouverte (pas "est-ce que tu veux ça ?" mais "comment tu fais ça aujourd'hui ?")
- Partager les chiffres de validation en temps réel (build in public)
- Angle cybersécurité : *"j'ai testé 20 workflows IA — 14 étaient vulnérables à une question simple"*

**Ce qui ne marche pas :**
- "J'ai lancé un outil, achetez-le"
- Parler des features avant de parler du problème
- Demander des retours sans donner de contexte

---

## Ton avantage compétitif à mettre en avant

Tu es ingénieur IVQ cybersécurité. Ça change tout pour ce produit :

- Tu comprends les vecteurs d'attaque réels (prompt injection, jailbreak, data exfiltration via LLM)
- Les 10 cas de test que tu conçois seront plus pertinents que ce qu'un builder no-code pourrait imaginer
- Tu peux ajouter un angle "sécurité" que personne d'autre ne touche : *"le seul outil de QA qui teste aussi la résistance aux attaques de ton workflow IA"*
- C'est un différenciateur fort dans ta communication

---

## KPIs hebdomadaires

| Semaine | Objectif |
|---------|----------|
| S1 | Repo publié + 3 posts communautaires |
| S2 | 50 stars + 5 issues |
| S3 | Thread IH publié + page PH Upcoming |
| S4 | 100 stars + 50 abonnés PH |
| S5 | Waitlist ouverte + premier email envoyé |
| S6 | 20 pre-sales ou décision pivot |
| S7-8 | Analyse + décision GO / NO GO |
