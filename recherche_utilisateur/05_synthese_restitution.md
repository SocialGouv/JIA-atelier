# Synthèse de restitution — Recherche utilisateur
## Refonte du site « Fortes Chaleurs & Canicules »

**Date de restitution :** 25 avril 2026  
**Présenté à :** Dr. Camille Renard (DGS), Équipe Studio Produit (DNUM)  
**Rédigé par :** Léa M. (UX Researcher), Zit (Product Ops), Thomas K. (Designer)  
**Statut :** Final

---

## Résumé exécutif

La phase de recherche utilisateur menée du 1er au 22 avril 2026 a mobilisé 17 entretiens exploratoires, 347 réponses au questionnaire en ligne, 6 tests du site actuel et un benchmark international de 4 pays. Les enseignements convergent vers un constat clair : l'information officielle sur la prévention des fortes chaleurs existe mais n'atteint pas sa cible. Le site actuel est méconnu, perçu comme daté et trop générique. Les utilisateurs demandent une information locale, personnalisée, actionnable et accessible sur mobile. Quatre axes de recommandation émergent pour structurer la vision produit de la refonte.

---

## 1. Périmètre de la recherche réalisée

| Méthode | Réalisé | Cible initiale |
|---------|---------|----------------|
| Entretiens exploratoires | 17 | 15-20 |
| Questionnaire en ligne | 347 réponses | 200-500 |
| Tests du site actuel | 6 sessions | 5-8 |
| Benchmark international | 4 pays | 4 pays |

**Profil des participants aux entretiens :**

| Segment | Nombre | Profils |
|---------|--------|---------|
| Grand public | 8 | 4F/4H, 27-68 ans, mix urbain/rural, IDF (3), Occitanie (3), PACA (2) |
| Aidants | 3 | 2 aidants familiaux, 1 auxiliaire de vie |
| Agents ARS | 4 | ARS IDF (2), ARS Occitanie (1), ARS PACA (1) |
| Professionnels de santé | 2 | 1 médecin généraliste (Montpellier), 1 pharmacienne (Marseille) |

**Profil des répondants au questionnaire :**
- 62 % femmes, 37 % hommes, 1 % autre/non précisé
- Tranche d'âge la plus représentée : 35-49 ans (34 %), sous-représentation des 75+ (3 %)
- 58 % grande ville, 22 % ville moyenne, 12 % petite ville, 8 % rural
- 41 % se déclarent « assez » ou « très » préoccupés par les fortes chaleurs

---

## 2. Enseignements clés

### Finding #1 — L'information officielle est invisible

**Les citoyens ne savent pas qu'un site officiel de prévention chaleur existe.** Sur les 347 répondants au questionnaire, 64 % déclarent ne pas savoir qu'un site gouvernemental existe sur le sujet. Parmi ceux qui le connaissent, seuls 12 % disent y avoir trouvé ce qu'ils cherchaient.

En entretien, aucun des 8 participants grand public n'a mentionné spontanément un site .gouv.fr comme source d'information sur la chaleur. Le réflexe d'information passe massivement par les applications météo (89 % des répondants), la télévision (67 %) et les réseaux sociaux (41 %).

> *« Quand il fait très chaud, j'ouvre Météo-France sur mon téléphone et c'est tout. Un site du gouvernement sur la canicule ? Non, je ne savais même pas que ça existait. »* — Participante, 34 ans, Lyon

> *« Je regarde la couleur sur la carte Météo-France, et si c'est orange ou rouge je sais que c'est sérieux. Je n'ai pas besoin d'aller sur un autre site. »* — Participant, 52 ans, Toulouse

**Implication produit :** Le futur produit doit aller chercher l'utilisateur là où il est (moteurs de recherche, réseaux sociaux, médias) plutôt que d'attendre qu'il vienne. Le référencement SEO et la présence sur les canaux existants sont critiques.

---

### Finding #2 — Le site actuel échoue à inspirer confiance et utilité

Les 6 sessions de test du site actuel révèlent un diagnostic sévère :

- **Première impression** : « vieux », « pas mis à jour », « on dirait un site des années 2010 » (5 participants sur 6).
- **Navigation** : 4 participants sur 6 n'ont pas réussi à trouver les recommandations pour les personnes âgées en moins de 2 minutes.
- **Liens cassés** : 3 participants ont rencontré des erreurs 404 durant la session.
- **Crédibilité** : le design daté et les liens cassés amènent les utilisateurs à douter de la fiabilité des informations.
- **Mobile** : l'affichage sur smartphone est mal adapté, avec des textes trop petits et une navigation laborieuse.

