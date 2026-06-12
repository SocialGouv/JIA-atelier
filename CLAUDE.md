# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

# JIA-atelier — point de départ

Repo de départ d'un atelier de développement assisté par IA.

## But de l'atelier

À partir de l'intrant terrain — `recherche_utilisateur/` (recherche utilisateur sur le site « Fortes Chaleurs & Canicules » : 17 entretiens, 347 réponses questionnaire, 6 tests, benchmark 4 pays) — dérouler en live, avec Claude, la chaîne complète :

**retours terrain → spec produit (README) → maquette (Claude Design) → board (GitHub Projects) → tâches techniques → code (PR) → doc & changelog.**

Le but n'est pas de livrer un produit parfait, mais que chacun **comprenne comment déléguer une partie de son métier à l'IA**, et sache le reproduire. Les prompts et les décisions restent visibles et explicités : c'est le cœur de l'atelier.

## Pré-requis

- Claude Code en **mode AUTO** (auto-accept).
- **`gh`** authentifié avec le scope `project` : `gh auth refresh -s project`.
- **pnpm** installé globalement.
- Le MCP `dsfr` se charge seul via `.mcp.json` (`npx dsfr-mcp`).

## Comment travailler

- **Va droit au but.** Pas de plan préalable, pas de « laisse-moi d'abord faire un plan » : produis directement l'artefact demandé. Une tâche déjà spécifiée (un ticket) s'exécute sans la re-planifier.
- **Ne bloque pas sur des questions de friction.** Prends des décisions raisonnables, **documente brièvement tes hypothèses**, et ne pose que les questions qui changent vraiment l'orientation produit ou technique.
- **Sorties lisibles**, structurées, en **français**. On doit pouvoir suivre ton raisonnement.

## Commandes (une fois le projet Vite initialisé)

```bash
pnpm install       # installer les dépendances
pnpm dev           # serveur de développement (Vite, hot-reload)
pnpm build         # build de production dans dist/
pnpm preview       # prévisualiser le build
```

## Stack (étape code)

Landing **client-only**, **sans React** :

- **Vite** (template vanilla) + **pnpm** comme gestionnaire de paquets.
- **DSFR de base** (Système de Design de l'État) : markup `fr-*`, CSS et JS du DSFR. **Utilise le MCP `dsfr`** pour récupérer le markup exact des composants (header, composition/hero, stepper, tuiles, formulaire, footer, alert…) au lieu de l'inventer.
- Le **JS interactif du DSFR** (menu, accordéons) s'initialise tout seul une fois chargé — on reste en vanilla, donc aucun bricolage React.

## Architecture cible (landing page)

Le projet n'a pas encore de code — il se construit en live. La structure Vite vanilla attendue :

```
index.html          # page unique, markup DSFR (fr-*)
src/
  main.js           # point d'entrée JS, logique simulateur d'éligibilité
  style.css         # surcharges légères si nécessaire
public/             # assets statiques
```

Le DSFR s'initialise seul dès que son JS est chargé — pas de code d'init manuel requis. Récupère toujours le markup exact des composants via le **MCP `dsfr`** ; ne jamais inventer les classes `fr-*`.

## Périmètre (slice)

Viser petit et faisable :

- **100 % côté client** : pas d'API, pas de base de données, pas de Matomo réel.
- Logique du simulateur d'éligibilité **côté client** (JS).
- Capture email = formulaire front (l'envoi réel n'est pas nécessaire pour la démo).
- **Accessibilité RGAA** et **DSFR** non négociables.

> Le reste de l'ambition produit (matching, logistique, espace territoire, mesure serveur) reste **hors périmètre** de l'atelier — à mentionner, pas à construire.
