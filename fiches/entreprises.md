# Entreprises

# Dernière modification : 2026-10-16 18:12:46

## Open Source Pledge

- **Type** : engagement d'entreprises, sans candidature
- **Principe** : les entreprises membres versent en espèces plus de 2 000 $ par an et par développeur employé, directement aux mainteneurs et aux fondations
- **Membres cités sur la page** : Posit, AG Grid, Sentry, Sanity, Zerodha, Mux
- **Utilité** : repérer les entreprises qui financent des mainteneurs et les contacter
- **Exemple** : Zerodha déclare 823 281 $ de contributions sur 12 mois en 2025 (239 600 $ en 2024)

**Sources** : [Open Source Pledge](https://opensourcepledge.com) ; [Zerodha — rapport 2025](https://zerodha.com/open-source/2025-report/)

## thanks.dev

- **Type** : répartition automatique d'un don entre les dépendances du donateur, sans candidature
- **Fonctionnement** : le donateur donne accès à son code hébergé sur GitHub ou GitLab et choisit un montant. thanks.dev lit les fichiers manifestes, établit l'arbre des dépendances jusqu'à 3 niveaux et répartit le don en largeur d'abord : chaque niveau reçoit (1/2)^n du don (n = profondeur), partagé entre les dépendances de ce niveau au prorata de leur fréquence. Dépendances circulaires et dépendances de développement transitives exclues. Le donateur peut exclure des projets ou en pondérer (« boost »).
- **Écosystèmes** : Go (go.mod), Java (pom.xml), JavaScript (package.json), Python (requirements, Pipfile, pyproject.toml), PHP (composer.json), Ruby (Gemfile), Rust (Cargo.toml). Elixir désactivé ; Objective-C, Swift et .NET annoncés, sans date.
- **Frais** : au moins 5 % prélevés sur le don, côté donateur. Aucun frais pour les mainteneurs, mais les frais de GitHub Sponsors ou d'Open Collective sont répercutés.
- **Pour le développeur** : seuls les projets inscrits sur thanks.dev reçoivent de l'argent. L'inscription passe par GitHub, pour vérifier les droits d'administration (l'accès peut être limité à un seul dépôt public). Versements par Stripe Connect, GitHub Sponsors ou Open Collective, arrondis au dollar inférieur, à partir de 1 $ de solde. Un solde non réclamé pendant plus de 3 mois est redistribué aux autres bénéficiaires du donateur.
- **Délai** : un don reste 7 jours en attente (ajustement ou remboursement possible) avant d'être distribué
- **Entreprises citées sur la page** : Canonical, Square, Sentry, Sourcegraph, Frontend Masters
- **Licence** : aucune condition mentionnée

**Sources** : [thanks.dev](https://thanks.dev/) ; [thanks.dev — How does thanks.dev work?](https://thanks.dev/static/how) ; [thanks.dev — ecosystems](https://thanks.dev/static/ecosystems) ; [thanks.dev — FAQ](https://thanks.dev/faq)

## Copie publique

- **Type** : engagement d'entreprises, sans candidature
- **Principe** : en trois règles. Rétribution : « Une enveloppe variable annuelle dont le montant est déterminé par une formule librement adoptée par l'entreprise », qui dépend des états financiers annuels. Démocratie : l'enveloppe est répartie chaque année par les salariés et salariées, par choix individuel ou par vote collectif. Redistribution : « Le montant bénéficie à des projets ou des initiatives du Libre ».
- **Entreprises participantes et formules** : Arawa (6 % du bénéfice net), Néréide (3 % de l'excédent net de gestion), Code Lutin, IndieHosters, John Livingston, OuestWare, Ouvaton et simplementWeb (1 % du chiffre d'affaires), XWiki SAS (1 % du chiffre d'affaires récurrent)
- **Bilan affiché** : 200 762 € redistribués, 9 entreprises participantes, 160 projets bénéficiaires. La page détaille les versements de 2011 à 2025 (aucun en 2017 et 2018), par année, entreprise et bénéficiaire, de 13 € à 9 000 €.
- **Exemples** (2025) : YunoHost (5 000 €), Open Food Facts (3 000 €), inventaire (2 000 €), Fondation Matrix (939 €), Mobilizon (625 €) ; aussi Framasoft, F-Droid, GIMP, Krita, OpenStreetMap, Let's Encrypt
- **Pour le développeur** : financement surtout indirect. Les versements vont en majorité à des projets, associations ou fondations (Framasoft, Wikimedia France, Fondation Matrix…), qui décident de leur usage ; quelques-uns vont directement à des personnes (par exemple David Revoy en 2024, kovidgoyal en 2019). Pour en bénéficier, un projet doit être choisi par le personnel d'une entreprise participante, sans candidature possible. Un guide pour les salariés sert à demander la mise en place du dispositif à son employeur.
- **Structure** : site édité par Code Lutin (SAS à participation ouvrière), l'une des entreprises participantes ; soutiens affichés : April et CNLL
- **Licence** : aucune condition nommée ; vise des « projets ou des initiatives du Libre »

**Source** : [Copie publique](https://copiepublique.fr/)

## Microsoft FOSS Fund

- **Type** : fonds d'entreprise, sans candidature des projets
- **Principe** : chaque trimestre, « up to $12,500 USD across one or more open source project(s) » ; une ancienne section de la même page indique « up to 10,000 », sans devise. Toute personne salariée ou stagiaire chez Microsoft peut proposer un projet ; votent les salariés qui contribuent à un projet open source sur GitHub. Propositions acceptées en continu, sélection trimestrielle.
- **Conditions pour le projet** : utilisé par Microsoft ; « The project must have an OSI-approved open source license » ; capable de recevoir des fonds acceptés par les services achats et juridique de Microsoft (GitHub Sponsors de préférence) ; pas détenu par un salarié de Microsoft ; la diversité, l'équité et l'inclusion sont à privilégier dans les propositions
- **Exemples** : FOSS Fund 36 (mars 2026) : actix, aiohttp, Apache Solr, cheerio, cucumber, onnx, byte-buddy, core-js… ; tours antérieurs : webpack, Godot Engine, GNOME, OpenSSL, curl, OpenStreetMap, QEMU, Debian, LLVM, Mastodon
- **Pour le développeur** : être une dépendance utilisée chez Microsoft et proposée par une personne salariée

**Source** : [Microsoft — FOSS Fund](https://github.com/microsoft/foss-fund)

## Spotify FOSS Fund

- **Type** : fonds d'entreprise, sans candidature des projets
- **Principe** : créé en 2022 avec 100 000 € pour la première année. Les équipes R&D de Spotify proposent des projets, en s'appuyant sur les données de dépendances de ses dépôts internes ; un comité choisit parmi les projets éligibles.
- **Critères** (annonce de 2022) : projets gérés de façon indépendante, pas par des personnes employées par Spotify, conformes aux valeurs de l'entreprise, activement maintenus, et pour lesquels le soutien financier compte vraiment
- **Exemples** (fonds 2025, article de janvier 2026) : FFmpeg (30 000 €), Mock Service Worker (15 000 €), Xiph.Org Foundation (25 000 €)
- **Licence** : aucune condition mentionnée

**Sources** : [Spotify — annonce du FOSS Fund (2022)](https://engineering.atspotify.com/2022/4/announcing-the-spotify-foss-fund) ; [Spotify — bénéficiaires 2025](https://engineering.atspotify.com/2026/1/congratulations-to-the-recipients-of-the-2025-spotify-foss-fund)

