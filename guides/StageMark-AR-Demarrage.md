# StageMark AR — démarrage rapide plateau

> Préversion AR 0.1.1 build 15 : relevé lissé et reconnaissance des cibles au sol ou sur pied. Les hauteurs nécessitent StageMark 2027.0.8 ou sa Beta ; les anciens PC restent utilisables avec des repères au sol. Signature de développement ; recette nécessaire sur chaque matériel. La vue est personnelle : elle ne remplace ni un vidéoprojecteur visible par tous, ni un instrument de mesure.

## Nouveau : choisir sol ou pied pour chaque cible

1. Dans **StageMark → Sorties & installation → Réalité augmentée → Guide pas à pas → Placement A/B/C**, choisissez **À plat au sol** ou **Verticale sur pied**, séparément pour A, B et C. Les coordonnées X/Y restent celles du projet. Travaillez sur une copie si vous comptez réouvrir le projet dans une version antérieure, qui ne conserve pas ces nouveaux réglages.
2. Pour un pied, mesurez **verticalement du sol local au centre du motif**, par exemple 140 cm. Entrez la hauteur réelle, pas la hauteur du pied ni une estimation « à hauteur d’homme ». Gardez le centre à l’aplomb du X/Y indiqué. La hauteur peut être différente pour chaque cible ; des cibles au sol et sur pied peuvent être mélangées.
3. Réutilisez vos feuilles, fixées à plat sur un support rigide, sans reflet. Pour un pied, le support est vertical ; l’image entière, marge blanche comprise, mesure **160 × 160 mm**, imprimée à 100 %. Ne déplacez pas les cibles entre A et C. La fiche PDF du projet rappelle support, X/Y et hauteur.
4. Démarrez l’AR sur le PC. Dans l’APK build 15, choisissez **Caméra du téléphone** puis associez le PC. Cadrez la bonne feuille entière et nette, suffisamment proche pour qu’elle occupe environ un quart de l’image caméra. **CIBLE A RECONNUE** confirme la lettre attendue ; il n’est pas nécessaire de viser exactement le centre avec la croix.
5. Touchez **Relever** une fois et gardez la feuille visible. Le relevé filtre les petites oscillations sur plusieurs images ; la coche confirme le point. Faites B puis C, puis **Valider et afficher les repères**. Le téléphone déduit le sol à partir de la hauteur déclarée, sans confondre celle-ci avec la pente de la scène.

**Si la reconnaissance est peu pratique au sol**, choisissez **Viser le sol manuellement** : l’ancien parcours reste disponible, avec le même lissage amélioré. Ce repli n’est pas proposé pour une cible sur pied, car mesurer le sol à sa place fausserait la hauteur. Une mauvaise lettre, une cible hors champ ou une mesure périmée ne valent pas un point reconnu.

Les petits écarts calculés restent acceptables après avertissement et consentement explicite. L’indice de cohérence masquable est indicatif, pas une précision garantie. Une reprise individuelle ne supprime pas les autres points suivis. Si une seule ancre ne revient pas après la courte attente, seul ce point est à reprendre ; une perte globale prolongée ou une interruption impose encore une nouvelle calibration.

**À vérifier sur chaque appareil avant exploitation** : trois cibles au sol, une cible sur pied, puis trois cibles sur pied ; vérifier physiquement une position connue et les masques AR PC/personnel. Les tests logiciels ne prouvent pas la reconnaissance optique ou la précision en salle. La publication de cette préversion ne vaut pas qualification terrain ; n’utilisez pas l’AR pour un repérage critique.

## Ce que dessine l’AR

Le build 14 corrige les objets qui apparaissaient comme une seule barre : praticables, rectangles, retours, amplis, pieds de micro et autres symboles ont maintenant leur contour au sol. Les cercles vides/pleins sont distincts, la croix est un X et les tracés libres conservent leurs courbes. Dimensions, rotation, couleur, épaisseur et opacité sont reprises du plan reçu. Il s’agit d’empreintes au sol, pas de volumes 3D représentant les équipements.

