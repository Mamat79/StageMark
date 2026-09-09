# StageMark AR 0.1.1 build 5 — viser clairement, accepter un écart

**Remplacée par le [build 6](RELEASE_NOTES_AR_BUILD6.md), qui corrige le bouton de relevé.** Les fonctions ci-dessous sont conservées, mais l’empreinte build 5 n’est plus celle de l’APK téléchargeable.

Correctif Android du 9 septembre 2026. **Seule l’APK est à remplacer** si vous avez déjà StageMark Desktop 2027.0.5 avec le guidage AR. Le numéro visible 0.1.1 est conservé ; vérifiez **build 5** dans les réglages. Windows et les DMG ne sont pas remplacés par ce correctif.

## Ce qui change

- La croix est centrée dans la zone caméra dégagée, au-dessus des commandes. Visez le **centre du motif noir/blanc**, pas le bord de la feuille. Turquoise signifie sol détecté, pas reconnaissance automatique du marqueur.
- L’application distingue téléphone suivi et sol détecté sous la cible. Depuis les réglages, il faut revenir à la caméra avant de relever un point.
- Un écart limité n’impose plus de tout recommencer : après A/B/C et validation, choisissez **ACCEPTER L’ÉCART ET AFFICHER L’AR**, ou replacez les feuilles et refaites les relevés. **AR APPROXIMATIVE** reste affiché si vous acceptez.
- Les points incohérents restent bloquants : triangle inversé/aplati, sol de hauteur différente, valeurs invalides, résidu maximal > 50 cm ou différence de distance > 15 %. Ces limites ne constituent pas une précision garantie.
- Le plan n’est pas redimensionné ; la calibration du vidéoprojecteur reste inchangée. Une interruption ou nouvelle mesure retire l’accord précédent. Le masquage du PC reste prioritaire sur l’affichage personnel.

## Installation

StageMark Desktop : [Windows 2027.0.5 guidé](https://github.com/Mamat79/StageMark/releases/download/v2027.0.5/StageMark-2027.0.5-Setup.exe?edition=guided-20260909) · [ses fonctions et notices FR/EN](RELEASE_NOTES_GUIDED_2027.0.5.md). Ce paquet Windows ne change pas dans la présente mise à jour Android.

[Télécharger StageMark AR 0.1.1 build 5](https://github.com/Mamat79/StageMark/releases/download/v2027.0.5/StageMark-AR-0.1.1-Development.apk?build=5) · [SHA-256](https://github.com/Mamat79/StageMark/releases/download/v2027.0.5/StageMark-AR-0.1.1-Development.apk.sha256?build=5) · [Guide de démarrage actualisé](guides/StageMark-AR-Demarrage.md).

Ouvrez cette APK sur le téléphone pour mettre à jour l’application existante, sans désinstallation préalable. Même identité et certificat Android. **203920178 octets**, SHA-256 `EE9F15567CC411CC5E6EF29671B5EB0C8EF3F41BA9F23522E4F01E53B1499F96`.

Android 10 minimum, ARM64 ; téléphone compatible ARCore ou XREAL Air 2 Ultra + Beam Pro. Les feuilles A/B/C déjà imprimées restent utilisables. Les notices PDF Desktop précédentes restent disponibles ; le guide en ligne décrit ce nouveau choix de tolérance.

## Vérifications et limites

926 tests applicatifs et 26 complémentaires, 65 assertions C# Unity, compilation ARM64 et signature APK v2 vérifiées. Même ensemble de 160 entrées APK ; 77 bibliothèques natives tierces inchangées. Les sauvegardes des anciens assets sont conservées ; seuls l’APK 0.1.1, son SHA et le manifeste sont remplacés. Windows, DMG, notices PDF et ancien APK 0.1.0 inchangés.

Le logiciel reste une préversion expérimentale signée pour le développement. La disposition est contrôlée mathématiquement en portrait/paysage ; le rendu final, la précision et la dérive doivent encore être testés sur téléphone/lunettes. Même avec un faible écart calculé, vérifiez une position indépendante au mètre. Ne pas utiliser l’AR comme instrument de mesure ou pour un positionnement critique. Aucun enregistrement ou transfert de caméra.

## English

**Android-only update; existing guided Desktop 2027.0.5 does not need reinstalling.** Install the APK above and check **0.1.1 build 5** in settings. The reticle moves into the unobscured camera area. Aim at the centre of the black/white pattern, not the paper edge. Turquoise means a floor hit, not automatic marker recognition. Capturing from settings with a hidden target is disabled.

Small discrepancies can now be explicitly accepted instead of forcing another calibration. The **approximate AR** warning remains visible. Reposition and recapture whenever needed. Missing/invalid/inverted/flattened references, different floor heights, maximum residual over 50 cm or distance mismatch over 15% remain blocked. These are experimental consistency limits, not an accuracy guarantee. The plan is never rescaled; projector calibration is untouched. New observations, tracking/network loss or interruption revoke prior consent. PC hide still overrides personal visibility.

Software tests/build/signature passed; actual phone/glasses layout and positioning still require device testing. Existing Windows, Mac DMGs and desktop PDF manuals are unchanged; this online guide documents the Android correction. No new Mac build is claimed.
