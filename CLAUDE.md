# JIA-atelier — point de départ

Repo de départ d'un atelier de développement assisté par IA. **Dispositif fictif** (« TerriTest », un séjour d'essai territorial) : support de démonstration uniquement.

## But de l'atelier

À partir du seul intrant — `investigation-terrain-territest.md` (5 entretiens terrain) — dérouler en live, avec Claude, la chaîne complète :

**retours terrain → spec produit (README) → maquette (Claude Design) → board (GitHub Projects) → tâches techniques → code (PR) → doc & changelog.**

Le but n'est pas de livrer un produit parfait, mais que chacun **comprenne comment déléguer une partie de son métier à l'IA**, et sache le reproduire. Les prompts et les décisions restent visibles et explicités : c'est le cœur de l'atelier.

## Comment travailler

- **Va droit au but.** Pas de plan préalable, pas de « laisse-moi d'abord faire un plan » : produis directement l'artefact demandé. Une tâche déjà spécifiée (un ticket) s'exécute sans la re-planifier.
- **Ne bloque pas sur des questions de friction.** Prends des décisions raisonnables, **documente brièvement tes hypothèses**, et ne pose que les questions qui changent vraiment l'orientation produit ou technique.
- **Sorties lisibles**, structurées, en **français**. On doit pouvoir suivre ton raisonnement.

## Stack (étape code)

Landing **client-only**, **sans React** :

- **Vite** (template vanilla) + **pnpm** comme gestionnaire de paquets.
- **DSFR de base** (Système de Design de l'État) : markup `fr-*`, CSS et JS du DSFR. **Utilise le MCP `dsfr`** pour récupérer le markup exact des composants (header, composition/hero, stepper, tuiles, formulaire, footer, alert…) au lieu de l'inventer.
- Le **JS interactif du DSFR** (menu, accordéons) s'initialise tout seul une fois chargé — on reste en vanilla, donc aucun bricolage React.

## Périmètre (slice)

Viser petit et faisable :

- **100 % côté client** : pas d'API, pas de base de données, pas de Matomo réel.
- Logique du simulateur d'éligibilité **côté client** (JS).
- Capture email = formulaire front (l'envoi réel n'est pas nécessaire pour la démo).
- **Accessibilité RGAA** et **DSFR** non négociables.

> Le reste de l'ambition produit (matching, logistique, espace territoire, mesure serveur) reste **hors périmètre** de l'atelier — à mentionner, pas à construire.