Les noms internes des objets ne deviennent pas automatiquement des étiquettes. Un objet texte et les dimensions d’un praticable font partie du symbole, comme sur le PC. Les étiquettes explicitement transmises restent affichées. Le protocole Desktop actuel ne transmet pas tous les réglages typographiques : taille et placement des textes utilisent des valeurs de repli dans l’APK. Les tracés libres fermés ont leur contour, sans remplissage intérieur. Ces limites ne changent ni les objets du projet ni la vidéoprojection.

La mise à jour de l’APK suffit pour cette correction ; aucun remplacement du logiciel PC ni déplacement des repères A/B/C n’est nécessaire. Relancez toutefois l’AR et calibrez après installation, comme après toute interruption de la session.

## Client tactile et démarrage direct

Pour relever un point, une seule pression suffit : gardez ensuite le centre visé. L’APK attend désormais jusqu’à **8 secondes** (au lieu de 3) et indique « Recherche du sol » puis la stabilisation. La coche confirme l’enregistrement et nomme le repère suivant. Une erreur distingue le sol non repéré d’une visée trop instable ; A/B/C déjà enregistrés ne sont pas effacés par cet échec. Cela laisse plus de temps sans assouplir la précision exigée des mesures ni inventer un sol absent.

Sur le PC : **Sorties & installation → Réalité augmentée → Démarrer l’AR**. Cette action ouvre la session et autorise les repères après association et calibration. Pas de second bouton Afficher obligatoire. Le guide pas à pas et les outils d’impression restent disponibles sans être imposés.

Le build 13 ajoute un relevé sur plusieurs images, une reprise des points ancrés après une courte perte de suivi pendant A/B/C, et la prise en compte d’un plateau régulièrement incliné jusqu’à 10 %. Il conserve l’interface tactile, la correction de pose native et les étiquettes sans nom automatique. Les vidéos A54 des versions précédentes montrent une croix et son changement de couleur reçus du PC ; elles ne qualifient pas ce correctif ni la précision métrique, la stabilité prolongée ou les lunettes. XREAL et RayNeo gardent la même priorité de développement ; RayNeo n’est pas encore activé dans cette APK.

- **Accueil** : Caméra du téléphone ou Lunettes XREAL ; les modes restent des choix explicites.
- **Connexion** : nom du projet, champ numérique à six chiffres et bouton Connecter. Un Wi-Fi d'hôtel peut laisser voir le PC mais bloquer la connexion ; préférer un réseau privé. Le relais USB employé pour le diagnostic n'est pas une fonction autonome distribuée.
- **Calibration** : A, B puis C, positions en mètres à trois décimales et progression lisible. Le bouton de relevé reste fixé en bas ; les détails et les reprises individuelles défilent au doigt dans le panneau.
- **Validation** : distances et avertissement, puis Valider et afficher ou Accepter l'écart si proposé. Un refus reste visible et ne retire aucun contrôle de cohérence.
- **Vue AR** : panneau compact, Masquer pour moi et Recalibrer accessibles. Réglages ouvre les explications et Quitter l'AR. En paysage, le panneau passe à côté de la caméra, jamais sur la cible.

Faites glisser les explications vers le haut pour lire la suite ; la barre verticale indique qu'il reste du contenu. Les actions principales ne défilent pas. Les sections suivantes décrivent le parcours métier commun ; les libellés peuvent être présentés en minuscules dans la nouvelle interface.

## Téléphone ou lunettes ?

