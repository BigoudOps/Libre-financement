# Plateformes

## Open Collective

- **Principe** : un collectif reçoit des contributions ; un hébergeur fiscal (organisation juridique) détient les fonds des collectifs qu'il soutient
- **Frais de plateforme** pour les organisations (grille des nouveaux clients depuis mars 2026) : Discover 0 $/mois (1 collectif actif, 10 dépenses payées par mois), Basic 60 $/mois (5 collectifs, 50 dépenses), Pro 320 $/mois (20 collectifs, 200 dépenses). Les collectifs restent gratuits à utiliser.
- **Contributions** : gratuites si les « Platform Tips » facultatifs sont activés, ou frais fixes de 5 % sur les fonds entrants sur demande. L'ancien modèle prélevait 15 % sur les frais d'hébergement.
- **Non précisé sur la page** : frais de traitement des paiements, frais des hébergeurs fiscaux, conditions propres aux projets open source
- **Licence** : aucune condition mentionnée

**Source** : [Open Collective — tarifs](https://opencollective.com/pricing)

## Liberapay

- **Principe** : dons récurrents, sans contrepartie, plafonnés à 100 $ par semaine et par donateur ; montants donnés et reçus publics par défaut
- **Forme juridique** : organisation à but non lucratif fondée en 2015 en France ; le code est sur GitHub
- **Frais** : Liberapay ne prélève pas de commission ; des frais de traitement des paiements existent, détaillés dans leur FAQ
- **Licence** : aucune condition mentionnée

**Source** : [Liberapay — à propos](https://liberapay.com/about/)

## Tidelift

- **Principe** : Tidelift, qui fait désormais partie de Sonar, paie les mainteneurs (« lifters ») dont les paquets respectent un ensemble documenté de standards. Le revenu dépend de plusieurs facteurs, dont l'usage par les abonnés (calculé d'après les SBOM que les clients téléversent) et un poids fondé principalement sur la taille du code, avec des ajustements.
- **Paiement** : l'usage et le statut de lifter sont relevés le dernier jour ouvré du mois ; les paiements partent le troisième jour ouvré du mois suivant, vers un portefeuille Hyperwallet. Tidelift peut payer des personnes comme des organisations, à but lucratif ou non, dès lors qu'un accord signé existe. Avec plusieurs co-mainteneurs, le premier mainteneur reçoit par défaut tous les revenus ; chaque co-mainteneur doit signer l'accord. Les paiements vers des pays ou banques sous sanctions sont bloqués.
- **Tâches demandées** : activer l'authentification à deux facteurs sur GitHub et sur le gestionnaire de paquets ; documenter clairement le type de licence du paquet ; documenter une politique de sécurité et un plan de maintenance de sécurité, fournir un retour sur les vulnérabilités et créer une version corrective ; renseigner l'URL du dépôt et le schéma de versions ; vérifier que seules des personnes autorisées gèrent les publications. Les standards peuvent évoluer.
- **Ce que Tidelift dit ne pas demander** : support technique ou conseil, abandon du contrôle de la feuille de route, changement du type de licence
- **Retrait** : « vous pouvez arrêter de lifter un paquet à tout moment » (page de support Tidelift)
- **Non précisé sur les pages** : écosystèmes pris en charge, montant minimum de versement, montants versés par paquet, licences acceptées

**Sources** : [Sonar — mainteneurs open source (Tidelift)](https://www.sonarsource.com/open-source-maintainers/) ; [Tidelift — comment les lifters sont payés](https://support.tidelift.com/hc/en-us/articles/4406294816916-How-we-pay-lifters) ; [Tidelift — tâches des lifters](https://support.tidelift.com/hc/en-us/articles/4406288074260-Lifter-tasks-overview)


## funding.json

- **Principe** : manifeste JSON autonome qui permet à un projet libre de déclarer ses besoins de financement dans un format lisible par machine, comparé par sa page à robots.txt. Il se publie dans un dépôt ou sur un site, sans emplacement imposé : les exemples de la page montrent la racine d'un site (`https://example.com/funding.json`) et un chemin de dépôt. Un fichier `/.well-known/funding-manifest-urls` sert à vérifier des URL hébergées sur un autre nom de domaine que le manifeste.
- **Champs obligatoires** : au niveau racine, `entity` et `funding`. `entity` : `type`, `role`, `name`, `email`, `description`, `webpageUrl.url`. `funding.channels[]` : `guid`, `type`. `funding.plans[]` : `guid`, `status`, `name`, `amount`, `currency`, `frequency`, `channels`. Pour chaque projet déclaré dans `projects[]` : `guid`, `name`, `description`, `webpageUrl.url`, `repositoryUrl.url`, `licenses`, `tags`.
- **Outils** : un validateur en ligne (dir.floss.fund/validate) et un constructeur de manifeste sont liés depuis la page. La page cite l'annuaire de FLOSS/fund parmi les outils, voir [FLOSS/fund](fonds-prives.md#flossfund-zerodha).
- **Licence de la spécification, conditions d'éligibilité** : non précisées sur la page

**Source** : [funding.json](https://fundingjson.org/)

## FUNDING.yml (bouton de soutien d'un dépôt GitHub)

Ce fichier ajoute un bouton de soutien à un dépôt GitHub. Il n'est utile que si le dépôt y est hébergé ou en miroir, mais il liste des plateformes hors GitHub Sponsors.

- **Emplacement** : fichier `FUNDING.yml` dans le dossier `.github` du dépôt, sur la branche par défaut
- **Plateformes prises en charge** (syntaxe de la documentation) :
  - `community_bridge: PROJET` (LFX Mentorship)
  - `github: UTILISATEUR` (un compte d'organisation et jusqu'à quatre développeurs)
  - `issuehunt: UTILISATEUR`
  - `ko_fi: UTILISATEUR`
  - `liberapay: UTILISATEUR`
  - `open_collective: UTILISATEUR`
  - `patreon: UTILISATEUR`
  - `tidelift: PLATEFORME/PAQUET`
  - `polar: UTILISATEUR`
  - `buy_me_a_coffee: UTILISATEUR`
  - `thanks_dev: u/gh/UTILISATEUR`
  - `custom: LIEN` : jusqu'à quatre URL personnalisées, utiles pour toute autre plateforme
- **Limite** : chaque plateforme externe prend un seul identifiant (utilisateur, paquet ou projet)

**Source** : [GitHub — afficher un bouton de soutien](https://docs.github.com/en/repositories/managing-your-repositorys-settings-and-features/customizing-your-repository/displaying-a-sponsor-button-in-your-repository)


## Kickstarter

- **Principe** : financement participatif de projets créatifs, dont du logiciel
- **Frais** : 5 % prélevés par Kickstarter sur les fonds collectés si le projet est financé, plus les frais de paiement de Stripe, « roughly 3-5 % ». Si l'objectif n'est pas atteint, aucun frais n'est prélevé.
- **Non précisé sur la page lue** : les pays d'où l'on peut lancer un projet, les conditions propres aux projets open source
- **Licence** : aucune condition mentionnée

**Source** : [Kickstarter — frais](https://help.kickstarter.com/hc/en-us/articles/115005028634-What-are-the-fees)

## Ulule

- **Principe** : financement participatif en France et en Europe
- **Commission** : pour un projet en euros collectant moins de 100 000 €, 6,67 % HT en cas de paiement par carte bancaire et 4,17 % HT en cas de paiement par chèque. En mode récompense, elle n'est prélevée que si l'objectif est atteint ; en mode don, elle s'applique à tous les fonds transférés. Au-delà de 100 000 €, les taux baissent par paliers (carte de 5,83 % à 4,17 %, chèque de 3,33 % à 1,67 %). La TVA dépend du pays du porteur de projet.
- **Frais pour les contributeurs** : depuis le 14 avril 2025, 0,10 € plus 2,2 % TTC par contribution, à la charge des contributeurs seuls
- **Conditions pour lancer un projet** : être majeur et vivre dans un pays qui utilise l'une des devises prises en charge (euro, dollar américain ou canadien, franc suisse, livre sterling). L'inscription et l'utilisation du site sont gratuites. Types de structures (particulier, association, entreprise) et projets acceptés : non précisés sur la page lue.
- **Licence** : aucune condition mentionnée

**Sources** : [Ulule — commission](https://support.ulule.com/hc/en-us/articles/211812409-What-is-Ulule-s-commission) ; [Ulule — qui peut utiliser Ulule](https://support.ulule.com/hc/en-us/articles/212423385-Who-can-use-Ulule-How-much-does-it-cost-to-join)

