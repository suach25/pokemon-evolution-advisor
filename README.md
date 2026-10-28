# Pokémon Evolution Advisor — SDU Case 1

A simple website that compares the six base stats of a Pokémon with its immediate next evolution(s) using the provided `pokemon.csv` dataset. It uses HTML, CSS, and JavaScript (no build tools or API key).

## Run locally

From the project folder, run `python -m http.server 8000` and open `http://localhost:8000`. Do not open `index.html` directly with `file://` because browsers often block CSV fetches.

## Deploy with GitHub Pages

1. Create a new **public** GitHub repository called `pokemon-evolution-advisor`.
2. Upload `index.html`, `style.css`, `app.js` and `pokemon.csv` to its root (README is optional).
3. Open **Settings → Pages → Build and deployment**; choose **Deploy from a branch**, select **main** and **/(root)** and save.
4. Wait for deployment and find the published website link on **Settings → Pages**. The site address is generally `https://YOUR-USERNAME.github.io/pokemon-evolution-advisor/` (replace username with your own).
5. Open the public site and test Bulbasaur, Eevee, and Venusaur.

## Decision rule

Calculate the sum of HP, Attack, Defense, Special Attack, Special Defense and Speed for the selected Pokémon and each immediate next evolution. A positive difference leads to “Evolve for stronger base stats.” This is **not** a recommendation based on an individual Pokémon's level, moves, evolution costs or player strategy.

The ordinary evolution relationship uses `evolves_from_species_id`, and only base-form rows (`id < 10000`) are treated as next evolution targets. Sprite images are loaded from the public PokeAPI sprite repository when available. Missing images display a fallback.

## Submission checklist

- [ ] Live GitHub Pages URL
- [ ] Public GitHub repository URL
- [ ] Actual time spent on the case (track your own work and AI-assistance time)
- [ ] Actual monetary cost and AI tool plan/usage (report honestly; do not guess)
