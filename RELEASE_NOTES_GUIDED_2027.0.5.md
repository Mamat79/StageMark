# StageMark 2027.0.5 — guidage AR et sortie vidéo de secours

**APK actuelle : build 7.** [Caméra téléphone, veille et nouvelle empreinte](RELEASE_NOTES_AR_BUILD7.md). Les notes build 4 ci-dessous décrivent la livraison guidée précédente ; son empreinte APK n’est plus celle de l’asset remplacé. Windows et notices restent inchangés.

Réédition du 9 septembre 2026. **Windows et APK actualisés, numéros visibles conservés.** Réinstallez Windows manuellement et vérifiez **0.1.1 build 4** dans StageMark AR. Les DMG Mac présents sont inchangés, en attente d’une reconstruction Codemagic.

## Ce qui change

- **Vidéo et AR indépendantes** : vidéo seule, AR seule, les deux ou aucun affichage. Dans Connexion → Réalité augmentée, **AFFICHER AR / MASQUER AR** concernent les compagnons, jamais le vidéoprojecteur. La session AR démarre masquée.
- **MASQUER POUR MOI** dans l’APK : chacun masque ses repères sans agir sur les autres. Réafficher localement ne peut pas annuler le masquage du PC. Caméra, connexion et calibration restent actives tant que le suivi est valide.
- **Guidage matériel → placement → connexion → validation**. Sur le téléphone : A, B, C, puis **VALIDER ET AFFICHER LES REPÈRES** ; le calcul est automatique. Les erreurs et distances mesurées/attendues sont visibles ; chaque point peut être repris séparément.
- **Marqueurs A/B/C réutilisables** pour toutes les scènes. Coordonnées dans le logiciel, fiche facultative de placement propre au projet, aides sur le plan et en projection activables indépendamment.
- **Ctrl+Maj+F12** ferme la sortie vidéo, son rideau noir et Spout, sans quitter le projet ni arrêter l’AR. Échap fonctionne dans la fenêtre projetée ; **FERMER SORTIE** reste accessible en haut. BLACKOUT garde au contraire l’écran noir ouvert. Un avertissement protège l’ouverture sur l’écran de travail.

## Télécharger

- [Windows 2027.0.5](https://github.com/Mamat79/StageMark/releases/download/v2027.0.5/StageMark-2027.0.5-Setup.exe?edition=guided-20260909) · [SHA-256](https://github.com/Mamat79/StageMark/releases/download/v2027.0.5/StageMark-2027.0.5-Setup.exe.sha256?edition=guided-20260909)
- [StageMark AR 0.1.1 build 4](https://github.com/Mamat79/StageMark/releases/download/v2027.0.5/StageMark-AR-0.1.1-Development.apk?build=4) · [SHA-256](https://github.com/Mamat79/StageMark/releases/download/v2027.0.5/StageMark-AR-0.1.1-Development.apk.sha256?build=4)
- [Premier essai guidé](guides/StageMark-AR-Demarrage.md) · [Notice FR](guides/StageMark-Notice-FR.pdf) · [User manual EN](guides/StageMark-Notice-EN.pdf)
- [Manifeste complet SHA-256](https://github.com/Mamat79/StageMark/releases/download/v2027.0.5/SHA256SUMS-2027.0.5)

Windows : **118771430 octets**, SHA-256 `5E7BB2E45CE0B41F49CDAC141D999313425A4472A10F5A0C0AF817B4D1767E11`.

APK : **167011219 octets**, SHA-256 `BD42126CEF07AF698D7626C14D821F69573C4D3356185BEFEBD6935588FB5643`. Android 10+, ARM64 ; téléphone compatible ARCore (dont Galaxy A54 5G), ou XREAL Air 2 Ultra + Beam Pro. Même identité et certificat de développement : mise à jour par-dessus la précédente sans désinstallation.

## Vérifications et limites

926 tests applicatifs + 25 complémentaires, 37 assertions C# Unity, build Windows/APK et signature Android vérifiés. Trois scénarios natifs de fermeture vidéo testés en fenêtres cachées, 12 dispositions FR/EN clair/sombre et notices 14 pages/langue contrôlées.

**L’AR reste une préversion technique.** Précision, dérive, reprise et nouvelle procédure doivent être testées sur appareil réel ; rendu de primitives, sans qualification complète de tous les symboles complexes. Les motifs XREAL restent à qualifier. Aucun usage de positionnement critique. La caméra n’est ni enregistrée ni envoyée. Les marques AR sont personnelles ; pour des marques réellement visibles au sol, il faut un ou plusieurs vidéoprojecteurs.

Fermer la sortie peut montrer le bureau sur le vidéoprojecteur ; cela n’éteint pas son alimentation. Formats, millimètres, licences et données utilisateur conservés. Les fichiers remplacés ont été archivés et vérifiés ; anciens APK 0.1.0 et DMG Mac inchangés. Windows non signé, APK signé pour le développement, Mac existants non notarisés. Les changements décrits ici ne sont pas encore présents dans les DMG disponibles.

## English

This reissue adds **independent video and AR visibility**, plus **hide for me** in APK **0.1.1 build 4**. PC hide overrides personal show. AR starts hidden; hiding retains camera, connection and valid calibration. A four-step PC guide explains equipment, measured marker placement, pairing and automatic A/B/C validation. Errors and measured/expected distances are visible; individual points can be recaptured. Reusable A/B/C sheets and optional per-project placement sheets replace repeated project-specific printing.

**Ctrl+Shift+F12**, Escape in the output window, or **CLOSE OUTPUT** closes video, its black curtain and Spout without quitting the editor or stopping AR. BLACKOUT deliberately keeps a black window open. Covering the working display requires confirmation. This closes video windows, not the projector’s electrical power, and can expose the desktop.

Manually reinstall Windows and check **build 4** in the companion: visible versions are retained. Identity/signing certificate and existing licences/projects remain compatible. Software tests and hidden native checks passed; physical tracking, precision and the new procedure still require device testing. **Existing Mac DMGs are unchanged**, pending Codemagic. AR is a debug-signed primitive-rendering prototype, not suitable for critical positioning.
