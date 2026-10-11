# Contribuer

Le dépôt ne contient que du Markdown. Une entrée suit le format des fiches existantes : type, financeur, montant, licence, éligibilité, candidature, exemples, sources.

## Règles

- Chaque fait vient de la page officielle du programme. Pas de source officielle, pas d'entrée.
- Ce que la page ne dit pas s'écrit « non précisé ».
- Pas de chiffre issu d'un article de presse, d'un agrégateur ou d'un forum.
- Pas de date limite ni de statut d'ouverture : ils se périment. Décrire le fonctionnement (cycles, échéances périodiques) et renvoyer vers la page officielle.
- Un programme terminé va dans la section « Terminés » de la fiche de sa catégorie, ou dans [fiches/historique.md](fiches/historique.md) s'il n'a pas de catégorie claire. Il garde la date de fin donnée par la page officielle.
- Une affirmation qui dépend d'une année s'écrit avec cette année (« en 2025 »).
- Ajouter l'entrée dans le README et dans LICENCES.md.
- LICENCES.md liste tous les programmes actifs, avec ce que dit leur page sur la licence, ou « non précisée » quand la page ne dit rien, ainsi que les modèles de licence. Les services payants, funding.json, FUNDING.yml et les statuts français n'y figurent pas, sauf mention déjà présente.
- Toute contribution est publiée sous la même licence, CC BY-SA 4.0 (voir [LICENSE](LICENSE)).

## Contribuer sans connaître Git

Trois façons de participer, de la plus simple à la plus complète :

1. **Ouvrir une issue.** Onglet « Issues », puis « New issue » : le formulaire « Proposer un programme » ou « Signaler une erreur » indique ce qu'il faut fournir. Aucun fichier à modifier.
2. **Modifier un fichier depuis GitHub.** Ouvrir une fiche dans le dossier `fiches/`, cliquer sur le crayon, corriger, puis « Propose changes ». GitHub crée la pull request.
3. **Pull request classique.** Fork, modification en local, pull request. Le modèle de pull request rappelle les vérifications à faire.

Une proposition incomplète est acceptée : une issue avec le nom du programme et l'adresse de sa page officielle suffit, le reste peut être complété ensuite.

## Format d'une entrée

Chaque programme est une section `##` dans la fiche de sa catégorie. Les lignes qui ne s'appliquent pas peuvent être omises ; ce que la page ne dit pas s'écrit « non précisé ».

```markdown
## Nom du programme

- **Type** : subvention, bourse, parrainage fiscal, plateforme…
- **Structure** : organisme qui porte le programme
- **Montant** : montants ou frais, tels que la page les donne
- **Licence** : ce que la page dit de la licence, ou « non précisée »
- **Éligibilité** : qui peut candidater, conditions
- **Candidature** : comment candidater, sans date limite
- **Exemples** : projets financés, si la page en cite

**Sources** : [Titre de la page](https://adresse-de-la-page-officielle)
```

Entrées réelles à prendre comme exemples :

- [Software in the Public Interest](fiches/fondations-et-parrainage-fiscal.md#software-in-the-public-interest) : une entrée complète, avec citations de la page.
- [Open Source Collective](fiches/fondations-et-parrainage-fiscal.md#open-source-collective) : une entrée avec frais chiffrés et plusieurs sources.

Après l'ajout, renseigner aussi le programme dans le [README](README.md) et dans [LICENCES.md](LICENCES.md).
