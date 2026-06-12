# Getting started — pré-requis opérateur

Checklist du poste de la personne qui opère Claude Code (la « GO »), à faire avant la démo (~10 min). Le déroulé et le prompt kickoff sont dans le [README](README.md).

Objectif : **zéro friction le jour J** — tout ce qui peut être préparé ou préchargé avant la démo doit l'être ; rien ne doit interrompre le live (permission, login, téléchargement, copier-coller à bricoler).

## Claude Desktop

- [ ] **Claude Desktop** installé et connecté.
- [ ] Repo **cloné localement**, Claude Desktop **ouvert sur le dossier du repo**.
- [ ] Modèle **Opus 4.8**, contexte **1M** activé.
- [ ] **Fast mode** activé (`/fast`).
- [ ] Effort **Extra High** (parfois noté « extra »).
- [ ] Autorisations en **mode auto** (auto-accept) — pour ne jamais être coupé par une permission en live.

## GitHub & outillage

- [ ] **Forker** le repo (le repo source doit être public) puis cloner **ton fork** — un board GitHub Projects est lié au compte, pas au repo : chacun opère sur le sien.
- [ ] Dans le clone, **pointer `gh` sur le fork** : `gh repo set-default <ton-handle>/JIA-atelier` — sinon les PR partent sur le repo source.
- [ ] **Activer les Issues** sur le fork (désactivées par défaut) : `gh repo edit <ton-handle>/JIA-atelier --enable-issues`.
- [ ] `gh` authentifié avec le scope **`project`** : `gh auth refresh -s project`.
- [ ] Créer un **board GitHub Projects** vide, nom unique, et le rendre **public** (les participants le suivent en live) :
  `gh project create --owner "@me" --title "Canicule — <ton-handle>"` puis `gh project edit <numéro> --owner "@me" --visibility PUBLIC`.
- [ ] **pnpm** installé globalement.
- [ ] MCP `dsfr` et `context7` : rien à faire, chargés via `.mcp.json` (npx — prévoir un accès réseau).

## Préchauffage (zéro friction)

- [ ] Ouvrir Claude une première fois sur le repo et vérifier `/mcp` : `dsfr` et `context7` connectés — ça précharge les paquets npx.
- [ ] Préparer le **prompt kickoff** (cf. README) avec `<board>` déjà remplacé, prêt à coller.

## Retex

Après chaque répétition : noter ici les pièges et optimisations de la démo, et dans `CLAUDE.md` ce qui doit changer le comportement de Claude.
