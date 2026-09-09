# StageMark AR — démarrage rapide plateau

> Préversion technique 0.1.1 build 7 : caméra Android ARCore et lunettes XREAL. Signature de développement ; recette physique nécessaire sur chaque matériel. Ne remplace ni un vidéoprojecteur visible par tous, ni un instrument de mesure, ni la sécurité du plateau.

## Téléphone ou lunettes ?

L'APK **StageMark AR** accompagne l'unique application StageMark pour ordinateur. Choisissez **CAMÉRA DU TÉLÉPHONE** pour un Android ARCore (le Galaxy A54 5G figure dans la liste officielle Google), ou **LUNETTES XREAL** pour Air 2 Ultra + Beam Pro depuis MyGlasses. Le mode est choisi au démarrage ; relancez l'APK pour en changer. Le numéro visible reste 0.1.1 : vérifiez **build 7** à l'accueil pour distinguer cette mise à jour. Sur le PC, **Connexion → Réalité augmentée** guide matériel, placement A/B/C, connexion et validation. L’AR seule ne demande pas d’ouvrir la sortie vidéo. Le Desktop 2027.0.5 guidé déjà installé reste compatible : seule l’APK est à remplacer pour ce correctif.

Le build 7 corrige la liaison des mouvements du téléphone avec la caméra virtuelle : une calibration acceptée ne suffisait pas à rendre les marques visibles dans le build précédent. Les corrections du relevé tactile sont conservées. Vous pouvez viser depuis votre hauteur normale : le motif n’a pas besoin de remplir l’écran. Le toucher recontrôle immédiatement le sol ; si le point ne peut pas être relevé, un message explique pourquoi. Aucun point ancien n’est réutilisé.

Pendant l’AR téléphone au premier plan, la veille automatique est suspendue pour éviter de refaire A/B/C à chaque extinction automatique. **Verrouiller manuellement le téléphone ou quitter l’application reste possible**, mais une interruption exige encore une nouvelle calibration. Quitter l’AR rétablit le comportement de veille précédent. Cela ne modifie pas les réglages système du téléphone.

## Premier essai sur téléphone

1. Sur le PC, créez par exemple une scène **2 m de large et 2 m de profondeur** dans un espace dégagé réellement mesuré. Ajoutez une croix nommée MIC 1 au centre (X 0, Y 1 m). Enregistrez votre projet normalement.
2. Repérez physiquement A = X -1 m / Y 0, B = X +1 m / Y 0 et C = X 0 / Y 2 m. Trois petits repères adhésifs dont les centres sont mesurés suffisent pour ce mode manuel ; ne changez pas d'échelle après mesure.
3. Activez **Connexion → Réalité augmentée → ACTIVER STAGEMARK AR** sur le PC et utilisez le même Wi-Fi privé.
4. Dans l'APK, choisissez **CAMÉRA DU TÉLÉPHONE**, autorisez la caméra. Si demandé, choisissez **INSTALLER LES SERVICES AR** : cette installation Google initiale peut nécessiter Internet. Aucun enregistrement ou transfert de caméra n'est effectué par StageMark.
5. Saisissez le code à six chiffres du PC et **CONNECTER**. Bougez lentement le téléphone pour détecter un sol horizontal bien éclairé et texturé. Évitez tapis uni, reflets, obscurité et table.
6. Placez la croix, au centre de la zone caméra dégagée, **au centre du motif noir/blanc A, pas au bord de la feuille**. Turquoise signifie **sol détecté**, pas marqueur reconnu. Touchez **RELEVER LE POINT A**, puis faites de même pour B et C. Depuis les réglages, revenez d’abord à la caméra : on ne peut pas relever un point sans voir la cible. Touchez **VALIDER ET AFFICHER LES REPÈRES** : le calcul est automatique. Si un écart est détecté, comparez les distances mesurées/attendues. Vous pouvez **ACCEPTER L’ÉCART ET AFFICHER L’AR** lorsque l’application le propose, ou reprendre un point avec **Refaire A/B/C**.
7. Sur le PC, choisissez **AFFICHER AR** (la session démarre masquée). Vérifiez la croix MIC 1 à l'endroit mesuré. Marchez doucement, revenez et constatez l'écart. Un résidu faible de calibration ne garantit pas la précision réelle du suivi. Un plan vide est signalé : ajoutez un objet visible sur le PC.
8. **RÉGLAGES** ouvre le panneau complet ; **RECOMMENCER A / B / C** efface la calibration. Pause, perte de suivi/réseau ou changement de géométrie masquent les marques et demandent de recalibrer. **QUITTER L'AR** libère la caméra. Le PC n'allume pas cette caméra à distance.

Les autres téléphones doivent être compatibles ARCore, Android 10 minimum et ARM64. Le démarrage vérifie la disponibilité ; une incompatibilité ou un refus caméra est affiché, pas masqué par un faux aperçu. La caméra donne une vue personnelle sur l'écran, pas des marques lumineuses réelles sur le sol.

### Si les feuilles ne sont pas placées exactement