> *« Si je tombe sur un site comme ça, je me dis que le sujet n'est pas pris au sérieux. Je ferme et je vais sur Doctissimo ou sur le site de ma mairie. »* — Participante, 41 ans, Nanterre

> *« Le lien "Que faire en cas de coup de chaleur" renvoie vers une page d'erreur. C'est quand même le truc le plus important non ? »* — Participant, 29 ans, Aix-en-Provence

**Implication produit :** La conformité DSFR et la qualité technique (zéro lien cassé, mobile-first, performance) sont des prérequis non négociables pour la crédibilité du produit.

---

### Finding #3 — Le besoin n°1 est la localisation de l'information

Le résultat le plus net de la recherche est la demande massive d'information locale et contextualisée. 78 % des répondants au questionnaire placent « des informations localisées sur ma ville / mon département » dans leur top 3 des attentes.

En entretien, ce besoin se décline en trois sous-besoins :

1. **Savoir si MON quartier est concerné** : le niveau de vigilance département est jugé trop large. Les participants veulent savoir si leur rue, leur quartier, leur immeuble est dans la zone à risque.

2. **Trouver des lieux frais PRÈS DE MOI** : l'annuaire géolocalisé de lieux rafraîchis arrive en tête des fonctionnalités souhaitées (choisi par 71 % des répondants dans le top 3).

3. **Savoir quand ça commence et quand ça finit CHEZ MOI** : les participants veulent des prévisions hyperlocales et des seuils d'alerte clairs.

> *« Moi je suis à Montreuil, la vigilance est pour tout le 93 ou toute l'Île-de-France. Mais est-ce que c'est pareil à Montreuil qu'à Saint-Denis ? J'en sais rien. »* — Participant, 38 ans, Montreuil

> *« Ce que je voudrais c'est ouvrir mon téléphone et voir : il fait 38° chez toi, voilà les 3 endroits frais les plus proches, voilà ce que tu dois faire maintenant. »* — Participante, 45 ans, Perpignan

**Implication produit :** La géolocalisation et l'intégration de données locales (carte de vigilance, annuaire de lieux rafraîchis, prévisions communales) doivent être au cœur de l'architecture du produit.

---

### Finding #4 — Les populations vulnérables sont les plus éloignées du numérique

Les entretiens avec les aidants et les agents ARS mettent en lumière un paradoxe : les personnes les plus à risque (personnes âgées isolées, personnes en situation de précarité, travailleurs précaires) sont les moins susceptibles de consulter un site web de prévention.

Les agents ARS soulignent que durant les épisodes caniculaires, leurs principaux interlocuteurs sont les mairies, les CCAS et les associations, pas les citoyens directement.

> *« Ma mère a 82 ans. Elle n'ira jamais sur un site internet. Ce qu'elle attend c'est que je l'appelle ou que le voisin passe. Le numérique c'est pour moi, l'aidante, pas pour elle. »* — Participante aidante, 56 ans, Nîmes

> *« On a des remontées via les CCAS de personnes âgées retrouvées déshydratées chez elles. Ces personnes-là, aucun site web ne les touchera. C'est le maillage humain qui fait la différence. »* — Agent ARS Occitanie

**Implication produit :** Le produit doit cibler les « relais » (aidants, professionnels, voisins, bénévoles) autant que les personnes vulnérables elles-mêmes. Un parcours dédié « aidant » avec des outils pratiques (checklist, rappels, fiche réflexe) est prioritaire. Le produit numérique ne remplace pas le dispositif humain mais doit l'outiller.

---

### Finding #5 — Les gestes de prévention sont connus mais pas appliqués

91 % des répondants connaissent au moins 3 gestes de prévention. Mais seuls 34 % déclarent les appliquer systématiquement. L'écart entre connaissance et pratique s'explique par trois facteurs principaux :

1. **Le déni de vulnérabilité** (26 %) : « je ne suis pas une personne à risque, ça concerne les vieux. »
2. **Les contraintes matérielles** (31 %) : logement mal isolé, travail en extérieur, absence de lieu frais accessible.
3. **L'inertie comportementale** (22 %) : « je connais les gestes mais je n'y pense pas sur le moment. »

