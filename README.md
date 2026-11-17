# Kadastre

Plateforme de données de référence financières. Chaque jour, Kadastre collecte le registre mondial des entités juridiques (LEI, publié par GLEIF) et le référentiel européen des instruments financiers (FIRDS, publié par l'ESMA), historise chaque changement, et répond à une question de banque : **à une date donnée, quels instruments ont été émis par les entités d'un même groupe, et lesquels posent un problème de qualité ?**

## État

Phase P0 (cadrage des sources), novembre 2026. MVP visé fin février 2027 : GLEIF LEI2 et RR, FIRDS catégories E (actions) et D (dette), en local.

## Sources

| Source | Contenu | Conditions de réutilisation |
|---|---|---|
| [GLEIF Golden Copy](https://www.gleif.org/en/lei-data/gleif-golden-copy/download-the-golden-copy) | LEI2 (qui est qui), RR (qui détient qui) | à vérifier et citer (P0, Q1) |
| [ESMA FIRDS](https://registers.esma.europa.eu/publication/helpApp) | Instruments admis sur les plateformes de l'UE (FULINS, DLTINS) | à vérifier et citer (P0, Q1) |

Les fichiers bruts restent dans `data/`, jamais dans le dépôt.

## Architecture

À venir (schéma Mermaid, février 2027).

## Lancer

```bash
uv sync
uv run pytest
```

## Structure

```
src/kadastre/   collecte (novembre), parseurs bronze (décembre)
tests/          pytest et petites fixtures
orchestration/  Dagster (janvier)
dbt/            staging, silver, gold (janvier)
infra/          Terraform (mars)
docs/           DECISIONS.md, sources, contrats de schéma
notebooks/      exploration
ops/launchd/    planification locale de la collecte
data/           ignoré par git
```

## Décisions

Voir [docs/DECISIONS.md](docs/DECISIONS.md).
