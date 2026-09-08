# StageMark AR 0.1.1 — compagnon Android expérimental

## Réédition du 9 septembre 2026 — build 3

Cette préversion accompagne la même application StageMark Desktop **2027.0.5**. L'installeur Windows et les notices FR/EN sont actualisés ; les DMG macOS restent pour le moment ceux de l'édition précédente, avant reconstruction Codemagic. Aucun changement de licences, projets, projection, télécommande ou BLACKOUT.

- Nouvelle icône StageMark avec grand **AR**, adaptée aux lanceurs Android classiques, ronds et adaptatifs.
- Accueil agrandi sur les écrans haute résolution, avec défilement et boutons plus faciles à toucher.
- Choix explicite **CAMÉRA DU TÉLÉPHONE** (ARCore) ou **LUNETTES XREAL**, sans activation automatique de caméra. Relancer l'APK pour changer de mode.
- Téléphones compatibles ARCore, dont le Galaxy A54 5G : autorisation caméra, vérification de disponibilité et installation Google AR explicite si nécessaire.
- Détection du sol horizontal, visée centrale et relevé manuel des centres mesurés A/B/C, puis validation de calibration à l'échelle réelle.
- Ancre locale ; masquage et recalibration après perte de suivi/réseau, pause ou changement de géométrie. Un changement de plan dans la même scène conserve la calibration.
- Images caméra ni enregistrées ni transférées par StageMark. Connexion au PC toujours locale et volontaire, par code.

L'APK nécessite Android 10 minimum et ARM64 ; le mode caméra nécessite aussi un appareil de la [liste ARCore Google](https://developers.google.com/ar/devices). Le mode lunettes conserve **XREAL Air 2 Ultra + Beam Pro**. La première installation des services AR Google peut nécessiter Internet. Les repères sont une vue personnelle, jamais de vraies marques lumineuses sur le sol. [Premier essai guidé](guides/StageMark-AR-Demarrage.md).

**Préversion de développement, non validée sur matériel réel.** Tests logiciels et compilation réussis, mais caméra, précision, dérive, reprise après pause et suivi doivent encore être testés sur l'A54 et les autres appareils. Le rendu reste un prototype de primitives, sans qualification complète des symboles complexes. Les images XREAL restent signalées comme peu riches par le SDK. Une calibration mathématiquement cohérente n'est pas une précision certifiée ; ne pas utiliser pour du positionnement critique.

Identité et certificat de signature conservés pour permettre la mise à jour sans désinstallation. Version visible **0.1.1**, code Android **3** : vérifier **build 3** dans l'accueil. L'asset 0.1.1 précédent est remplacé après archivage ; l'ancien 0.1.0 reste disponible. Windows conserve aussi son numéro 2027.0.5 et demande une réinstallation manuelle pour obtenir cette réédition.

## English

The 9 September reissue adds **ARCore phone camera support** to the same **0.1.1 build 3** companion, alongside XREAL. Select the mode explicitly, allow camera access, scan a horizontal floor, aim and capture the measured A/B/C centres, then validate calibration. Relaunch the APK to switch modes. Tracking/network loss, pause or changed stage geometry hides marks and requires recalibration. Switching plans within unchanged geometry preserves calibration.

Requires Android 10+, ARM64 and, for phone mode, [ARCore device support](https://developers.google.com/ar/devices), including Galaxy A54 5G. Initial Google AR Services installation may need Internet. StageMark does not record or upload camera images. XREAL Air 2 Ultra + Beam Pro remain supported in the separate glasses mode. This is **debug-signed and not hardware-validated**: software tests/build passed, but camera operation, drift, accuracy, pause recovery and marker robustness require real-device testing. Rendering remains a primitive prototype, not full complex-symbol parity; not suitable for critical positioning. Identity and signing certificate are unchanged for in-place updates.

Windows 2027.0.5 and FR/EN manuals are refreshed. The available Mac DMGs are unchanged, pending Codemagic rebuild. Since visible version numbers are retained, manually download/reinstall the new Desktop package and check **build 3** in the companion. Existing license and projection behaviour are unchanged.

## Download / Téléchargement

- [StageMark-AR-0.1.1-Development.apk](https://github.com/Mamat79/StageMark/releases/download/v2027.0.5/StageMark-AR-0.1.1-Development.apk?build=3) — **203836567 bytes / octets**.
- [SHA-256](https://github.com/Mamat79/StageMark/releases/download/v2027.0.5/StageMark-AR-0.1.1-Development.apk.sha256?build=3) : `9CA2744B91D02E2F299C5C05834E1E64DA712AE66F82F61E3328BAA3907F02DA`.

Read-only LAN companion: no project editing, no projection commands, no BLACKOUT removal. Compagnon LAN en lecture seule : aucune édition du projet, commande de projection ou levée de BLACKOUT.
