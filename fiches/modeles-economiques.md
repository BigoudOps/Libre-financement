# Modèles économiques

## Fair Source

Le code est publié et la licence limite la concurrence directe, puis il devient open source après un délai.

- **FSL** (Functional Source License) : licence de non-concurrence simple, conversion en open source après deux ans. C'est la licence phare recommandée par fair.io.
- **FCL** (Fair Core License) : variante du FSL avec prise en charge des clés de licence, à envisager pour monétiser du logiciel auto-hébergé avec des fonctions commerciales.
- **BUSL** (Business Source License) : licence de non-concurrence plus complexe, conversion généralement après quatre ans.
- **Pas de l'open source au sens de l'OSI** : Sourcebot l'écrit explicitement après son passage de MIT à FSL (version 4.5.3, 20 juillet 2025), son cœur n'est plus sous licence open source approuvée par l'OSI.
- **Exemples** : Sourcebot (conversion en Apache 2.0 après deux ans) ; Keygen (FCL, conversion vers Apache 2.0 ou MIT après deux ans, selon son annonce)

**Sources** : [Fair Source — licences](https://fair.io/licenses/) ; [Sourcebot — passage à Fair Source (archive)](https://web.archive.org/web/20260402013758/https://sourcebot.dev/blog/fair-source) ; [Keygen — passage au FCL](https://keygen.sh/blog/keygen-is-now-fair-source/)

## Double licence

Le même logiciel est proposé sous une licence libre et sous une licence commerciale.

- **Exemple : MySQL.** Le serveur et les bibliothèques clientes sont disponibles sous GPLv2, avec une exception FOSS universelle pour les bibliothèques clientes. Une licence commerciale est proposée aux éditeurs et distributeurs qui intègrent MySQL à un logiciel commercial sans vouloir publier son code source sous GPLv2.
- **Ce que la licence commerciale permet** : distribuer des binaires MySQL avec un logiciel commercial sans que celui-ci soit soumis à la GPL

**Source** : [MySQL — licences OEM](https://www.mysql.com/about/legal/licensing/oem/)

## Open core

Positions publiées par des projets, sans définition commune.

- **Keygen** écrit viser un modèle « open core » avec la FCL et cite Plausible, GitLab, PostHog et Cal.com comme projets open core. Il précise que les fonctions commerciales ne deviennent jamais open source, sauf licence commerciale ponctuelle qui se comporte comme la BUSL ou la FSL.
- **Nextcloud** critique les produits « Open Core » : ses risques seraient similaires à ceux des logiciels propriétaires. Nextcloud ne se présente pas comme open core.

**Sources** : [Keygen — passage au FCL](https://keygen.sh/blog/keygen-is-now-fair-source/) ; [Nextcloud — licence et entreprises (article de 2018)](https://nextcloud.com/blog/how-nextcloud-protects-your-business-from-license-uncertainty)