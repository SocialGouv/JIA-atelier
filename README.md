# JIA-atelier — démo

Atelier de développement assisté par IA. À partir du seul intrant terrain — [recherche_utilisateur/](recherche_utilisateur/) (recherche utilisateur sur le site « Fortes Chaleurs & Canicules » : 17 entretiens, 347 réponses questionnaire, 6 tests, benchmark 4 pays) — dérouler en live avec Claude, en **2h max**, la chaîne complète :

**retours terrain → spec produit (`SPEC.md`) → maquette (Claude Design) → board (GitHub Projects) → code (PR) → doc & changelog.**

Le but n'est pas de livrer un produit parfait, mais que chacun **comprenne comment déléguer une partie de son métier à l'IA** et sache le reproduire — les prompts restent visibles et expliqués à chaque étape.

Pré-requis du poste opérateur → [GETTING-STARTED.md](GETTING-STARTED.md).

## Déroulé (2h, parallélisé)

| Quand | Claude Code (poste opérateur) | Le groupe, en parallèle |
|---|---|---|
| T0 | Coller le **prompt kickoff** ↓ | Présenter l'intrant terrain |
| T0 → T10 | **`SPEC.md` en priorité** — c'est le point de synchro | Lire la spec dès qu'elle tombe |
| T10 → T40 | Tickets postés sur le board, socle Vite + DSFR | **Maquette sur Claude Design** à partir de `SPEC.md` |
| T40 → T90 | Maquette déposée dans `maquette/` → landing alignée, **PR** ouverte | Revue du board, des tickets, du diff |
| T90 → T120 | CHANGELOG + doc | Récap : ce qui a été délégué, comment le reproduire |

Le minutage est indicatif ; la règle, elle, ne l'est pas : **la préparation n'attend rien, la publication attend le « go »** de chaque étape. Seule dépendance dure : la maquette attend la spec — c'est pourquoi `SPEC.md` sort en premier, vite.

## Prompt kickoff

Point de départ, à co-écrire/commenter avec le groupe — **montrer le geste, c'est le cœur de l'atelier**. (Remplacer `<board>` par le nom de ton board Projects.)

```text
Lis recherche_utilisateur/ et déroule la chaîne de l'atelier (cf. CLAUDE.md) en mode démo guidée :

— Prépare en tâche de fond tout ce qui peut l'être (spec, tickets, socle, code) : la préparation ne s'arrête jamais.
— Mais marque un arrêt à chaque étape du fil rouge : présente le résultat en quelques lignes et attends mon « go » avant toute action visible (post des tickets, PR…) et avant l'étape suivante.

Fil rouge : 1. SPEC.md (priorité — le groupe l'attend pour la maquette) · 2. tickets → issues + board « <board> » · 3. socle Vite vanilla + pnpm + DSFR (MCP dsfr) · 4. landing = strictement le premier ticket → PR · 5. CHANGELOG + README.

Tiens le board à jour (In Progress / Done). La maquette se fait pendant ce temps sur Claude Design ; je la déposerai dans maquette/ et tu aligneras la landing dessus.
```

Quand la maquette Claude Design est prête : copier ses fichiers dans `maquette/` et dire à Claude « maquette déposée dans `maquette/`, aligne la landing dessus ». La maquette exportée est souvent du **React** : elle sert de **référence visuelle et structurelle** — le code, lui, reste vanilla DSFR (cf. CLAUDE.md).

Les artefacts se créent dans le repo au fil de la démo : `SPEC.md`, `maquette/`, le code, `CHANGELOG.md`.
