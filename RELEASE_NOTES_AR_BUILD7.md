# StageMark AR 0.1.1 build 7 — caméra téléphone et veille

Correctif Android du 9 septembre 2026. Une calibration pouvait être acceptée, avec AR autorisée et suivi actif, sans marques visibles : les mouvements du téléphone n’étaient pas reliés correctement à la caméra virtuelle. Le build 7 ajoute cette liaison ARCore tout en conservant le mode lunettes XREAL.

La **veille automatique est suspendue pendant l’AR téléphone au premier plan**. Quitter l’AR ou passer en arrière-plan rétablit le comportement précédent. Le verrouillage manuel reste possible ; après verrouillage, interruption ou perte du suivi, il faut encore refaire A/B/C. Ce n’est pas une restauration automatique de calibration.

Le relevé tactile corrigé, les motifs réutilisables, la tolérance après acceptation explicite et les deux masques PC/personnel sont conservés. L’échelle du plan et la calibration du vidéoprojecteur ne changent pas.

## Installation

[Télécharger l’APK build 7](https://github.com/Mamat79/StageMark/releases/download/v2027.0.5/StageMark-AR-0.1.1-Development.apk?build=7) · [SHA-256](https://github.com/Mamat79/StageMark/releases/download/v2027.0.5/StageMark-AR-0.1.1-Development.apk.sha256?build=7) · [Guide](guides/StageMark-AR-Demarrage.md).

Ouvrez l’APK sur le téléphone pour remplacer la précédente **sans désinstallation**. Vérifiez **build 7** dans les réglages. Relevez A/B/C, choisissez AFFICHER AR sur le PC puis contrôlez une croix à une position connue. Un écart accepté reste signalé comme approximatif.

**167051783 octets**, SHA-256 **`BD832C4A4CDD28434818DB45A368CC2828507C77736D3F47EC37E1B1E4501655`**. Version visible 0.1.1, code Android 7, même identité et certificat de développement. Android 10+, ARM64, téléphone compatible ARCore ou XREAL Air 2 Ultra + Beam Pro.

**APK seule : aucune réinstallation de StageMark sur le PC.** Windows, macOS et notices PDF embarquées restent inchangés ; le guide en ligne est actualisé. [Téléchargements Desktop](RELEASE_NOTES_GUIDED_2027.0.5.md).

## Vérifications et limites

91 assertions Unity, dont un véritable périphérique simulé dans Input System et le déplacement du TrackedPoseDriver, compatibilité des liaisons lunettes et restauration de la politique de veille. 926 tests applicatifs + 27 complémentaires, un test hôte facultatif ignoré ; compilation ARM64 et signature v2 vérifiées. Les 160 entrées APK sont conservées ; aucune dépendance ARCore/XREAL retirée.

La vérification physique du nouveau build sur A54 et lunettes reste nécessaire : les tests logiciels ne garantissent pas la précision ou la stabilité sur le terrain. AR expérimentale, signature de développement. Rendu actuel limité aux croix et primitives simples, pas encore à tous les symboles/Béziers Desktop. Aucun enregistrement/transfert des images caméra, aucune commande du vidéoprojecteur depuis l’AR.

## English

**Build 7 fixes the handheld camera pose bindings.** Calibration could succeed and AR be enabled while no marks appeared because the virtual camera did not follow the phone. ARCore handheld position/rotation bindings are now present; headset bindings remain available.

Automatic screen sleep is prevented only while phone AR is active in the foreground. Pausing, losing focus or exiting restores the previous policy. Manual lock is still possible; interruption or tracking loss still requires A/B/C recalibration. No persistent relocalization is claimed.

Install the APK above over the previous app and check build 7. Capture A/B/C, enable SHOW AR on the PC, and check a cross at a measured position. Capture-on-tap, explicit discrepancy acceptance and independent PC/personal masks are retained. No Desktop or Mac reinstall is needed.

91 Unity assertions, 926 application tests and 27 supplementary tests passed; ARM64 build and APK signature verified. Same Android identity/signing certificate. Actual phone/glasses rendering and sleep behaviour still need device testing. Experimental AR is not a certified measuring instrument; complex Desktop symbols and Bezier rendering remain outside this POC.
