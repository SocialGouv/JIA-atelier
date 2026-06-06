# Guide GO — atelier JIA  (⚠️ à supprimer avant de lancer l'atelier)

Mode d'emploi de la **GO** (l'animatrice qui opère Claude Code pour le groupe).
**Supprime ce `README.md` avant de commencer** : l'étape 1 de l'atelier écrira la spec produit à sa place.

## L'atelier en deux mots

À partir du seul intrant `investigation-terrain-territest.md`, on déroule en live avec Claude la chaîne :
**retours terrain → spec → maquette → board → tâches → code (PR) → doc.**
But : que les participants **comprennent comment déléguer une partie de leur métier à l'IA** et sachent le refaire. Le prompt reste visible et expliqué à chaque étape — c'est ça, la leçon.

## Pré-requis (poste GO)

- Claude Code installé et connecté, lancé en **mode AUTO** (auto-accept) pour ne pas être coupé par les demandes de permission.
- **`gh`** authentifié, avec le scope **`project`** : `gh auth refresh -s project`.
- **pnpm** installé.
- Le MCP `dsfr` se charge seul via `.mcp.json` (`npx dsfr-mcp`) — l'accepter au 1er lancement.

## Setup avant l'atelier (≈ 5 min)

1. **Forker** ce repo sur ton compte. *(Le repo source doit être public pour autoriser le fork.)*
2. **Cloner** ton fork.
3. **Activer les Issues** sur ton fork — elles sont **désactivées par défaut sur un fork** :
   `gh repo edit <ton-compte>/JIA-atelier --enable-issues` (ou Settings → Features → Issues).
4. **Créer ton board** GitHub Projects avec un **nom unique** (ex. `TerriTest — <ton-handle>`).
   ⚠️ Un Project est lié au **compte**, pas au repo → il n'est **pas** inclus dans le fork, chacun crée le sien.
5. **Supprimer ce `README.md`**, puis lancer Claude Code.

## Déroulé — les 6 étapes

Les prompts ci-dessous sont des **points de départ** : co-écris-les avec le groupe, montre le geste.

1. **Spec** — « Lis `investigation-terrain-territest.md` et rédige la spec produit dans `README.md` : vision, problème (verbatims), objectifs, features P0, KPI, périmètre client-only. Va à l'essentiel. »
2. **Maquette** — dans **Claude Design** : générer la maquette DSFR depuis la spec → **copier les fichiers dans `maquette/`** (copie manuelle).
3. **Board** — « À partir de la spec, crée dans mon board GitHub Projects les tickets des features, **avec labels, une priorité et un ordre de réalisation** (le socle d'abord, la mesure en dernier). »
4. **Tâches techniques** — « Décline en tâches concrètes : la landing + un test E2E du parcours simulateur. »
5. **Code** — « Implémente le ticket [n] en **Vite vanilla + DSFR de base** (markup via le MCP `dsfr`), d'après la maquette. Pas de re-planification. Puis ouvre une PR via `gh`. »
6. **Doc** — « Lis `gh pr diff`, rédige le CHANGELOG et mets à jour le README. »

## Règles de conduite

- **Pas de plan mode**, pas de « je fais un plan d'abord » : on va droit à l'artefact.
- Le **prompt reste visible** : les participants doivent voir et comprendre le geste pour le reproduire.
- Stack imposée : **Vite vanilla + pnpm + DSFR de base** (markup via le MCP `dsfr`), **pas de react-dsfr**, landing **100 % côté client**.

## Pièges connus (repérés en répétition)

- Fork → **Issues désactivées** par défaut → les activer (étape 3 du setup).
- **Projects liés au compte**, pas au repo → créer son board, nom unique par GO.
- `gh` doit avoir le scope **`project`**.
