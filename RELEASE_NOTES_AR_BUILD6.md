# StageMark AR 0.1.1 build 6 — bouton de relevé corrigé

**Remplacée par le [build 7](RELEASE_NOTES_AR_BUILD7.md), correctif caméra téléphone et veille.** L’empreinte ci-dessous reste celle du build 6 archivé, pas de l’APK téléchargeable actuelle.

Correctif Android du 9 septembre 2026. Le build 5 pouvait montrer une cible turquoise sans enregistrer A lorsque vous touchiez **RELEVER LE POINT A**. Un contrôle lié au cycle d’affichage empêchait le bouton de fonctionner ; ce n’était pas un problème de distance ou de taille du motif.

Le build 6 vérifie le sol directement au toucher, sans utiliser un ancien point. Si le relevé est impossible, un message en donne la raison. La visée dégagée, la reprise des points et l’acceptation explicite d’un écart limité sont conservées. Le plan, la calibration vidéo et les masques PC/personnel ne changent pas.

## Installer

[Télécharger l’APK 0.1.1 build 6](https://github.com/Mamat79/StageMark/releases/download/v2027.0.5/StageMark-AR-0.1.1-Development.apk?build=6) · [SHA-256](https://github.com/Mamat79/StageMark/releases/download/v2027.0.5/StageMark-AR-0.1.1-Development.apk.sha256?build=6) · [Guide actualisé](guides/StageMark-AR-Demarrage.md).

Ouvrez l’APK sur le téléphone pour remplacer la précédente **sans désinstallation**. Vérifiez **build 6** dans les réglages. Vous pouvez viser depuis votre hauteur normale : le motif n’a pas besoin de remplir l’écran, mais son centre doit rester identifiable sous la croix.

**167038347 octets** ; SHA-256 `32A242A6FCD01019238F3E49100A4184EE38576B9CACACFF956F1DBF1DA3BFEE`. Identité et certificat Android conservés, Android 10 minimum / ARM64, ARCore compatible ou XREAL Air 2 Ultra + Beam Pro.

**Correctif APK seulement : aucune réinstallation du Desktop guidé 2027.0.5.** Windows, DMG et notices PDF restent inchangés. [Fonctions Desktop et téléchargements](RELEASE_NOTES_GUIDED_2027.0.5.md) · [Visée et tolérance](RELEASE_NOTES_AR_BUILD5.md).

## Vérifications et limites

76 assertions dans le vrai Unity, dont l’ordre des événements du bouton et les contrôles de relevé ; compilation ARM64 et signature v2 vérifiées. Même ensemble de 160 fichiers APK, 77 bibliothèques natives tierces identiques. Tests généraux : 926 applicatifs + 26 complémentaires, un contrôle hôte facultatif ignoré.

L’essai sur téléphone du build 6 reste nécessaire : les tests logiciels ne garantissent pas une précision physique. APK de développement, AR expérimentale ; contrôler une position indépendante au mètre. Aucun effet sur le vidéoprojecteur, aucune capture/transmission caméra.

## English

**Build 6 fixes the capture button regression in build 5.** A turquoise target could be displayed while tapping CAPTURE POINT A did nothing. A frame-timing guard incorrectly rejected the input; distance from the marker was not the cause.

The floor is now checked directly when you tap. No old point is reused; a failed capture explains why. Clear aiming, individual recapture and explicit acceptance of limited calibration discrepancies are retained. Aim from normal standing height; the pattern does not need to fill the screen, but its centre must be identifiable under the cross.

Install the APK above over the existing app and check build 6. No Desktop reinstall or new Mac build is needed. Identity/signing certificate unchanged. 76 Unity assertions, full application tests, ARM64 build and APK signature passed. Physical phone/glasses testing remains necessary; experimental AR is not a certified measuring instrument.