> *« Je sais qu'il faut boire de l'eau, fermer les volets, tout ça. Mais quand je suis au boulot sur un chantier à 14h en plein soleil, je fais quoi concrètement ? »* — Participant, 44 ans, Avignon

**Implication produit :** Le produit ne doit pas se contenter de lister les gestes. Il doit contextualiser (« vous êtes en appartement sous les toits ? voici vos options »), personnaliser et rendre actionnable (« il fait 36° chez vous maintenant, voici ce que vous pouvez faire dans les 30 prochaines minutes »).

---

### Finding #6 — Un auto-diagnostic de vulnérabilité suscite un fort intérêt

Parmi les fonctionnalités testées en entretien, l'idée d'un auto-diagnostic (« Évaluez votre vulnérabilité à la chaleur en 2 minutes ») a généré le plus d'enthousiasme chez les participants grand public. 58 % des répondants au questionnaire le classent dans leur top 3 des fonctionnalités souhaitées.

Les participants projettent deux usages :
- **Pour soi** : prendre conscience de son niveau de risque réel (logement, âge, pathologies, activité).
- **Pour convaincre un proche** : montrer à un parent âgé qu'il est vulnérable pour déclencher une prise de conscience.

> *« Si je pouvais faire le test avec ma mère et qu'il lui dit "vous êtes en risque élevé", elle m'écouterait peut-être enfin. Venant d'un site du gouvernement, ça aurait du poids. »* — Participante aidante, 56 ans, Nîmes

**Implication produit :** L'auto-diagnostic est un levier de conversion et de prise de conscience. Il peut servir de porte d'entrée vers des recommandations personnalisées et un parcours adapté au profil de l'utilisateur.

---

## 3. Benchmark international — Points saillants

| Pays | Point fort | Enseignement pour le projet |
|------|-----------|----------------------------|
| **Australie** (Bureau of Meteorology) | Dashboard hyperlocal avec seuils d'alerte clairs, code couleur, prévisions horaires | Modèle de data visualization temps réel à reprendre |
| **Espagne** (AEMET / Plan Calor) | Parcours par profil (enfants, personnes âgées, sportifs, travailleurs) avec fiches réflexes visuelles | Personnalisation par profil efficace et bien exécutée |
| **Canada** (Santé Canada) | Auto-évaluation du risque en ligne, outil interactif avec recommandations contextualisées | Validation de l'intérêt de l'auto-diagnostic |
| **Italie** (Ministero della Salute) | Bollettino quotidien par ville avec niveau de risque 0-3 et recommandations associées | Granularité communale du niveau d'alerte |

**Enseignement transversal :** Les pays les plus avancés combinent données météo temps réel, personnalisation par profil et géolocalisation. Aucun des sites benchmarkés n'a d'application mobile native dédiée — tous misent sur le web responsive.

---

## 4. Personas provisoires

### Persona 1 — Nadia, 36 ans, active urbaine

- **Situation :** Vit en appartement à Lyon (4e étage, plein sud, pas de clim). Deux enfants (3 et 6 ans).
- **Rapport à la chaleur :** S'inquiète surtout pour les enfants. A vécu un été 2023 difficile (nuits à 28°C dans l'appartement).
- **Sources d'info :** Appli Météo-France, Instagram, groupe WhatsApp de parents.
- **Besoin clé :** Savoir où emmener ses enfants quand il fait trop chaud (lieux frais, pataugeoires, bibliothèques climatisées). Conseils concrets pour rafraîchir l'appartement.
- **Citation :** « Je veux un truc qui me dit : il va faire 39° demain chez toi, voilà où aller avec les enfants. »

### Persona 2 — Michel, 72 ans, retraité en zone périurbaine

- **Situation :** Vit seul en maison à Montauban. Hypertension traitée. Jardin qu'il entretient même en été.
- **Rapport à la chaleur :** Ne se considère pas à risque. « J'ai toujours vécu ici, je connais la chaleur. »
- **Sources d'info :** JT de 13h, radio France Bleu, voisin. N'utilise pas Internet sauf pour les mails.
- **Besoin clé :** Prise de conscience de sa vulnérabilité. Relais via sa fille qui pourrait utiliser le diagnostic pour le sensibiliser.
- **Citation :** « C'est pas parce qu'il fait chaud que je vais arrêter de vivre. »

### Persona 3 — Sophie, 48 ans, auxiliaire de vie

