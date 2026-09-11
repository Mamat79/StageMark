# StageMark 2027.0.9 — livraison macOS / macOS delivery

Les versions Apple Silicon et Intel sont maintenant disponibles dans la Release 2027.0.9. Les quatre fichiers DMG/SHA-256 ont été téléchargés depuis GitHub et leurs empreintes vérifiées. Ce complément remplace l'attente Mac décrite dans les notes initiales, conservées à l'identique.

Codemagic a réalisé les tests d'exécution natifs sur Apple Silicon : démarrage, commandes de sécurité, ouverture d'un projet StageFlow synthétique inchangé et exports PDF/PNG. Le paquet Intel a été monté et son architecture contrôlée, sans lancement natif Intel. La correction de relance concerne uniquement le nettoyage des volumes de test, sans modification du code livré ni de la version produit.

Les DMG ne sont pas signés Apple Developer ID ni notariés. Ne désactivez pas les protections macOS. La recette avec un vidéoprojecteur, un téléphone ou des lunettes reste distincte de ces contrôles logiciels. Windows 2027.0.9 et l'APK 0.1.1 build 16 déjà publiés sont inchangés.

## English

Apple Silicon and Intel installers are now available in release 2027.0.9. All four DMG/checksum assets were downloaded from GitHub and verified. This addendum supersedes the Mac-pending status in the unchanged original release notes.

Codemagic performed native Apple Silicon runtime smoke tests: startup, safety controls, opening an unchanged synthetic StageFlow project, and PDF/PNG exports. The Intel package was mounted and its architecture verified, without a native Intel launch. The retry correction only changes test-volume cleanup, not the shipped application or product version.

No Apple Developer ID signing or notarisation. Do not disable macOS protections. Projector, phone and glasses hardware acceptance remains separate. Previously published Windows 2027.0.9 and AR APK 0.1.1 build 16 are unchanged.
