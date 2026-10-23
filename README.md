# Pokémon Game 2.0

> C'est l'un de mes tout premiers jeux ! Cette version 2.0 corrige les plantages de la [première version](https://github.com/Alex12062012/Pokemon-Game).

Un petit jeu web de collection et de combats inspiré de Pokémon : on ouvre des boosters pour former une équipe, puis on affronte 5 boss de plus en plus forts.

▶ **Jouer en ligne :** https://pokemon-game-2-0.onrender.com (hébergé gratuitement sur Render : le premier chargement peut prendre une minute)

| Menu | Booster | Combat |
|---|---|---|
| ![Menu](docs/menu.jpg) | ![Booster](docs/booster.jpg) | ![Combat](docs/combat.jpg) |

## Comment jouer

- **Boosters (50 €)** : un Pokémon au hasard. Commun 50 %, Rare 20 %, Épique 20 %, Dracaufeu 8 %, Mew 2 %.
- **Combats** : choisis un Pokémon, puis *Attaquer* (15 % de coups critiques) ou *Soigner* (+45 % des PV). Le boss peut aussi se soigner.
- **Victoire** : la récompense du boss, de 150 € à 1 000 000 € pour le dernier, Pyrodraco.
- **Défaite** : il faut soigner l'équipe (30 €) avant de recombattre. Si tu n'as plus d'argent, revends un Pokémon (40 à 800 € selon la rareté).
- Équipe de 6 Pokémon maximum. Il y a des comptes joueurs et des sauvegardes, avec une interface en français, anglais et russe.

## Lancer le jeu

```bash
pip install -r requirements.txt
python Qwen_python_20260113_8ii4z3f7i.py
```

Ouvre ensuite http://localhost:5000.

## Technique

- **Langage et serveur :** Python avec [Flask]. Tout le jeu tient dans un seul fichier, pages HTML comprises.
- **Données :** les comptes sont dans `pokemon_users.json`, avec des mots de passe hachés (SHA-256). Les parties sont dans `pokemon_saves/`.
- **Origine du code :** il a été écrit avec l'aide de l'assistant IA Qwen, d'où le nom du fichier.

[Flask]: https://flask.palletsprojects.com

---
*Projet de fan, non officiel. Pokémon est une marque de Nintendo / Creatures / Game Freak.*