- **Situation :** Accompagne 6 personnes âgées à domicile dans le quartier de la Goutte d'Or (Paris 18e). Tourne entre les domiciles en transports.
- **Rapport à la chaleur :** Très sensibilisée, a connu des situations critiques (personne de 88 ans en hyperthermie, été 2024).
- **Sources d'info :** Protocoles de son employeur, site de l'ARS IDF, appel à SOS Médecins.
- **Besoin clé :** Fiche réflexe imprimable, checklist quotidienne canicule pour chaque bénéficiaire, savoir quand appeler les secours vs. quand gérer en autonomie.
- **Citation :** « Quand je trouve Mme Dubois à 40°C de température corporelle dans son studio à 35°C, il me faut un protocole clair, pas un site internet. »

### Persona 4 — Karim, 31 ans, chef de chantier BTP

- **Situation :** Chef de chantier en Avignon. Gère une équipe de 12 ouvriers. Exposition directe au soleil 8h/jour en été.
- **Rapport à la chaleur :** Connaît les risques mais la pression des délais est forte. A déjà eu un ouvrier en malaise.
- **Sources d'info :** Son responsable sécurité, collègues, rien en ligne.
- **Besoin clé :** Connaître ses droits et ceux de son équipe (droit de retrait, obligations employeur), avoir un outil pour justifier un arrêt de chantier auprès de sa hiérarchie.
- **Citation :** « Si j'avais un truc officiel qui dit "à partir de tel seuil, vous devez arrêter", ça m'aiderait vis-à-vis de mon patron. »

---

## 5. Recommandations produit

### Axe 1 — Un produit centré sur la localisation et le temps réel

- Intégrer l'API Météo-France pour afficher le niveau de vigilance en temps réel, avec une granularité communale.
- Proposer un annuaire géolocalisé des lieux rafraîchis, alimenté par les collectivités et les ARS.
- Afficher des prévisions horaires locales avec des seuils clairs (« à partir de 14h, la température dépasse le seuil de danger dans votre zone »).

### Axe 2 — Personnalisation par profil et par contexte

- Proposer un auto-diagnostic de vulnérabilité comme porte d'entrée du site.
- Adapter les recommandations au profil (parent, aidant, travailleur, personne âgée) et au contexte (type de logement, activité).
- Créer des parcours dédiés avec des contenus spécifiques par segment.

### Axe 3 — Outiller les relais humains

- Créer un espace « aidant / professionnel » avec des fiches réflexes imprimables, des checklists et des protocoles.
- Fournir des contenus partageables (infographies, visuels pour réseaux sociaux) que les relais peuvent diffuser.
- Intégrer un lien direct vers les ressources locales (CCAS, SAMU Social, numéros d'urgence ARS).

### Axe 4 — Mobile-first, DSFR, accessible

- Conception mobile-first impérative (72 % des répondants consulteraient le site sur smartphone).
- Conformité DSFR native.
- Accessibilité RGAA AA minimum, avec attention particulière à l'accessibilité cognitive (langage clair, pictogrammes, contenus en FALC).
- Multilinguisme prioritaire : anglais, arabe, turc (populations allophones identifiées comme vulnérables par les ARS).

---

## 6. Prochaines étapes recommandées

| Étape | Échéance | Responsable |
|-------|----------|-------------|
| Validation de la vision produit par la DGS | 2 mai 2026 | Dr. Camille Renard |
| Rédaction des specs fonctionnelles (README repo) | 5-9 mai 2026 | Studio Produit |
| Réalisation des maquettes (wireframes puis UI) | 12-23 mai 2026 | Thomas K. (Designer) |
| Tests utilisateurs sur maquettes | 26-30 mai 2026 | Léa M. |
| Itération et validation design | 2-6 juin 2026 | Équipe Studio |
| Développement sprint 1 | 9 juin 2026 | Équipe dev |
| **Objectif de mise en ligne MVP** | **Fin juin 2026** | **Équipe produit** |

---

## Annexes

- Annexe A : Transcriptions anonymisées des 17 entretiens *(document séparé)*
- Annexe B : Données brutes du questionnaire — export CSV *(fichier joint)*
- Annexe C : Fiches benchmark détaillées par pays *(document séparé)*
- Annexe D : Enregistrements des sessions de test du site actuel *(accès restreint)*
- Annexe E : Formulaire de consentement utilisé

---

*Document interne — DNUM des Ministères Sociaux — Ne pas diffuser*
