# StageMark 2027.0.9 — formes AR, relevé rapide et reprise contrôlée

Avec le compagnon **StageMark AR 0.1.1 build 16**, toujours en préversion :

- Remplissages, opacités, tailles de texte et contours composés transmis en AR, y compris les trous. Les cotations restent des annotations du plan. Un ancien APK est masqué pour une forme enrichie, plutôt que de montrer un dessin incomplet.
- Relevé rapide facultatif : mesure plus courte et plus tolérante au bruit. Les points doivent rester réellement suivis ; les écarts demandent toujours votre accord et l'indice de cohérence n'est pas une précision garantie.
- Sur téléphone déjà calibré, une courte interruption peut conserver les ancres jusqu'à 30 secondes. Reprendre demande des ancres cohérentes et une confirmation ; déconnexion, redémarrage, délai dépassé ou changement de calibration imposent A/B/C.
- Choisissez téléphone ou XREAL dans l'APK ; le SDK indique ensuite le modèle identifié. Aucun changement automatique de fournisseur. XREAL Air 2 Ultra + Beam Pro reste à qualifier sur lunettes réelles.
- Les mêmes feuilles A/B/C réutilisables conviennent, au sol ou sur pied avec hauteur du centre renseignée. Vidéo et AR restent indépendantes ; le masque personnel ne peut pas annuler celui du PC.
- Notices FR/EN et guide AR mis à jour. Aucun changement du format projet, des licences ou des raccourcis de secours.

**Limites :** APK Android ARM64 signée développement, Android 10+ et ARCore pour le téléphone. Les nouveaux comportements nécessitent un essai sur votre appareil et votre plateau. Vérifiez un emplacement connu ; ne pas utiliser pour un repérage critique. Au-delà de 2048 points par objet, simplifiez le tracé : l'AR est masquée au lieu de tronquer la forme.

RayNeo X3 Pro garde la même priorité que XREAL. Son SDK réel est intégré à un **diagnostic local séparé**, mais les ancres de scène et l'affichage des marques au sol ne sont pas encore disponibles. Cette APK publique ne revendique donc pas de compatibilité RayNeo.

Windows est construit et testé localement. Les DMG 2027.0.9 seront ajoutés uniquement après succès du pipeline Codemagic ; en leur absence, les derniers Mac vérifiés restent 2027.0.8. Pas de signature Apple Developer ID ni notarisation. Smoke natif ARM64 et contrôle d'architecture Intel, sans prétendre à un essai natif Intel.

## English

Desktop 2027.0.9 and AR preview build 16 transmit fills, opacity, text sizes and compound contours with holes. Dimensions remain plan annotations; older companions are hidden for enriched shapes. Optional quick capture accepts more measurement noise but never invents tracking. A calibrated phone can retain anchors for up to 30 seconds after interruption; coherent anchors and explicit confirmation are required before resuming. Disconnect, restart, timeout or changed calibration geometry require A/B/C again.

Choose phone or XREAL explicitly; the SDK reports the model when available. The hideable consistency score is not guaranteed accuracy. Reusable markers, raised target heights and independent PC/personal/video masks remain. Development-signed Android ARM64 preview; physical testing is still required. XREAL glasses require hardware qualification. RayNeo is a separate local SDK diagnostic with no stage anchors or floor marks, not supported by this public APK. Mac 2027.0.9 files are only available after successful Codemagic publication; until then the verified Mac release remains 2027.0.8, unsigned and not notarised.
