# StageMark 2027.0.7 — atelier de dessin

La version d’essai approuvée devient la version stable. Elle remplace la précédente comme téléchargement recommandé ; les anciennes Releases restent disponibles pour récupération.

- Palette par familles, bibliothèque personnelle et 14 silhouettes d’instruments génériques aux dimensions modifiables.
- Rectangle et ellipse au glisser ; Maj pour carré/cercle. Outil Points pour sélectionner et déplacer plusieurs sommets d’un tracé libre. Conversion explicite et annulable des primitives.
- Cotations fines, sélectionnables, déplaçables, éditables et supprimables ; poignées d’extrémités et de décalage.
- Fond et contour indépendants ; union, soustraction et intersection avec courbes et trous.
- Panneaux repliables/détachables et rangement explicite. En-tête compact, connexions et sorties identifiables, Conduite rééquilibrée.
- Correction de la disposition lors du détachement des panneaux et du dialogue de fermeture ; fermeture de secours, démarrage noir et indépendance vidéo/AR conservés.
- Notices française et anglaise actualisées. Installation Windows stable et builds macOS Intel/Apple Silicon via Codemagic.

## Compatibilité et limites

Travaillez sur une copie si vous devez rouvrir le projet dans une version plus ancienne : elle peut ignorer les nouveaux fonds et contours supplémentaires. Les licences, formats métriques et projets StageFlow locaux/LIVE restent compatibles dans leur parcours existant. Aucun profil Beta n’est importé automatiquement dans le profil stable ; ouvrez explicitement vos fichiers enregistrés.

Les instruments sont des modèles génériques, pas des fiches constructeur. L’édition des sommets concerne le contour principal ; une ellipse convertie est une approximation Bézier. Les cotations restent des annotations, pas des repères AR.

Le compagnon AR n’est pas reconstruit dans cette livraison. Les nouveaux remplissages et contours supplémentaires ne sont pas entièrement transmis aux APK existantes (y compris build 14). La précision de calibration, les lunettes et la projection physique restent à qualifier sur le matériel réel. Les Mac ne sont pas signés Apple Developer ID ni notarisés ; le pipeline teste nativement ARM64 sur M2 et vérifie l’architecture Intel sans test natif Intel.

## English

The approved drawing beta becomes StageMark 2027.0.7 stable: grouped tools, personal library and 14 generic instrument presets; Shift-constrained rectangle/ellipse drawing; multi-vertex Points editing and explicit conversion to paths; thin, editable dimensions; independent fill/stroke and boolean operations preserving curves and holes; floating panels, compact controls and a balanced live workspace. Updated French/English manuals.

Keep a project copy for older versions, which may ignore added appearance fields. Beta preferences are not automatically imported into the stable profile. Instruments are generic; vertex editing covers the main contour; converted ellipses approximate cubic curves. Dimensions are annotations, not AR objects. Existing APKs (including build 14) do not fully display new fills/extra compound contours. No new APK or claim of hardware AR precision. macOS uses Codemagic; no Developer ID/notarisation, native ARM64 smoke and Intel architecture checks only.
