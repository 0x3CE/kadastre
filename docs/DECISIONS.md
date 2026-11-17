# Décisions

Une décision par section, au format ADR : contexte, options, décision, conséquences, et un chiffre mesuré quand il y en a un.

| N° | Décision | Phase | État |
|---|---|---|---|
| ADR-000 | Changer de projet : de px4-fleet-health à Kadastre | — | acceptée |
| ADR-001 | Sources, accès machine et historique | P0, Q1 | à écrire |

## ADR-000 · Changer de projet : de px4-fleet-health à Kadastre

*2026-11-16*

**Contexte.** Le dépôt portait une plateforme de logs de vol PX4. La finance pèse lourd en Suisse (Genève, Zurich, Vaud), et ces employeurs sont visés en plus des grandes boîtes tech.

**Décision.** Le dépôt est repris pour Kadastre, une plateforme de données de référence financières (GLEIF et ESMA FIRDS). La robotique reste pour plus tard.

**Conséquences.** Le travail PX4 de novembre est gardé dans `docs/archive-px4/`. Le paquet `px4fh` devient `kadastre`.

<!-- Gabarit pour les suivantes :

## ADR-00X · Titre

*AAAA-MM-JJ*

**Contexte.**

**Options.**
1.
2.

**Décision.**

**Conséquences.**
-->
