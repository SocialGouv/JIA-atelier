# Getting started — opérateur de la démo

Guide de la personne qui opère Claude Code pendant la démo (la « GO »). La démo tient en **2h max** et déroule de bout en bout la chaîne **retours terrain → spec → maquette → board → code (PR) → doc & changelog**, en parallélisant tout ce qui peut l'être : Claude avance (spec, tickets, socle technique) pendant que le groupe produit la maquette sur Claude Design.

## 1. Setup du poste (~10 min, avant la démo)

### Claude Desktop

- [ ] **Claude Desktop** installé et connecté.
- [ ] Repo **cloné localement**, Claude Desktop **ouvert sur le dossier du repo**.
- [ ] Modèle **Opus 4.8**, contexte **1M** activé.
- [ ] **Fast mode** activé (`/fast`).
- [ ] Effort **Extra High** (parfois noté « extra »).
- [ ] Autorisations en **mode auto** (auto-accept) — pour ne jamais être coupé par une demande de permission en live.

### GitHub & outillage

- [ ] **Forker** le repo puis cloner **ton fork** — un board GitHub Projects est lié au compte, pas au repo : chacun opère sur le sien.
- [ ] **Activer les Issues** sur le fork (désactivées par défaut) : `gh repo edit <ton-handle>/JIA-atelier --enable-issues`.
- [ ] `gh` authentifié avec le scope **`project`** : `gh auth refresh -s project`.
- [ ] Créer un **board GitHub Projects** vide, nom unique (ex. `TerriTest — <ton-handle>`).
- [ ] **pnpm** installé.
- [ ] Rien à faire pour les MCP : `dsfr` et `context7` se chargent seuls via `.mcp.json` (npx — prévoir un accès réseau).

## 2. Déroulé (2h, parallélisé)

| Quand | Claude Code (poste GO) | Le groupe, en parallèle |
|---|---|---|
| T0 | Coller le **prompt kickoff** ↓ | Présenter l'intrant terrain |
| T0 → T30 | Spec dans le README, tickets postés sur le board, socle Vite + DSFR | **Maquette sur Claude Design** à partir de la spec |
| T30 → T90 | Maquette déposée dans `maquette/` → landing alignée, **PR** ouverte | Revue du board, des tickets, du diff |
| T90 → T120 | CHANGELOG + doc | Récap : ce qui a été délégué, comment le reproduire |

Le minutage est indicatif ; la règle, elle, ne l'est pas : **rien n'attend rien**. Claude avance pendant que la maquette se fait.

## 3. Prompt kickoff

À coller tel quel au démarrage (remplacer `<board>` par le nom de ton board Projects) :

```text
Lis investigation-terrain-territest.md et déroule toute la chaîne de l'atelier (cf. CLAUDE.md), en parallélisant au maximum :

1. Spec produit concise → remplace le contenu de README.md.
2. Tickets priorisés du MVP → issues GitHub + board Projects « <board> » (via gh).
3. Sans attendre : socle Vite vanilla + pnpm + DSFR de base (markup via le MCP dsfr).
4. Implémente la landing (simulateur d'éligibilité côté client, deux portes, capture email), puis ouvre une PR via gh.
5. CHANGELOG + doc.

La maquette se fait en parallèle sur Claude Design : ne bloque pas dessus, je la déposerai dans maquette/ et tu aligneras la landing dessus. Annonce chaque étape franchie.
```

Quand la maquette Claude Design est prête : copier ses fichiers dans `maquette/` et dire à Claude « maquette déposée dans `maquette/`, aligne la landing dessus ».

## 4. Pièges connus & retex

Section vivante : après chaque répétition, noter ici ce qui optimise la démo réelle (et dans `CLAUDE.md` quand ça doit changer le comportement de Claude).

- Fork → **Issues désactivées** par défaut → les activer (`gh repo edit … --enable-issues`).
- **Projects liés au compte**, pas au repo → chacun crée son board, nom unique.
- `gh` doit avoir le scope **`project`** (`gh auth refresh -s project`).
