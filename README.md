# Guide GO — atelier JIA  (⚠️ à supprimer avant de lancer l'atelier)

Mode d'emploi de la **GO** (la personne qui opère Claude Code pour le groupe).
**Supprime ce `README.md` avant de commencer** : l'étape 1 écrira la spec produit à sa place.

## L'atelier en deux mots

À partir du seul intrant `investigation-terrain-territest.md`, on déroule en live avec Claude :
**retours terrain → spec → maquette → board → tâches → code (PR) → doc.**
But : que les participants **comprennent comment déléguer une partie de leur métier à l'IA** et sachent le refaire. Le prompt reste visible et expliqué à chaque étape — c'est ça, la leçon.

## Pré-requis (poste GO)

- Claude Code connecté, lancé en **mode AUTO** (auto-accept) pour ne pas être coupé par les permissions.
- **`gh`** authentifié avec le scope **`project`** : `gh auth refresh -s project`.
- **pnpm** installé.
- Le MCP `dsfr` se charge seul via `.mcp.json` (`npx dsfr-mcp`).

## Setup avant l'atelier (≈ 5 min)

1. **Forker** ce repo sur ton compte (le repo source doit être public).
2. **Cloner** ton fork.
3. **Activer les Issues** sur ton fork — désactivées par défaut sur un fork :
   `gh repo edit <ton-compte>/JIA-atelier --enable-issues`.
4. **Créer ton board** GitHub Projects, **nom unique** (ex. `TerriTest — <ton-handle>`) — un Project est lié au compte, pas au repo, donc chacun crée le sien.
5. **Supprimer ce `README.md`**.

## Déroulé — les 6 étapes

Les prompts sont des points de départ : co-écris-les avec le groupe, montre le geste.

1. **Spec** — « Lis `investigation-terrain-territest.md` et rédige la spec produit dans `README.md` : vision, problème (verbatims), objectifs, features, KPI, périmètre client-only. Va à l'essentiel. »
2. **Maquette** — dans **Claude Design** : générer la maquette DSFR depuis la spec, puis **copier les fichiers dans `maquette/`**.
3. **Board** — « Crée dans mon board GitHub Projects les tickets des features, **ordonnés et priorisés** (le socle d'abord, la mesure en dernier). Reste simple : une page = quelques tickets, **pas d'épics**. »
4. **Tâches techniques** — « Décline en tâches concrètes : la landing + un test E2E du parcours simulateur. »
5. **Code** — « Implémente le ticket [n] en **Vite vanilla + DSFR de base** (markup via le MCP `dsfr`), d'après la maquette. Pas de re-planification. Puis ouvre une PR via `gh`. »
6. **Doc** — « Lis `gh pr diff`, rédige le CHANGELOG et mets à jour le README. »

## Règles

- **Pas de plan mode**, pas de « je fais un plan d'abord » : on va droit à l'artefact.
- Le **prompt reste visible** : les participants doivent voir le geste pour le reproduire.
- Stack : **Vite vanilla + pnpm + DSFR de base** (markup via MCP `dsfr`), **pas de react-dsfr**, landing **100 % client**.

## Pièges connus (repérés en répétition)

- Fork → **Issues désactivées** par défaut → les activer.
- **Projects liés au compte**, pas au repo → créer son board, nom unique.
- `gh` doit avoir le scope **`project`**.
