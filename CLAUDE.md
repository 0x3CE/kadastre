# Kadastre : consignes pour Claude

Plateforme de données de référence financières (GLEIF et ESMA FIRDS). Cahier des charges : https://claude.ai/artifact/P1FwoxYmDykDAgwDsoHsjb. Plan et guide : le site Cap Lausanne et le projet claude.ai « Projet Expatriation ».

## Phase en cours

P0, cadrage des sources (novembre 2026). Ensuite : P1–P2 en décembre, P2–P4 en janvier et février (MVP fin février), P5 de mars à juin, P6 en juillet et août.

## Répartition (Option B)

- Aj code toute la logique : collecte, parseurs, SCD2, modèles dbt, SQL récursif, règles de qualité, réconciliation, tests.
- Claude prépare l'outillage : scaffolding, `pyproject.toml`, configs (ruff, pytest, pre-commit, launchd, Docker), gabarits de docs, squelette Terraform.
- Quand Aj bloque : mode socratique strict, indices et questions seulement, jamais la solution sauf demande explicite. La doc officielle d'abord, Claude en dernier recours.

## Règles

- Claude ne lit ni ne modifie `.env`, les secrets, `.ssh` et `.github/workflows`.
- Claude n'installe et ne télécharge rien : il donne les commandes, Aj les exécute.
- Rien de `data/` dans git ; aucun secret ; aucun fichier brut volumineux.
- `entretiens/` est ignoré par git : il ira dans un dépôt privé.
