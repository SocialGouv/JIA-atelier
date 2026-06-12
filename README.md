# JIA-atelier — TerriTest (démo)

Atelier de développement assisté par IA. À partir du seul intrant terrain — [investigation-terrain-territest.md](investigation-terrain-territest.md) (5 entretiens) — dérouler en live avec Claude, en **2h max**, la chaîne complète :

**retours terrain → spec produit (`SPEC.md`) → maquette (Claude Design) → board (GitHub Projects) → code (PR) → doc & changelog.**

**Dispositif fictif** (« TerriTest », un séjour d'essai territorial) : support de démonstration uniquement. Le but n'est pas de livrer un produit parfait, mais que chacun **comprenne comment déléguer une partie de son métier à l'IA** et sache le reproduire — les prompts restent visibles et expliqués à chaque étape.

Pré-requis du poste opérateur → [GETTING-STARTED.md](GETTING-STARTED.md).

## Déroulé (2h, parallélisé)

| Quand | Claude Code (poste opérateur) | Le groupe, en parallèle |
|---|---|---|
| T0 | Coller le **prompt kickoff** ↓ | Présenter l'intrant terrain |
| T0 → T30 | Spec dans `SPEC.md`, tickets postés sur le board, socle Vite + DSFR | **Maquette sur Claude Design** à partir de `SPEC.md` |
| T30 → T90 | Maquette déposée dans `maquette/` → landing alignée, **PR** ouverte | Revue du board, des tickets, du diff |
| T90 → T120 | CHANGELOG + doc | Récap : ce qui a été délégué, comment le reproduire |

Le minutage est indicatif ; la règle, elle, ne l'est pas : **rien n'attend rien** — Claude avance pendant que la maquette se fait.

## Prompt kickoff

Point de départ, à co-écrire/commenter avec le groupe — **montrer le geste, c'est le cœur de l'atelier**. (Remplacer `<board>` par le nom de ton board Projects.)

```text
Lis investigation-terrain-territest.md et déroule toute la chaîne de l'atelier (cf. CLAUDE.md), en parallélisant au maximum :

1. Spec produit concise → SPEC.md.
2. Tickets priorisés du MVP → issues GitHub + board Projects « <board> » (via gh).
3. Sans attendre : socle Vite vanilla + pnpm + DSFR de base (markup via le MCP dsfr).
4. Implémente la landing (simulateur d'éligibilité côté client, deux portes, capture email), puis ouvre une PR via gh.
5. CHANGELOG + mise à jour du README.

La maquette se fait en parallèle sur Claude Design : ne bloque pas dessus, je la déposerai dans maquette/ et tu aligneras la landing dessus. Annonce chaque étape franchie.
```

Quand la maquette Claude Design est prête : copier ses fichiers dans `maquette/` et dire à Claude « maquette déposée dans `maquette/`, aligne la landing dessus ».

Les artefacts se créent dans le repo au fil de la démo : `SPEC.md`, `maquette/`, le code, `CHANGELOG.md`.
