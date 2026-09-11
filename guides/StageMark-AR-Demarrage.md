# StageMark AR — démarrage rapide plateau

> Desktop 2027.0.9 et APK 0.1.1 build 16. APK en préversion signée développement, Android 10+ ARM64. Les tests logiciels ne prouvent pas la précision sur votre scène : vérifiez toujours un emplacement connu. Aucun usage de repérage critique.

## Choisir l’affichage

Dans l’APK, choisissez **Caméra du téléphone** (Android compatible ARCore, dont Galaxy A54 5G) ou **Lunettes XREAL** (cible de test : Air 2 Ultra + Beam Pro). Le SDK identifie le modèle quand il le peut ; consultez Réglages. Le PC reçoit cette identification : aucun modèle à saisir une seconde fois sur le PC. Aucun changement automatique de SDK ; relancez l’APK pour changer de famille.

**RayNeo X3 Pro a la même priorité que XREAL**, mais la variante RayNeo actuelle est un diagnostic séparé. Elle interroge réellement le SDK OpenXR ARDK 1.1.2 pour la pose et les plans ; elle n’affiche pas encore les marques de scène. Aucune API d’ancre spatiale exploitable n’a été identifiée dans ce SDK. Un panneau fixé à la tête n’est pas un repère au sol. Ni toutes les lunettes XREAL, ni toutes les RayNeo ne sont déclarées compatibles.

## Préparer une fois, placer pour chaque projet

1. Imprimez les mêmes feuilles A/B/C à **100 %, sans ajustement** : image complète de 160 × 160 mm, marge blanche comprise. Gardez ce jeu pour les projets suivants.
2. Sur le PC : **Sorties & installation → Réalité augmentée → Guide pas à pas → Placement A/B/C**. Le logiciel donne X/Y ; seule la fiche de placement est propre au projet. Régénérez-la après modification des dimensions.
3. Pour chaque cible, choisissez **À plat au sol** ou **Verticale sur pied**. Sur pied, mesurez verticalement du sol local au **centre du motif** et entrez cette hauteur. Le centre reste à l’aplomb du X/Y prévu. Les hauteurs peuvent différer. Support rigide, sans reflet ; ne déplacez pas les cibles pendant le relevé.
4. **Afficher A/B/C sur le plan** et **Inclure A/B/C dans la projection** sont indépendants, désactivés par défaut. Ces croix de position ne remplacent pas les motifs à reconnaître. Elles n’ouvrent pas la sortie vidéo et n’annulent pas le BLACKOUT. Contrôlez les distances au mètre.

## Relier et calibrer

1. Ouvrez le projet sur le PC, ajoutez une croix à une position mesurée et enregistrez. Choisissez **Démarrer l’AR** dans Sorties & installation. Cela ouvre la session et autorise les marques après connexion et calibration, sans deuxième bouton obligatoire.
2. Utilisez le même Wi-Fi privé. Un Wi-Fi d’hôtel peut autoriser la découverte mais bloquer la connexion. « PC trouvé » n’est pas « connecté ». Le relais USB de diagnostic nécessite le PC et ses outils, ce n’est pas une liaison USB autonome.
3. Dans l’APK, choisissez l’affichage, autorisez la caméra si demandé et saisissez le code à six chiffres. Les services Google AR peuvent nécessiter Internet lors de leur première installation. StageMark n’enregistre ni ne transmet la caméra.
4. Sur téléphone, cadrez la feuille A entière, nette, sans reflet, assez proche pour que le motif soit reconnu. **CIBLE A RECONNUE** confirme la bonne lettre : inutile de centrer exactement la croix. Touchez **Relever** une seule fois et gardez la feuille visible jusqu’à la coche. L’attente est limitée à 8 secondes.
5. Au sol seulement, **Viser le sol manuellement** permet de viser le centre depuis votre hauteur, sans reconnaître le motif. Turquoise signifie alors sol détecté, pas image reconnue. Balayez autour de la feuille si nécessaire. Ce repli n’est pas proposé pour une cible sur pied.
6. Faites B puis C. **Refaire A/B/C** remplace un seul point après un relevé réussi ; les autres ancres suivies sont conservées. **Annuler le relevé** arrête l’attente. **Garder le point précédent** annule une reprise.
7. Touchez **Valider et afficher les repères**. Comparez les distances mesurées et prévues. Si l’application propose **Accepter l’écart et afficher**, vous pouvez accepter cet essai ou reprendre un point. Le plan conserve sa taille réelle.
8. Vérifiez la croix à l’endroit mesuré, marchez doucement et revenez. Le score de cohérence ne garantit ni la précision réelle ni l’absence de dérive.

## Relevé rapide, facultatif

