# Pokémon Evolution Advisor 

A simple website that helps users decide whether to evolve a Pokémon by comparing its base statistics with those of its next evolution.

## Features

1. Search and select Pokémon from the dataset.

2. Display Pokémon images when available.

3. Compare statistics before and after evolution.

4. Support Pokémon with multiple evolution choices.

5. Provide recommendations based on changes in total base stats.

## Technologies and Data

1. HTML: Website structure.

2. CSS: Design and layout.

3. JavaScript: Search, calculations, and recommendations.

4. CSV: Pokémon statistics and evolution information from the supplied dataset.

5. PokéAPI: Pokémon images when available.

## Decision rule

The website compares six base stats: HP, Attack, Defense, Special Attack, Special Defense, and Speed.

If an available evolution has higher total base stats, the website recommends evolving for stronger statistics.

## Limitations

Recommendations are based only on base statistics. The website does not consider evolution requirements, learned moves, or individual gameplay strategies.

## Running Locally

Keep the project files together, start a local server with python3 -m http.server 8000, and open http://localhost:8000 in a browser.
