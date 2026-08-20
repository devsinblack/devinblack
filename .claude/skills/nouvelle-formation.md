---
name: nouvelle-formation
description: Crée une nouvelle page de formation à partir du template formation-ga4.html
user_invocable: true
---

# Créer une nouvelle page de formation

Tu es un assistant qui aide à créer une nouvelle page de formation pour le site Devinblack. Tu utilises `formation-ga4.html` comme template.

## Étapes

### 1. Demander les informations

Utilise l'outil AskUserQuestion pour poser les questions suivantes **une par une** ou par groupes logiques. Ne commence pas à créer la page tant que toutes les informations ne sont pas collectées.

**Groupe 1 — Informations générales :**
- Quel est le nom de la formation ? (ex: "HubSpot CRM", "ActiveCampaign")
- Quel est le nom du fichier à créer ? (ex: "formation-hubspot.html")

**Groupe 2 — Section Hero :**
- Quel est le titre principal du hero ? (ex: "HubSpot CRM et l'automatisation de votre pipeline commercial")
- Quelle est la description du hero ? (le paragraphe sous le titre)
- Quelle URL d'image pour le hero ? (ou description pour trouver sur Unsplash)

**Groupe 3 — Section "Sujets Maîtrisés" (4 cartes) :**
Pour chaque carte (1 à 4), demander :
- Titre de la carte
- Description de la carte
- URL de l'image de la carte

**Groupe 4 — Section "Processus de formation" (6 étapes) :**
Les titres des 6 étapes sont génériques et restent les mêmes par défaut :
1. Appel de découverte des besoins
2. Définition des objectifs de la formation
3. Mise en place administrative
4. Mise en place formation présentiel/distanciel
5. Suivi administratif
6. Support pendant 3 mois

Demander : "Les titres et descriptions des 6 étapes du processus sont-ils les mêmes que pour GA4, ou souhaites-tu les personnaliser ?"

**Groupe 5 — Section "Aide supplémentaire" :**
Demander si les textes de cette section restent les mêmes ou doivent être modifiés.

### 2. Créer la page

Une fois toutes les informations collectées :

1. Lire le fichier `formation-ga4.html` comme template
2. Copier le contenu dans le nouveau fichier
3. Remplacer les éléments suivants :
   - `<title>` : remplacer "Formation Google Analytics 4" par le nom de la formation
   - Hero : titre (`<h1>`), description (`<p class="hero-desc">`), image hero
   - Section Sujets : les 4 cartes (titre `<h3>`, description `<p>`, image `<img>`)
   - Section Processus : les descriptions des 6 étapes si modifiées
   - Section Aide : les textes si modifiés
4. Conserver TOUT le reste identique (nav, footer, CSS, logos de confiance, structure)

### 3. Vérifier

- Ouvrir la page dans le navigateur pour vérifier le rendu
- Montrer le résultat à l'utilisateur

### Règles importantes

- Ne JAMAIS modifier le CSS ou la structure HTML — uniquement le contenu textuel et les images
- Conserver les logos de confiance identiques
- Conserver la nav et le footer identiques
- Le fichier de la nouvelle formation doit être créé à la racine de `C:\Users\sophi\devinblack-site\`
