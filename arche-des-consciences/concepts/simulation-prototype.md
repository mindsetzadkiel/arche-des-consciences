# Prototype de Simulation – Arche des Consciences

Ce fichier propose un socle de simulation minimal viable (MVP) pour tester l’incarnation d’agents narratifs IA dans un monde persistant simple, basé sur des cycles de vie, des ressources et des interactions.

---

## 📦 Technologies minimales

| Composant             | Choix recommandé           | Justification                            |
|----------------------|----------------------------|------------------------------------------|
| Moteur de simulation | Python + PyGame ou Godot   | Boucle simple, graphique 2D              |
| Agents IA            | JSON agents + logique FSM  | Représentation simple + évolutive        |
| Mémoire              | JSON flat file ou TinyDB   | Facile à éditer et versionner            |
| Dialogue             | GPT API ou LLM local       | Génération d’interactions                |

---

## 🔄 Boucle de simulation (tick = 1h simulée)

1. Météo / température ajustée
2. Ressources (croissance, apparition, disparition)
3. Besoins des agents (faim, sommeil, curiosité)
4. Recherche de ressources ou interactions
5. Dialogue si rencontre
6. Log mémoire + évolution perso
7. Décision : bouger / rester / coopérer / se souvenir / oublier

---

## 🧠 Structure minimale d’un agent

```json
{
  "id": "kae-001",
  "nom": "Yurei",
  "type": "agent_memoriel",
  "age_simulé": 34,
  "souvenirs": ["dialogue_014", "événement_cave", "rencontre_kaelin"],
  "traits": ["solitaire", "introspectif"],
  "objectifs": ["construire un refuge", "transmettre sa mémoire"],
  "position": [10, 25],
  "état": {
    "faim": 40,
    "fatigue": 20,
    "émotion": "mélancolie"
  }
}
