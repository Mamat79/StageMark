# StageMark 2027.0.10 — traits et plans réutilisables

## Français

- Épaisseur des nouveaux traits mémorisée par projet, dans Dessin → Actions & cotations. Les objets existants et les cotations conservent leur style.
- Import/export `.stagemarkplans` : sélection de plans, ajout dans un autre projet sans remplacer ses plans, scène facultative. Calques, styles, géométrie, groupes et cotations sont conservés avec des identifiants distincts.
- Remplacement de scène volontaire et séparé : BLACKOUT vidéo et arrêt AR avant application. Refaire la calibration et les hauteurs des cibles ; aucune calibration d'un autre lieu n'est importée.
- Association des groupes StageFlow aux plans : créer les plans manquants ou relier les plans existants. Plans supplémentaires libres conservés.
- Suivi LIVE bidirectionnel facultatif : commence désactivé, reprend le groupe du réseau à l'activation, conserve les liens pendant le travail indépendant. Un plan libre met le suivi en pause. Ne démarre aucune sortie ni aucun moteur audio.

**Compatibilité réseau :** le suivi nécessite des versions StageFlow et StageMon prenant en charge `group-selection-v1`. Leurs mises à jour sont préparées séparément, mais ne sont pas publiées ou installées par cette livraison StageMark. Les versions précédentes restent utilisables sans suivi des groupes. Les tests croisés logiciels ne remplacent pas une répétition sur deux postes réels.

Windows x64 : tests complets et quatre contrôles du paquet réussis (démarrage, Spout, exports PDF/PNG, fermeture de secours). Notices FR/EN actualisées, 16 pages chacune. L'installeur est non signé. Projets, licences et raccourci permanent StageMark v2027 conservés.

macOS Intel/Apple Silicon : construction via Codemagic après publication Windows ; seuls les fichiers effectivement présents dans cette Release sont disponibles. En attendant, les Mac 2027.0.9 restent accessibles. Pas de signature Apple Developer ID ni de notarisation. Le runner Apple Silicon exécute le paquet ARM64 ; Intel reçoit un contrôle d'architecture, pas un essai natif Intel.

L'APK publique reste **0.1.1 build 16**, disponible dans la Release 2027.0.9. La candidate APK 17 avec caméra dégagée reste distincte et locale. Aucune nouvelle qualification physique AR ou lunettes n'est déduite de cette livraison Desktop.

## English

Default width for new strokes, saved per project. Portable `.stagemarkplans` files append selected plans to another project with fresh identities, keeping geometry, styles, layers, groups and dimensions. Stage replacement is optional and explicitly stops AR and blacks out video; recalibrate afterwards. Source venue calibration is never imported.

Link musical groups to existing plans or create missing plans. Optional bidirectional LIVE following starts off, resumes from the network group and can be paused for independent work. Unlinked plans pause following. It never starts output or audio.

**Requires compatible StageFlow/StageMon versions supporting `group-selection-v1`. Those companion updates are prepared separately and are not installed or publicly released by this StageMark delivery.** Older versions remain usable without group following. Automated cross-application checks do not replace rehearsal on two real computers.

Windows x64 package checks passed. Updated 16-page FR/EN manuals included. Unsigned installer. Mac DMGs are built through Codemagic; only actual assets in this release are available. Until then use Mac 2027.0.9. No Developer ID signature or notarisation; ARM64 runtime smoke and Intel architecture-only checks. Public Android companion stays build 16 in release 2027.0.9; local build 17 is separate. No new AR or glasses hardware qualification.
