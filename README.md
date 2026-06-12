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

Le minutage est indicatif ; la règle, elle, ne l'est pas : **rien n'attend rien** — à une exception près, la maquette attend la spec. C'est pourquoi `SPEC.md` sort en premier, vite.

## Prompt kickoff

Point de départ, à co-écrire/commenter avec le groupe — **montrer le geste, c'est le cœur de l'atelier**. (Remplacer `<board>` par le nom de ton board Projects.)

```text
Lis recherche_utilisateur/ et déroule toute la chaîne de l'atelier (cf. CLAUDE.md), en parallélisant au maximum :

1. En priorité : spec produit concise → SPEC.md — annonce-la dès qu'elle est prête, le groupe l'attend pour démarrer la maquette sur Claude Design.
2. Puis en parallèle : tickets priorisés du MVP → issues GitHub + board Projects « <board> » (via gh), et socle Vite vanilla + pnpm + DSFR de base (markup via le MCP dsfr).
3. Implémente le premier ticket — la landing — puis ouvre une PR via gh.
4. CHANGELOG + mise à jour du README.

La maquette se fait pendant ce temps sur Claude Design : ne bloque pas dessus, je la déposerai dans maquette/ et tu aligneras la landing dessus. Annonce chaque étape franchie.
```

Quand la maquette Claude Design est prête : copier ses fichiers dans `maquette/` et dire à Claude « maquette déposée dans `maquette/`, aligne la landing dessus ».

Les artefacts se créent dans le repo au fil de la démo : `SPEC.md`, `maquette/`, le code, `CHANGELOG.md`.