L'APK **StageMark AR** accompagne l'unique application StageMark pour ordinateur. Choisissez **CAMÉRA DU TÉLÉPHONE** pour un Android ARCore (le Galaxy A54 5G figure dans la liste officielle Google), ou **LUNETTES XREAL** pour Air 2 Ultra + Beam Pro depuis MyGlasses. Le mode est choisi au démarrage ; relancez l'APK pour en changer. Le numéro visible reste 0.1.1 : vérifiez **build 13** à l'accueil pour distinguer cette mise à jour. Sur le PC, **Sorties & installation → Réalité augmentée** guide matériel, placement A/B/C, connexion et validation. L’AR seule ne demande pas d’ouvrir la sortie vidéo. Pour ce correctif, mettez à jour seulement l’APK : le Desktop 2027.0.6 déjà installé reste compatible.

Vous pouvez viser depuis votre hauteur normale : le motif n’a pas besoin de remplir l’écran. Touchez **Relever** une seule fois, puis gardez la croix sur le centre un court instant : l’application recherche une mesure stable pendant au maximum trois secondes. Elle confirme le point ou explique l’échec, sans effacer les autres points. **Annuler le relevé** interrompt l’attente. **Refaire A**, **B** ou **C** remplace seulement ce point après un nouveau relevé réussi ; **Garder le point précédent** annule cette reprise.

Le téléphone doit encore détecter un vrai plan de sol. Une petite marge près d’une zone déjà reconnue facilite la visée, mais l’application n’invente pas un sol quand le suivi est indisponible. Sur un plateau uniforme ou réfléchissant, scannez aussi autour des feuilles, dans une lumière stable. Même avec de la lumière, les reflets, surfaces sans texture ou changements d’éclairage peuvent limiter le suivi.

Pendant l’AR téléphone au premier plan, la veille automatique est suspendue pour éviter de refaire A/B/C à chaque extinction automatique. **Verrouiller manuellement le téléphone ou quitter l’application reste possible**, mais une interruption exige encore une nouvelle calibration. Quitter l’AR rétablit le comportement de veille précédent. Cela ne modifie pas les réglages système du téléphone.

## Premier essai sur téléphone

1. Sur le PC, créez par exemple une scène **2 m de large et 2 m de profondeur** dans un espace dégagé réellement mesuré. Ajoutez une croix nommée MIC 1 au centre (X 0, Y 1 m). Enregistrez votre projet normalement.
2. Repérez physiquement A = X -1 m / Y 0, B = X +1 m / Y 0 et C = X 0 / Y 2 m. Trois petits repères adhésifs dont les centres sont mesurés suffisent pour ce mode manuel ; ne changez pas d'échelle après mesure.
3. Activez **Sorties & installation → Réalité augmentée → Démarrer l’AR** sur le PC et utilisez le même Wi-Fi privé.
4. Dans l'APK, choisissez **CAMÉRA DU TÉLÉPHONE**, autorisez la caméra. Si demandé, choisissez **INSTALLER LES SERVICES AR** : cette installation Google initiale peut nécessiter Internet. Aucun enregistrement ou transfert de caméra n'est effectué par StageMark.
5. Saisissez le code à six chiffres du PC et **CONNECTER**. Bougez lentement le téléphone pour détecter le plateau bien éclairé et texturé. Une pente régulière de scène est acceptée jusqu’à 10 % (ce ne sont pas des degrés). Évitez reflets, obscurité et table ; placez les trois centres sur le même plateau, pas de part et d’autre d’une marche.
6. Placez la croix, au centre de la zone caméra dégagée, **au centre du motif noir/blanc A, pas au bord de la feuille**. Turquoise signifie **sol détecté**, pas marqueur reconnu. Touchez **RELEVER LE POINT A**, gardez le centre visé jusqu’à confirmation, puis faites de même pour B et C. Si le suivi s’interrompt brièvement entre deux points, ralentissez et regardez une zone déjà scannée : les points ancrés sont conservés jusqu’à 15 secondes et la reprise est automatique si les ancres sont retrouvées. Depuis les réglages, revenez d’abord à la caméra. Touchez **VALIDER ET AFFICHER LES REPÈRES** : le calcul est automatique, pente comprise. Si un écart est détecté, comparez les distances mesurées/attendues. Vous pouvez **ACCEPTER L’ÉCART ET AFFICHER L’AR** lorsque l’application le propose, ou reprendre un seul point.
7. Sur le PC, le démarrage autorise déjà les repères ; choisissez **AFFICHER AR** seulement si vous les aviez masqués. Vérifiez la croix MIC 1 à l'endroit mesuré. Marchez doucement, revenez et constatez l'écart. Un résidu faible de calibration ne garantit pas la précision réelle du suivi. Un plan vide est signalé : ajoutez un objet visible sur le PC.
8. **RÉGLAGES** ouvre le panneau complet ; **RECOMMENCER A / B / C** efface la calibration. Pause/verrouillage, perte réseau, perte du suivi une fois l’affichage calibré ou changement de géométrie masquent les marques et demandent de recalibrer. La conservation pendant 15 secondes concerne seulement le relevé A/B/C en cours, pas une calibration persistante après verrouillage. **QUITTER L'AR** libère la caméra. Le PC n'allume pas cette caméra à distance.

