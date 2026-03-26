# Chuck Norris Facts - Recherche

Moteur de recherche temps réel sur 10 527 Chuck Norris facts issus de [chucknorrisfacts.fr](https://www.chucknorrisfacts.fr/).

## Demo

[qiwi.ch/norris](https://qiwi.ch/norris)

## Fonctionnalités

- Recherche temps réel par mot-clé avec debounce (multi-mots)
- Copie d'un fact en un clic
- Affichage de la note /10
- 100% côté client, aucun backend requis

## Stack

- HTML + CSS + JS vanilla
- JSON statique (1.3 Mo, 10 527 facts)
- Recherche via `Array.filter()` (< 5ms sur 10k entrées)

## Utilisation

Servir `index.html` et `facts.json` depuis n'importe quel serveur HTTP :

```bash
python -m http.server 8000
```

## Structure

```
├── index.html    # Interface de recherche
└── facts.json    # Base de facts (id, texte, note)
```