L’application indique l’écart de calcul et laisse choisir un **alignement approximatif** plutôt que bloquer un petit décalage. Après acceptation, **AR APPROXIMATIVE** reste visible : les marques peuvent être décalées. Cela ne déforme pas le plan et ne change pas la calibration du vidéoprojecteur. Vous pouvez replacer les feuilles et **RECOMMENCER A / B / C** quand vous le souhaitez.

Une incohérence majeure reste bloquante : point manquant, triangle inversé/aplati, sol de hauteur différente, écart calculé maximal supérieur à 50 cm ou différence de distance supérieure à 15 %. Ces limites ne sont pas une précision garantie. Même avec un calcul cohérent, vérifiez une position indépendante au mètre ; le suivi peut dériver. Toute pause ou perte du suivi retire l’accord précédent et impose une nouvelle calibration.

Si « Recherche de StageMark… » reste affiché, vérifier l'activation sur le PC et le réseau Wi-Fi privé commun. Si « StageMark trouvé » et le nom du projet apparaissent, la découverte a réussi : saisir le code du PC, puis **CONNECTER**. La découverte seule ne prouve ni la connexion, ni le suivi des lunettes, ni la calibration.

## Connexion et calibration dans les lunettes

### Feuilles permanentes, placement propre au projet

Les motifs A/B/C ne changent pas avec la scène. Gardez un jeu imprimé à 100 % et réutilisez-le. **Connexion → Réalité augmentée → Placement A/B/C** indique les coordonnées des centres en mètres (calculées en millimètres entiers). **Fiche de placement PDF du projet** et **Imprimer le placement** donnent une page séparée avec vue de dessus et tableau ; régénérez-la après changement de dimensions.

Deux cases indépendantes permettent **Afficher A/B/C sur le plan** et **Inclure A/B/C dans la projection**. Toutes deux sont désactivées par défaut. Ce sont des croix de position, pas les images à scanner. Cocher la projection n’ouvre aucune sortie et ne retire jamais le BLACKOUT : utilisez les commandes vidéo habituelles. Masquez les aides après installation. Sur une scène non rectangulaire, vérifiez l’accessibilité des centres ; les portions hors contour ne sont pas projetées. La précision du placement projeté dépend de la calibration du vidéoprojecteur : contrôlez les distances au mètre avant de calibrer l’AR.

### Procédure lunettes

1. Dans StageMark, ouvrez **Connexion → Réalité augmentée**, puis choisissez **Marqueurs PDF réutilisables** ou **Imprimer les marqueurs**. Un seul jeu A/B/C sert pour toutes vos scènes ; les feuilles déjà imprimées restent compatibles. Imprimez à **100 % sans ajustement** : l’image complète, marge blanche comprise, mesure 160 × 160 mm. Chaque page rappelle où retrouver son emplacement dans le logiciel.
2. Placez **A**, **B** et **C** exactement aux positions affichées dans StageMark : A au nez Jardin, B au nez Cour, C au fond-centre.
3. Connectez le PC StageMark et le Beam Pro au même Wi-Fi privé.
4. Dans le même panneau Desktop, choisissez ce réseau puis cliquez **ACTIVER STAGEMARK AR**.
5. Dans les lunettes, ouvrez StageMark AR. Le message **StageMark trouvé : NOM-DU-PC** apparaît.
6. Recopiez le code à six chiffres affiché sur le PC, puis choisissez **CONNECTER**.
7. Regardez successivement A, B et C. Quand les trois sont relevés, choisissez **VALIDER ET AFFICHER LES REPÈRES**, puis **AFFICHER AR** sur le PC. Le SDK signale une faible richesse visuelle de ces images : leur reconnaissance réelle reste à qualifier.
8. N'utilisez les marques que si le statut indique **Tracking OK** ou **Calibration cohérente**. En cas de statut dégradé, arrêtez de vous fier aux positions et regardez à nouveau les marqueurs.
9. Vérifiez physiquement une croix connue avant de marcher sur toute la scène.

## Masquer et réafficher, sans couper l’autre diffusion

**AFFICHER AR / MASQUER AR** sur le PC concernent tous les compagnons AR, sans toucher à **AFFICHER / BLACKOUT** vidéo. Les quatre combinaisons sont possibles : vidéo seule, AR seule, les deux, rien. Masquer conserve connexion et calibration si le suivi reste valide ; **Arrêter la session AR** déconnecte les compagnons. **MASQUER POUR MOI / RÉAFFICHER POUR MOI** dans l’APK ne concerne que cette personne et ne peut jamais annuler un masquage du PC. La caméra reste visible et le suivi continue quand les repères sont masqués.

**Écran du PC couvert par la projection ?** Ctrl+Maj+F12 (Cmd+Maj+F12 sur Mac), Échap dans la fenêtre de sortie, ou **FERMER LA SORTIE** ferment la vidéo, son rideau noir et Spout, sans quitter le projet ni arrêter l’AR. **BLACKOUT** garde volontairement l’écran noir ; fermer la sortie peut montrer le bureau sur le projecteur, ce n’est pas une extinction électrique.

Pour télécharger l’APK et retrouver les vérifications et limites de cette version, lire les [notes de version](../RELEASE_NOTES_AR_BUILD7.md).