Les autres téléphones doivent être compatibles ARCore, Android 10 minimum et ARM64. Le démarrage vérifie la disponibilité ; une incompatibilité ou un refus caméra est affiché, pas masqué par un faux aperçu. La caméra donne une vue personnelle sur l'écran, pas des marques lumineuses réelles sur le sol.

### Si les feuilles ne sont pas placées exactement

L’application indique l’écart de calcul et laisse choisir **Accepter l’écart et afficher**. Pour un essai rapide, la tolérance va jusqu’à **1 mètre de résidu d’alignement et 30 % de différence de distance**. Ce sont des limites, pas une précision acceptable garantie : un écart important peut rendre le placement très approximatif. Rien n’est affiché automatiquement après l’avertissement : vous devez accepter les points qui viennent d’être mesurés. Vous pouvez aussi reprendre un seul point. Le plan garde sa taille réelle et la calibration du vidéoprojecteur ne change pas.

Dans la vue caméra, **Cohérence A/B/C · … %** est un petit indice indicatif. Touchez-le pour le masquer ; réaffichez-le depuis **Réglages → Afficher l’indicateur de cohérence**. Ce choix est mémorisé et ne masque pas les marques AR. Le score ne mesure ni la précision réelle, ni la qualité du placement des feuilles, ni la dérive du suivi : même 100 % demande de vérifier une position connue au mètre. Le détail des écarts reste dans les réglages ; **AR APPROXIMATIVE** signale l’acceptation d’un écart.

Une incohérence majeure reste bloquante : point manquant, triangle inversé/aplati, pente calculée supérieure à 10 %, écart calculé maximal supérieur à 1 m ou différence de distance supérieure à 30 %. Une différence de hauteur due à une pente régulière n’est plus refusée arbitrairement à 8 cm. Ces limites ne sont pas une précision garantie : trois points ne peuvent pas prouver que tout le plateau est un plan, ni détecter toute table ou marche. Vérifiez une position indépendante au mètre ; le suivi peut dériver. Toute pause ou perte du suivi retire l’accord approximatif précédent ; pendant le relevé, les points peuvent néanmoins être conservés si leurs ancres sont retrouvées dans le délai indiqué.

Si « Recherche de StageMark… » reste affiché, vérifier l'activation sur le PC et le réseau Wi-Fi privé commun. Si « StageMark trouvé » et le nom du projet apparaissent, la découverte a réussi : saisir le code du PC, puis **CONNECTER**. La découverte seule ne prouve ni la connexion, ni le suivi des lunettes, ni la calibration.

## Connexion et calibration dans les lunettes

### Feuilles permanentes, placement propre au projet

