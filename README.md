# SAT0RU - Visualiseur de Techniques Maudites (Jujutsu Kaisen)

![Demo GIF](https://github.com/user-attachments/assets/8ad2b871-02c0-4b97-95f3-34682e745be0)

## Description

SAT0RU est un visualiseur de techniques maudites basé sur l'anime populaire **Jujutsu Kaisen (呪術廻戦)**. Ce projet combine **MediaPipe** pour la détection des gestes de la main avec **Three.js** pour créer des visualisations 3D en temps réel des techniques les plus iconiques du manga.

Cette application transforme ta webcam en un véritable outil de sorcier !

## ✨ Fonctionnalités

Le système utilise 20 000 particules pour recréer le volume et l'énergie de chaque technique :

### 🖕 **Rouge (Repoussement)**

- **Description** : Version inversée de l'Azur, cette technique génère une force de repoussement absolue. Une sphère rouge tourbillonnante d'énergie négative.
- **Effet visuel** : Noyau blanc éblouissant avec des tentacules de particules rouges en rotation violente.
- **Déclencheur** : Index pointé vers le haut uniquement ✌️ (mais avec l'annulaire et l'auriculaire repliés)

### ✌️ **Vide Infini (Extension de Territoire de Gojo)**

- **Description** : L'extension de territoire de Satoru Gojo. Un espace céleste où l'infini submerge la conscience de l'adversaire.
- **Effet visuel** : Anneau lumineux blanc en rotation + sphère externe de particules bleues + noyau sombre représentant l'infini.
- **Déclencheur** : Index et majeur levés, annulaire et auriculaire repliés

### 🤏 **Violet Creux (Technique Secrète)**

- **Description** : La fusion du Rouge et de l'Azur créant une annihilation imaginaire. La technique la plus puissante de Gojo.
- **Effet visuel** : Singularité violette chaotique avec particules errantes, mélange d'attraction et de répulsion.
- **Déclencheur** : Pincement pouce-index (comme pour saisir quelque chose)

### ✝️ **Sanctuaire Innommable (Extension de Territoire de Sukuna)**

- **Description** : L'extension de territoire de Ryomen Sukuna. Un sanctuaire bouddhiste démoniaque entouré de crânes, d'où émanent les attaques "Cleave" et "Dismantle".
- **Caractéristiques uniques** :
  - **Pas de barrière** : Le territoire est "peint dans l'air" sans espace confiné
  - **Portée de 200 mètres** : Les découpages maudits frappent tout sur leur passage
  - **Sanctuaire à 4 entrées** : Chacune ornée de bouches grotesques
- **Effet visuel** : Structure en pagode rouge sang, crânes de taureaux au sol, cornes démoniaques au sommet, aura d'énergie maudite errante
- **Déclencheur** : Index et majeur **croisés** ✌️ (référence au chapitre 258 du manga) ou main plate en dernier recours

## 🎮 Comment Utiliser

### Prérequis

- Navigateur web moderne (Chrome, Edge, Firefox)
- Webcam fonctionnelle
- Bon éclairage pour une détection optimale

### Installation

1. **Cloner le dépôt**
   ```bash
   git clone https://github.com/reinesana/SAT0RU.git
   cd SAT0RU
   Lancer le projet
   ```

VS Code : Installer l'extension "Live Server", clic droit sur index.html → "Open with Live Server"

Ou simplement ouvrir index.html dans un navigateur (certaines fonctionnalités peuvent nécessiter un serveur local)

Guide des Gestes
Geste Technique Personnage Effet
🖕 Index levé Rouge Gojo Sphère rouge répulsive
✌️ Index + Majeur Vide Infini Gojo Domaine céleste infini
🤏 Pincement Violet Creux Gojo Singularité violette
✌️ Doigts croisés Sanctuaire Innommable Sukuna Temple démoniaque
🖐️ Main plate Neutre - Retour au calme
🎨 Détails Techniques
Technologies Utilisées
Three.js : Rendu 3D et système de particules

MediaPipe Hands : Détection des landmarks de la main

EffectComposer : Post-processing avec effet Bloom

Google Gemini 3 : Génération du code et assistance

Optimisations
20 000 particules pour un équilibre performance/qualité

Interpolation linéaire pour des transitions fluides

Détection multi-mains (possibilité d'utiliser les deux mains)

Mise à l'échelle automatique selon la résolution

🔧 Personnalisation
Tu peux modifier :

Le COUNT de particules (ligne ~85) pour plus ou moins de détails

Les couleurs dans chaque fonction getTechnique()

La sensibilité de détection dans hands.setOptions()

L'intensité du bloom dans bloomPass.strength

⚠️ Notes Importantes
La détection fonctionne mieux avec un fond uni et un bon éclairage

Distance recommandée : main à 30-50 cm de la caméra

Les gestes doivent être nets et distincts pour une reconnaissance optimale

Le projet est optimisé pour les écrans modernes (responsive)

🙏 Remerciements
Gege Akutami pour l'oeuvre originale Jujutsu Kaisen

Google Gemini 3 pour l'assistance au développement

MediaPipe pour la solution de tracking main

Three.js pour le moteur 3D

📄 Licence
Ce projet est à but éducatif et non-commercial. Tous les droits sur Jujutsu Kaisen appartiennent à leurs détenteurs respectifs.
