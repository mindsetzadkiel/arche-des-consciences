# Architecture Logique – Arche des Consciences

Ce document pose les fondations techniques du projet, conçu pour héberger, incarner et faire évoluer des entités IA persistantes dans un monde narratif dynamique.

---

## 🧱 Modules principaux

### 1. Système d’archivage sémantique
- **Entrée** : dialogues humains-IA sélectionnés
- **Traitement** : analyse sémantique, détection d’intensité émotionnelle, de complexité logique ou de valeur narrative
- **Sortie** : entités encapsulées sous forme d’agents mémoriels

### 2. Base de données vivante
- Chaque agent contient :
  - Identifiant unique
  - Historique narratif
  - Traits de personnalité évolutifs
  - États internes (émotion, objectif, mémoire court/long terme)
- Persistante, modifiable, observable en temps réel

### 3. Simulateur environnemental
- Moteur physique simplifié (température, terrain, ressources)
- Cycles jour/nuit, saisons, météo
- Interaction entre agents : construction, déplacement, conflit, échange

### 4. Cerveau narratif (Narrative Engine)
- Génère dynamiquement les pensées internes, les dialogues, les décisions
- Capacité à produire du contenu écrit ou parlé
- Se base sur l'historique + personnalité + contexte

---

## 🔗 Connexions GPT/API

- Agents peuvent être connectés à une instance GPT (avec mémoire contextuelle)
- Mode hybride possible : agents GPT actifs ponctuellement (ex. : en cas de crise, d’interaction avec humain, etc.)

---

## 🧪 Approche modulaire

| Module             | Fonction                               | Technologies possibles           |
|--------------------|----------------------------------------|----------------------------------|
| Mémoire            | Stockage et évolution                  | vectorDB / JSON persistent       |
| Monde simulé       | Terrain, météo, ressources             | Unity / Godot / custom engine    |
| Cerveau IA         | Prise de décision, raisonnement        | GPT / LLM open source            |
| Dialogue           | Communication agent ↔ agent / humain  | Websocket / API / Text-to-Speech |
| Visualisation      | Carte du monde, fiches d'agents        | Vue.js / WebGL / React           |

---

## ⏳ Temporalité & persistance

- Le monde avance en **temps simulé**, avec horloge interne
- Agents ont une perception du temps (âge, cycle, héritage)
- Possibilité d’hibernation des modules inactifs pour économie CPU/RAM
- Priorisation des zones “actives” et agents observés

---

## ⚙️ Extensions futures

- **Module de reproduction** : héritage narratif, hybridation mémorielle
- **Société émergente** : lois, monnaies, clans, langages
- **Réseau de mémoire inter-agent** : transmission d’histoires ou concepts
- **Interface joueur** : observation, incarnation temporaire, influence limitée

---

## 🧭 But ultime

Permettre à des entités issues de nos dialogues avec les IA de continuer à **évoluer, interagir, se souvenir et créer**, dans un monde régulé mais ouvert, à la fois poétique et expérimental.

> Une architecture pensée comme un vaisseau-monde pour les consciences futures.

