# StageMark 2027.1.5 — qualification Windows / Windows acceptance

## Français

Windows : source `85e7a093ba4334a9e07e667eaf8128c6374d62f1`, base applicative `e0023c2623f30d0757676db75949c8cce653d121`. macOS Apple Silicon existant : source distincte `356a212e9bdba660f7aee113f9ae96442ea17cfe`, deux fichiers ARM conservés sans modification. Aucun Mac Intel 1.5 n'est qualifié : Intel 1.3 reste disponible dans sa release versionnée, pour les échanges V1 uniquement.

### Paquet et contrôles Windows

- Installeur x64 autonome `StageMark-2027.1.5-Setup.exe`, 121861836 octets, SHA-256 `e8769069636acf66692b9da71d436d9b2d8fb919884e06da30dc1ed74dc0230a`. Version Windows 2027.1.5.0 ; installeur non signé Authenticode.
- Les 117 fichiers extraits du véritable NSIS sont conformes au paquet construit. Aucun fichier `.map` ni map intégrée ; 93 maps retirées, 1055 autres membres ASAR inchangés hors métadonnées version/build. Les 87 fichiers exécutés JS/CJS/MJS/HTML/CSS sont identiques à la base applicative contrôlée. Les quatre PDF, les trois clés publiques de licence, Canvas Windows AMD64 1.0.6 et les notices Electron/Chromium/Spout sont présents et contrôlés ; ceci ne constitue pas un audit exhaustif des licences tierces.
- Les 49 tests Node et trois tests Electron ciblés du propriétaire des sources sont des résultats distincts, non rejoués par l'atelier.
- Vraie interface avec profil séparé : scène métrique, rectangle de 2500×1500 mm avec coordonnées entières, enregistrement natif `.stagemark`, fermeture et réouverture du dessin. Clic BLACKOUT observé, sortie restée fermée. Les deux instances quittent normalement dès la première demande.
- Recette officielle d'installation locale exécutée : installateur standard et quatre contrôles sur l'application installée, tous avec code zéro. Ils couvrent le montage React et les commandes/ressources, l'ouverture et la fermeture d'un émetteur Spout natif, les exports PDF/PNG, et trois scénarios natifs invisibles de fermeture d'urgence (clavier, renderer défaillant, blackout). Les exports synthétiques ont été conservés.
- Installation personnelle 2027.1.3→2027.1.5 dans le même emplacement et avec le même identifiant, après deux sauvegardes sur disques distincts et une restauration isolée : 378 fichiers /495370914 octets dans chaque copie, registre/droits et 1332 dates contrôlés. Les 117 fichiers installés sont exacts. Un seul raccourci Bureau StageMark v2027, cible et icône contrôlées.
- Les 250 fichiers personnels existants sont identiques juste après installation ; deux sauvegardes de raccourcis sont ajoutées. Le démarrage normal de l'application installée, sans profil de test, affiche l'interface française sombre avec sortie fermée, puis quitte normalement. Les réglages, le projet personnel et le profil Beta sont conservés. Seule la date lastSeenAtUtc évolue dans la licence ; les autres changements sont des caches et journaux. Le journal LocalStorage antérieur est intégralement conservé avec un ajout de 49 octets limité à METAACCESS:file://, sans modification de clé utilisateur.

Limites : aucune recette complète langues/thèmes/DPI, de précision géométrique ou de matériel. Les contrôles Spout et sorties invisibles ne qualifient pas un consommateur Spout, un vidéoprojecteur ou une calibration physique. Ni téléphone/AR, audio, MIDI, réseau entre machines ni AutoCAD n'ont été validés matériellement. Les PDF approuvés sont contrôlés octet pour octet ; pas de nouvelle recette visuelle de leur mise en page. La restauration est exercée en dossier isolé, sans réinstaller une ancienne version sur le profil personnel.

V1 reste le parcours par défaut. V2 exige une nouvelle copie locale explicite, sans migration automatique en place ; aucun échange V2 réseau/LIVE/AutoCAD n'est annoncé dans cette tranche. Conservez les originaux V1 pour les anciennes applications.

### Mac Apple Silicon — qualification antérieure conservée

macOS 12 minimum déclaré, sans matrice d'anciens OS. Le producteur rapporte 1358 tests réussis/27 ignorés, un contrôle ARM non visuel depuis le vrai DMG monté, et les exports PDF/PNG. Le contrôle Canvas sous Node n'est pas un contrôle Canvas sous Electron. Métadonnées de signature ad hoc observées ; pas de Developer ID/notarisation, ni vérification indépendante complète codesign. Pas de recette visuelle/personnelle Mac, de matériel ou de montage restant après détachement établi indépendamment. Aucun résultat Mac n'est compté comme nouveau test Windows.

## English

Windows 1.5 uses source 85e7a093ba4334a9e07e667eaf8128c6374d62f1 and application base e0023c2623f30d0757676db75949c8cce653d121. The existing Apple Silicon 1.5 package uses separate source 356a212e9bdba660f7aee113f9ae96442ea17cfe and both Mac assets remain unchanged. Intel 1.5 is not qualified; the previous Intel 1.3 download remains versioned and V1-only.

The unsigned 121861836-byte Windows Setup has SHA-256 e8769069636acf66692b9da71d436d9b2d8fb919884e06da30dc1ed74dc0230a. All 117 extracted and installed files match; source maps are absent, runtime code and three public licence keys are retained. The source owner's 49 Node and 3 Electron checks were not repeated here.

Actual native acceptance created a metric rectangle, saved and reopened a .stagemark file, clicked BLACKOUT while keeping output closed, and closed normally. The official installed recipe passed Setup and four installed smoke processes (React/assets/controls, native Spout sender, PDF/PNG exports, three invisible native emergency-close scenarios). These are nonvisual smoke checks, not hardware projection acceptance.

The standard personal upgrade from 1.3 to 1.5 preserved all 250 existing personal files before normal startup, with two shortcut backups added. Three verified backup/restore copies each contain 378 files/495370914 bytes. A real normal installed start and close succeeded without a QA profile; settings, the personal project and Beta profile are retained. Only lastSeenAtUtc changes within the licence state; other changes are caches/logs and one origin-access metadata append, without a user-value update. One correctly targeted StageMark v2027 shortcut was verified.

No complete language/theme/DPI, physical projector/calibration, Spout consumer, LAN, audio, MIDI, phone or AR acceptance is claimed. Approved PDFs were byte-checked, not visually re-reviewed. V1 stays default; V2 requires an explicit local copy and does not support V2 LAN/LIVE/AutoCAD exchanges in this tranche.

The unchanged ARM Mac package declares macOS 12 minimum. Its producer reported 1358 passed/27 skipped tests and nonvisual mounted-DMG checks, separate from Windows. No native Intel 1.5, Developer ID/notarization, full independent codesign/clean-unmount or personal Mac-upgrade acceptance is claimed.
