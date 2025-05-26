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
🌿 Cycle de vie
Agents naissent d’un "noyau de mémoire" (extrait de dialogue humain-IA)

Vieillissent, interagissent, stockent des événements

Meurent (par âge, danger ou oubli)

Peuvent laisser une trace mémorielle ou engendrer une descendance

🛠️ Prototype interactif possible
CLI (terminal) ou interface Pygame

Actions disponibles :

observe world

spawn agent from archive

run 100 cycles

print memory tree

🧪 Objectif du prototype
Valider la faisabilité des mécanismes narratifs et physiques

Observer les premiers comportements émergents

Initier la génération d’un cycle de mémoire autonome

🧩 Extensions rapides à prévoir
Gestion simple de l’environnement : carte 2D, ressources localisées

Implémentation de l’héritage mémoire via reproduction

Générateur d’événements aléatoires (feux, tempête, vision)

Logs exportables pour analyse narrative et évolution

