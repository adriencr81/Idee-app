# Framework : Créer une App en 20 Jours (4 Phases)

Processus structuré pour sortir une MVP validée rapidement, sans perdre de temps sur des détails inutiles.

---

## Phase 1 : La Recherche & Le Design "Zéro Dev" (Jours 1 à 5)

**Objectif** : Valider et concevoir l'interface sans écrire une seule ligne de code.

### Étape 1 : Benchmark des 20 applications (Jours 1-2)
- Identifie un besoin ou un marché où des apps génèrent déjà de l'argent
- Télécharge les **20 meilleures applications** de cette niche
- Fais une capture d'écran de chaque étape de leur inscription/onboarding
- Aligne toutes les captures sur un canvas **Figma**

### Étape 2 : Frankenstein Design (Jours 3-5)
- Analyse ce qui fonctionne : meilleures questions, structure payante, usage des graphiques
- Crée ton propre flux d'onboarding en **mixant le meilleur** de tes concurrents
- Adapte à ta charte graphique
- **Règle d'or** : Inclure des visuels "scientifiques" (courbes, statistiques fictives basées sur réponses) pour justifier la valeur avant de demander le paiement

---

## Phase 2 : Le Cadrage Data & Le Scripting IA (Jours 6 à 8)

**Objectif** : Donner des fondations ultra-claires à l'IA pour éviter qu'elle ne s'égare.

### Étape 3 : Spécification du Schéma de Données (Jour 6)
- Rédige un document simple (Markdown ou texte brut)
- Liste la structure complète de ta base de données
- Écris un exemple de fichier **JSON complet** incluant tous les attributs (user, subscription, saved_items, etc.)

### Étape 4 : Initialisation de l'Assistant (Jour 7)
- Ouvre un outil IA (Claude ou ChatGPT)
- Soumets-lui le document de données en guise de contexte initial
- Dis-lui : **"Voici l'architecture de données de mon application. Tu vas te baser strictement sur ce JSON pour toutes les fonctionnalités."**

---

## Phase 3 : Le Développement Flash (Jours 9 à 20)

**Objectif** : Sortir une version qui fonctionne, pas une version parfaite.

### Étape 5 : Figma-to-Code (Jours 9-14)
- Initialise un projet **Expo** (React Native pour iOS + Android d'un coup)
- Prends des captures de tes maquettes Figma
- Donne-les directement à l'IA
- Demande-lui de générer les composants/écrans à partir du visuel
- **Ne perds pas de temps** à ajuster les pixels à la main

### Étape 6 : Cœur Métier d'abord, Onboarding ensuite (Jours 15-18)
- **Ignore l'onboarding au début**
- Code d'abord la fonctionnalité principale (le service que l'utilisateur vient chercher)
- Une fois que le cœur tourne, implémente le flux d'onboarding conçu en Phase 1

### Étape 7 : Câblage des Tiers (Jours 19-20)
- Ne réinvente pas la roue pour les fonctionnalités complexes
- **RevenueCat** : gérer les paiements et abonnements sans effort
- **Mixpanel** : suivre où les utilisateurs abandonnent dans l'onboarding

---

## Phase 4 : Le Marketing d'Infiltration (Jours 21+)

**Objectif** : Valider l'application auprès du public avant de dépenser en budget publicitaire.

### Étape 8 : Test Organique via Créateur (UGC)
- **N'achète pas de publicités Facebook tout de suite**
- Trouve un **micro-créateur** de contenu dans ta niche
- Paie-le pour faire une vidéo "test" au format très **naturel/organique**

### Étape 9 : Industrialisation et Scaling
- Si la vidéo du créateur génère des téléchargements → bon signe
- Engage **5 autres créateurs** pour reproduire exactement la même structure de vidéo
- Une fois que tu as accumulé une **bibliothèque de vidéos qui convertissent**, utilise-les pour lancer tes campagnes publicitaires payantes (Facebook Ads)

---

## Principes Clés

1. **Design d'abord, code après** : Valider le concept avant d'investir du temps en développement
2. **Données claires** : Une architecture bien documentée évite les refactors catastrophiques
3. **Prioriser le cœur** : Lancer avec la fonctionnalité principale, pas l'onboarding parfait
4. **Réutiliser** : RevenueCat, Mixpanel, Expo... ne pas réinventer
5. **Marketing organique d'abord** : Valider la demande avec des créateurs avant de payer pour des pubs
