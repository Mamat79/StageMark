# Banque de vidéoprojecteurs StageMark

`catalog.json` est la banque V2 lisible et versionnée. `manifest.json` publie sa version, sa taille exacte et son SHA-256. StageMark lit d’abord ce manifeste (64 Kio maximum), puis accepte le catalogue (2 Mio maximum) uniquement si taille et empreinte correspondent avant l’analyse JSON. Le manifeste du cache est remplacé en dernier : une copie interrompue ou déchirée est refusée et la banque intégrée hors ligne reste disponible.

Le lecteur accepte encore un catalogue V1 accompagné d’un manifeste valide et le normalise en mémoire vers V2. Une image V1 est volontairement écartée, car cet ancien format ne portait aucune licence de redistribution explicite. Le fichier publié aujourd’hui est déjà au format V2.

Chaque fiche fournit des sources constructeur officielles structurées et datées, la résolution, la valeur et l’unité de luminosité annoncée, la technologie, la source lumineuse, le poids, les orientations autorisées et au moins un objectif. Les champs techniques V2 peuvent préciser dimensions, consommation, bruit, entrées, lens shift, correction géométrique et edge blending.

Une photo est facultative. Elle n’est affichée que si sa taille, son SHA-256, son attribution et une licence explicitement redistribuable sont présents. Un lien sans licence ou un filigrane ne vaut jamais autorisation : StageMark affiche alors sa silhouette neutre. Voir [LICENSE.md](LICENSE.md).

Dans l’application, les filtres et les tris travaillent uniquement sur cette copie locale. Les favoris sont enregistrés dans les préférences du poste : ils ne modifient ni le projet ni le catalogue et ne sont envoyés à aucun service.

Choisir une fiche et un objectif copie dans le projet l’identifiant du modèle, la version de la banque, l’identifiant et le nom de l’objectif, la résolution et la plage de rapports optiques. Le profil de calibration ne reprend ce matériel que lorsque l’opérateur utilise explicitement l’action d’association.

Les contributions passent par une issue ou une pull request GitHub. Elles doivent citer la page ou la fiche technique officielle, préciser l’unité de luminosité et ne doivent contenir ni donnée personnelle, ni prix commercial, ni fichier dont la republication n’est pas autorisée. Une contribution ne devient jamais active automatiquement : elle est relue, testée et commitée avant publication.

Le catalogue aide au pré-calcul. Les fiches constructeur et l’essai sur site restent prioritaires.
