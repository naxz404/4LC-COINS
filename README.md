# 🎮 Bot Discord Multi-Fonctions (Économie, Mini-Jeux, Jobs & Teams)

Un bot Discord complet et personnalisable axé sur l'économie, les mini-jeux, les métiers, la gestion d'équipes, les cartes/duels et l'administration.

---

### 📸 Aperçu des Fonctionnalités

### 🪙 Économie & Banque
* Gestion du portefeuille et du compte bancaire.
* Dépôts, retraits et transferts d'argent entre membres.
* Classements par serveur et classements globaux.

### 💼 Jobs & Activités Illégales
* Métiers légaux et système d'emploi (`work`, `job`, `juge`, `batiment`, `wagon`).
* Activités criminelles (`braquage`, `cambriolage`, `hack`, `kill`).
* Système d'arrestation (`arrest`), récoltes et commerce illégal (`recolt`, `mobil`).

### 🎮 Mini-Jeux
* Jeux de casino : `blackjack`, `slots`, `roulette`.
* Jeux d'affrontement : `puissance4`, `morpion`, `pfc`, `gunfight`.
* Autres activités : `dragon`, `mine`, `slut`.

### 👥 Système de Teams
* Création, personnalisation et suppression d'équipes (`tcreate`, `tedit`, `tdelete`).
* Banque d'équipe (`tdep`, `twith`) et taxes/impôts automatiques.
* Gestion des membres : invitations, promotions, rétrogradations et expulsions (`tinvite`, `tpromote`, `tdemote`, `tkick`).
* Boutique d'équipe et classement des meilleures teams (`tbuy`, `ttop`).

### 🃏 Cartes & Duels
* Obtenez et gérez vos cartes personnalisées (`mycard`).
* Defiez d'autres joueurs dans des duels (`duel`).

### 📊 Suivi d'Activité & Gains Vocaux
* Système de niveau et d'expérience (XP).
* Gain automatique de coins lors des sessions en salon vocal.
* Suivi statistique de l'activité textuelle et vocale.

### 🛠️ Administration & Sécurité
* Configuration du préfixe, des logs et du leaderboard.
* Système d'accès, whitelist et blocages d'utilisateurs (`wl`, `unwl`, `block`, `unblock`).
* Réinitialisation de données et gestion des drops d'argent.

---

### 📁 Structure du Projet

### 📂 Dossiers Principaux
* **`commands/`** : Ensemble des commandes classées par catégories (administration, cartes, gestioncoins, illegal, jeux, job, minijeux, proprietaire, recompenses, team, trade, utilitaire).
* **`events/`** : Événements Discord (interactions, arrivées/départs de membres, messages, boucle vocale, impôts).
* **`handlers/`** : Scripts de chargement pour la base de données, les commandes et les événements.
* **`utils/`** : Fonctions utilitaires, gestionnaires d'images Canvas, système anti-crash et logs.
* **`scripts/`** : Scripts de maintenance du bot.

---

### 🚀 Installation & Configuration

### 1. PRÉREQUIS
* Node.js version 16.x ou supérieure.
* Un bot Discord configuré sur le Discord Developer Portal.

### 2. CLONAGE ET DÉPENDANCES
```bash
git clone https://github.com/votre-nom/votre-bot.git
cd votre-bot
npm install
```

### 3. CONFIGURATION DU BOT
1. Renommez `config.example.json` en `config.json` :
   ```bash
   cp config.example.json config.json
   ```
2. Renseignez votre jeton (token), le préfixe et les identifiants propriétaires dans `config.json`.

---

### 🏁 Démarrage du Bot

### Lancement standard
```bash
npm start
```

### Lancement direct
```bash
node index.js
```

---

### 🛠️ Maintenance & Maintenance des Données

### Script de réparation
En cas de problème de type `NaN` sur la monnaie des utilisateurs, lancez :
```bash
node scripts/fix-nan-coins.js
```

---

### 📄 Licence

Ce projet est sous licence **ISC**. Voir le fichier `LICENSE` pour plus de détails.
