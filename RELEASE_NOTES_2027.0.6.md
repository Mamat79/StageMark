# StageMark 2027.0.6 — préparer, configurer, exploiter

## Français

- **Connexion StageFlow** : StageFlow LIVE et télécommande. Les projets autonomes `.stagemark` et locaux `.stageflow` restent disponibles sans réseau.
- **Sorties & installation**, à côté : vidéoprojecteur/Spout, réalité augmentée, matériel, implantation et calibration. Les réglages se ferment pour retrouver le travail en cours.
- Navigation de travail allégée : Scène, Dessin, Patch StageFlow, Conduite. Plus de longue colonne de réglages de projection mêlée aux connexions.
- Conduite concentrée sur plans, cues, AFFICHER, BLACKOUT et visibilité AR indépendante. Prévol et édition détaillée des cues restent accessibles à la demande.
- **Démarrer l’AR** ouvre la session et autorise les repères en une action. L’appareil doit toujours s’associer et se calibrer. Le guide pas à pas et l’impression des marqueurs sont facultatifs et accessibles séparément.
- **APK 0.1.1 build 12** : interface tactile défilante avec actions accessibles, correction de l’entrée native des poses caméra, étiquettes explicites uniquement (plus de nom interne Cross ajouté), indications du nouveau menu Desktop. Signature de développement compatible conservée.
- Notices FR/EN actualisées. Les commandes vidéo et AR restent indépendantes ; ouvrir un menu n’allume aucune sortie. Licences, géométrie, formats et données utilisateur inchangés.

**Sécurité vidéo :** démarrage en noir, AFFICHER explicite. **Ctrl+Maj+F12** ferme la vidéo et son écran noir sans quitter le projet ni arrêter l’AR. Fermer une sortie peut montrer le bureau ; cela n’éteint pas électriquement le projecteur.

**Limites :** l’AR reste une préversion. Une croix et ses changements de couleur ont été observés sur A54, mais précision, dérive et relocalisation ne sont pas qualifiées. XREAL et les autres lunettes ne sont pas déclarés validés physiquement. Un Wi-Fi d’hôtel peut isoler les appareils ; le relais USB utilisé en diagnostic n’est pas une fonction universelle sans configuration. Les paquets Windows sont sans certificat éditeur. Les nouveaux DMG macOS sont attendus de Codemagic ; conserver les téléchargements Mac 2027.0.5 jusqu’à leur validation.

[Guide des parcours](https://github.com/Mamat79/StageMark/blob/main/guides/StageMark-Parcours-2027.0.6.md) · [Démarrage AR](https://github.com/Mamat79/StageMark/blob/main/guides/StageMark-AR-Demarrage.md) · [Empreintes SHA-256](https://github.com/Mamat79/StageMark/releases/download/v2027.0.6/SHA256SUMS-2027.0.6)

## English

StageFlow connection now contains LIVE and remote networking only. The adjacent **Outputs & setup** centre groups projector/Spout, AR, equipment, placement and calibration. The working sidebar keeps Scene, Drawing, StageFlow Patch and Live. Closing settings returns to the current workspace.

Live mode focuses on plans, cues, SHOW, BLACKOUT and independent AR visibility. Detailed cue editing and preflight remain available on demand. **Start AR** creates the session and authorises marks in one action; pairing and calibration remain required. The guided route and reusable marker printing are optional.

**AR 0.1.1 build 12** includes the scrollable touch client, native camera-pose input fix, explicit labels only and updated Desktop instructions. Existing development signing identity is preserved. Desktop formats, licensing and metric geometry are unchanged. FR/EN manuals are updated.

Video still opens black and requires explicit SHOW. **Ctrl+Shift+F12** closes video/black curtain/Spout without closing the project or stopping AR; the desktop may then appear on the projector. This is not a physical power command.

AR remains a development preview. A cross and live colour changes were observed on A54; physical accuracy, drift, relocalisation and XREAL hardware qualification are incomplete. Hotel networks may isolate devices; the diagnostic USB relay is not an automatic production feature. Windows packages are unsigned. New Mac DMGs are pending Codemagic validation; retain existing 2027.0.5 links until then. Developer ID signing and notarisation are not introduced.
