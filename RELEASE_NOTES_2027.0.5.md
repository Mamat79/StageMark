# StageMark 2027.0.5

## Réédition Windows et Android du 9 septembre 2026

**StageMark AR 0.1.1 build 3** ajoute la vue caméra pour téléphones ARCore, dont le Galaxy A54 5G, avec relevé manuel A/B/C et calibration à l'échelle réelle. Le mode XREAL reste distinct et disponible. Windows 2027.0.5 et les notices FR/EN sont actualisés ; licences, fichiers, projection et BLACKOUT sont inchangés. Les DMG Mac existants sont conservés dans l'attente du build Codemagic, sans prétendre qu'ils sont reconstruits.

La version visible étant conservée, téléchargez/réinstallez Windows manuellement et vérifiez **build 3** dans l'APK. Caméra et précision restent **à tester physiquement** ; l'AR demeure une préversion de développement. [Détails, SHA-256 et limites](RELEASE_NOTES_AR_0.1.1.md) · [Démarrage téléphone](guides/StageMark-AR-Demarrage.md).

**English:** the 9 September reissue adds ARCore phone-camera mode in **AR 0.1.1 build 3**, preserving XREAL. Windows and FR/EN manuals are refreshed without changing the version number. Manually reinstall to obtain this edition. Existing Mac DMGs remain unchanged pending Codemagic. Physical camera/tracking accuracy is unverified; the companion remains a development preview. See the [bilingual companion notes](RELEASE_NOTES_AR_0.1.1.md).

## Édition initiale / Initial edition

Cette version clarifie le matériel nécessaire : aucun projecteur pour concevoir, un ou plusieurs vidéoprojecteurs pour rendre les marques visibles au sol, et lunettes XREAL optionnelles pour une vue personnelle.

Elle ajoute la préversion technique **StageMark AR 0.1.0** pour XREAL Air 2 Ultra + Beam Pro. L’APK Android reçoit le plan actif en lecture seule sur le réseau local et se calibre avec les marqueurs A/B/C. Il ne peut ni modifier le projet, ni afficher la projection, ni retirer le BLACKOUT.

L’APK est signé avec une clé de développement. Sa construction, son identité Android et son empreinte ont été vérifiées ; précision, dérive et relocalisation physiques restent à mesurer avant tout usage critique.

La Release réunit Windows x64, macOS Intel, macOS Apple Silicon, leurs fichiers SHA-256 et les notices française et anglaise. StageMark reste autonome, hors ligne en exploitation, avec projets `.stagemark`, StageFlow optionnel, contrôleur local et licences existantes préservés.

## English

This release clarifies the required hardware: no projector for design work, one or more projectors to make floor marks visible, and optional XREAL glasses for a private wearer-only overlay.

It adds the **StageMark AR 0.1.0** technical preview for XREAL Air 2 Ultra + Beam Pro. The Android APK receives the active plan read-only over the local network and calibrates from A/B/C markers. It cannot edit the project, start projection or remove BLACKOUT.

The APK is debug-signed. Its build, Android identity and checksum were verified, while physical accuracy, drift and relocalisation still require real hardware testing.