Les motifs A/B/C ne changent pas avec la scène. Gardez un jeu imprimé à 100 % et réutilisez-le. **Sorties & installation → Réalité augmentée → Marqueurs A/B/C** indique les coordonnées des centres en mètres (calculées en millimètres entiers). **Fiche de placement PDF du projet** et **Imprimer le placement** donnent une page séparée avec vue de dessus et tableau ; régénérez-la après changement de dimensions.

Deux cases indépendantes permettent **Afficher A/B/C sur le plan** et **Inclure A/B/C dans la projection**. Toutes deux sont désactivées par défaut. Ce sont des croix de position, pas les images à scanner. Cocher la projection n’ouvre aucune sortie et ne retire jamais le BLACKOUT : utilisez les commandes vidéo habituelles. Masquez les aides après installation. Sur une scène non rectangulaire, vérifiez l’accessibilité des centres ; les portions hors contour ne sont pas projetées. La précision du placement projeté dépend de la calibration du vidéoprojecteur : contrôlez les distances au mètre avant de calibrer l’AR.

### Procédure lunettes

1. Dans StageMark, ouvrez **Sorties & installation → Réalité augmentée**, puis choisissez **Marqueurs PDF réutilisables** ou **Imprimer les marqueurs**. Un seul jeu A/B/C sert pour toutes vos scènes ; les feuilles déjà imprimées restent compatibles. Imprimez à **100 % sans ajustement** : l’image complète, marge blanche comprise, mesure 160 × 160 mm. Chaque page rappelle où retrouver son emplacement dans le logiciel.
2. Placez **A**, **B** et **C** exactement aux positions affichées dans StageMark : A au nez Jardin, B au nez Cour, C au fond-centre.
3. Connectez le PC StageMark et le Beam Pro au même Wi-Fi privé.
4. Dans le même panneau Desktop, choisissez ce réseau puis cliquez **Démarrer l’AR**.
5. Dans les lunettes, ouvrez StageMark AR. Le message **StageMark trouvé : NOM-DU-PC** apparaît.
6. Recopiez le code à six chiffres affiché sur le PC, puis choisissez **CONNECTER**.
7. Regardez successivement A, B et C. Quand les trois sont relevés, choisissez **VALIDER ET AFFICHER LES REPÈRES**. Le démarrage sur le PC autorise déjà l’AR ; **AFFICHER AR** ne sert que si vous l’aviez ensuite masquée. Le SDK signale une faible richesse visuelle de ces images : leur reconnaissance réelle reste à qualifier.
8. N'utilisez les marques que si le statut indique **Tracking OK** ou **Calibration cohérente**. En cas de statut dégradé, arrêtez de vous fier aux positions et regardez à nouveau les marqueurs.
9. Vérifiez physiquement une croix connue avant de marcher sur toute la scène.

## Masquer et réafficher, sans couper l’autre diffusion

**AFFICHER AR / MASQUER AR** sur le PC concernent tous les compagnons AR, sans toucher à **AFFICHER / BLACKOUT** vidéo. Les quatre combinaisons sont possibles : vidéo seule, AR seule, les deux, rien. Masquer conserve connexion et calibration si le suivi reste valide ; **Arrêter la session AR** déconnecte les compagnons. **MASQUER POUR MOI / RÉAFFICHER POUR MOI** dans l’APK ne concerne que cette personne et ne peut jamais annuler un masquage du PC. La caméra reste visible et le suivi continue quand les repères sont masqués.

**Écran du PC couvert par la projection ?** Ctrl+Maj+F12 (Cmd+Maj+F12 sur Mac), Échap dans la fenêtre de sortie, ou **FERMER LA SORTIE** ferment la vidéo, son rideau noir et Spout, sans quitter le projet ni arrêter l’AR. **BLACKOUT** garde volontairement l’écran noir ; fermer la sortie peut montrer le bureau sur le projecteur, ce n’est pas une extinction électrique.

Pour installer le SDK, compiler l'APK, configurer les images A/B/C ou réaliser la recette complète, lire [STAGEMARK_AR.md](STAGEMARK_AR.md).