Pendant A/B/C, **Relevé rapide (plus tolérant)** raccourcit la fenêtre minimale de stabilisation et tolère davantage de bruit autour de la mesure médiane, jusqu’à 10 cm. Il exige toujours plusieurs mesures fraîches, une vraie détection et un suivi actif. Une grande dérive de visée, une mauvaise lettre ou un sol absent ne deviennent pas une mesure valide.

Le mode standard reste disponible. Une calibration issue du mode rapide est signalée dans la vue AR. Ce mode est utile pour un essai, pas pour garantir une précision. La qualité affichée est la cohérence géométrique entre les trois relevés, pas une mesure de leur exactitude.

Pour un placement imparfait, le consentement peut accepter jusqu’à **1 m de résidu et 30 % de différence de distance**. Ce sont des bornes, pas une précision acceptable recommandée. Point manquant, triangle inversé/aplati, pente supérieure à 10 % ou écarts supérieurs aux limites restent refusés. Trois points ne prouvent pas l’absence de marche ou de table ; la scène doit être un même plan régulièrement incliné.

Touchez **Cohérence A/B/C · … %** pour masquer l’indicateur ; réaffichez-le dans Réglages. Même 100 % nécessite un contrôle indépendant.

## Perte de suivi et interruption

- Pendant le relevé sur téléphone : les points ancrés sont conservés jusqu’à 15 s. Regardez une zone déjà scannée et ralentissez. Seuls les points perdus sont à reprendre si le suivi revient.
- Après calibration sur téléphone : une courte interruption masque immédiatement les marques et conserve temporairement les ancres, jusqu’à 30 s. **Reprendre les repères** n’est proposé qu’après récupération stable des trois points et de l’ancre de scène, avec cohérence relative à 5 cm. Confirmez, puis vérifiez un emplacement connu.
- Si les ancres ne sont pas retrouvées, après déconnexion du PC, redémarrage de l’APK ou changement de géométrie/hauteur : refaites A/B/C. Ce n’est pas une carte persistante et aucune ancienne matrice n’est réaffichée après redémarrage.
- La reprise courte après calibration concerne le téléphone. Sur XREAL, une interruption demande encore de recalibrer.
- La veille automatique du téléphone est suspendue pendant l’AR au premier plan. Le verrouillage manuel reste possible ; Quitter l’AR rétablit la veille précédente.

## Dessins et masques

Desktop 2027.0.9 avec APK 16 transmet les remplissages, leurs couleurs/opacités, les contours composés et leurs trous, ainsi que la taille métrique des textes. Les courbes restent approximées pour le rendu. Les cotations sont des annotations du plan, pas des objets AR. Les tracés de plus de 2 048 points sont refusés explicitement plutôt que coupés ; simplifiez-les. Un rejet de dessin masque l’AR.

Les anciennes APK sont privées de dessins enrichis qu’elles ne sauraient afficher correctement. Mettez à jour l’APK et le Desktop ensemble. Conservez une copie avant d’ouvrir un projet dans une version ancienne qui ignore les hauteurs.

**Afficher AR / Masquer AR** sur le PC affecte tous les compagnons, indépendamment de **Afficher / BLACKOUT** vidéo. Vidéo seule, AR seule, les deux ou rien sont possibles. **Masquer pour moi** n’affecte que ce compagnon et ne peut annuler le masque du PC. Masquer conserve caméra et suivi ; **Arrêter la session AR** déconnecte les compagnons.

La vue caméra affiche les marques seulement sur l’écran du téléphone. Les lunettes offrent une vue personnelle. Pour des marques lumineuses réellement visibles par tout le monde au sol, il faut un ou plusieurs vidéoprojecteurs.

**Écran PC couvert par la sortie ?** Ctrl+Maj+F12 (Cmd+Maj+F12 sur Mac), Échap dans la fenêtre de projection ou **Fermer la sortie** ferment vidéo, rideau noir et Spout sans quitter le projet ni arrêter l’AR. BLACKOUT garde volontairement la fenêtre noire ; fermer la sortie peut montrer le bureau au projecteur.

## Premier essai XREAL

Avec Air 2 Ultra + Beam Pro, ouvrez l’APK depuis MyGlasses et sélectionnez XREAL. Même Wi-Fi privé, code du PC, puis observez A/B/C avant de valider. Vérifiez physiquement une position connue. Reconnaissance, affichage stéréoscopique, interaction et stabilité restent à qualifier sur les lunettes réelles. La présence du SDK ne certifie pas le fonctionnement.

Documentation fabricant : [XREAL](https://docs.xreal.com/) ; [RayNeo](https://rayneo-en.gitbook.io/rayneo-devdoc). Ces liens décrivent les plateformes, pas une certification StageMark.
