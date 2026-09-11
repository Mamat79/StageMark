# StageMark 2027.0.8 — calibration AR au sol ou sur pied

Cette version stable conserve l’atelier de dessin 2027.0.7 et ajoute les réglages nécessaires au compagnon **StageMark AR 0.1.1 build 15**, toujours en préversion.

- Choisissez une cible à plat au sol ou verticale sur pied, séparément pour A, B et C, dans Sorties & installation → Réalité augmentée → Guide → Placement A/B/C.
- Indiquez la hauteur réelle du centre au-dessus du sol local. La fiche de placement du projet rappelle X/Y, support et hauteur. Les mêmes feuilles réutilisables conviennent : motif complet de 160 × 160 mm, impression à 100 %.
- Sur téléphone : reconnaissance de la lettre attendue, sans devoir attendre la détection du sol sous une cible reconnue. Une pression lance le relevé lissé sur plusieurs images ; progression et confirmation restent visibles.
- Repli manuel au sol disponible ; les cibles sur pied exigent leur reconnaissance. Reprendre un point conserve les autres ancres encore suivies.
- La hauteur est traitée séparément de la pente. Les écarts admissibles peuvent être acceptés explicitement ; l’indice de cohérence masquable n’est pas une précision garantie.
- Vidéo et AR restent indépendantes. Le masque personnel ne peut pas annuler celui du PC. Démarrage vidéo noir, BLACKOUT et fermeture de secours conservés.
- Notices FR/EN et guide AR actualisés. Windows stable et macOS Intel/Apple Silicon distribués dans cette Release ; les DMG sont ajoutés par Codemagic lorsqu’ils sont vérifiés.

## Compatibilité et limites

Sauvegardez une copie avant de rouvrir un projet dans une ancienne version Desktop, qui ne conserve pas les nouveaux supports/hauteurs. Les anciens APK ne reçoivent pas les repères surélevés : utilisez build 15 avec StageMark 2027.0.8. Aucun profil Beta n’est importé automatiquement dans la stable.

**L’APK reste une préversion Android ARM64 signée avec une clé de développement.** Le nouveau relevé optique et la précision nécessitent une validation physique sur chaque appareil et lieu ; les tests logiciels ne la remplacent pas. Vérifiez une position connue après calibration ; n’utilisez pas l’AR pour un repérage critique. Une interruption ou une perte globale prolongée peut imposer une nouvelle calibration. Mode téléphone : Android 10+ et ARCore ; XREAL Air 2 Ultra + Beam Pro reste un parcours distinct à qualifier, sans changement de priorité ni annonce de prise en charge RayNeo.

Les remplissages et contours supplémentaires des formes composées ne sont pas encore entièrement transmis en AR ; les cotations restent des annotations du plan. Les fichiers Mac ne sont ni signés Apple Developer ID ni notarisés. Le pipeline teste nativement ARM64 sur M2 et contrôle l’architecture Intel, sans test natif Intel. Ne désactivez pas les protections macOS.

## English

StageMark 2027.0.8 keeps the drawing workspace and adds independent floor/vertical mounting and centre-height settings for targets A/B/C, saved in the project and shown on its placement sheet. Reuse the same complete 160 mm markers printed at 100%. Measure height vertically from the local floor to the pattern centre, directly above the stated X/Y.

The accompanying **AR 0.1.1 build 15 preview** recognises the expected letter on phone cameras, smooths capture over several frames and retains other tracked anchors when one point is repeated. Manual floor targeting remains available; raised targets require image recognition. Height and stage slope are handled separately. Explicit acceptance of permitted deviations and the hideable consistency indicator remain; that indicator is not guaranteed accuracy. Video, PC AR visibility and personal hiding remain independent as documented.

Use Desktop 2027.0.8 with APK 15 for raised targets; old APKs receive no raised geometry. Keep a copy for older Desktop versions, which do not retain these settings. Optical capture and accuracy still require physical qualification; verify a known point and never rely on AR for critical positioning. Tracking loss/interruption may require recalibration. Development-signed Android ARM64 preview, Android 10+ and ARCore for phone mode; separate XREAL path still requires hardware validation, no new RayNeo support claimed. New fills and extra compound contours are not fully transmitted; dimensions remain plan annotations. macOS builds use Codemagic, without Developer ID or notarisation; native ARM64 smoke, Intel architecture verification only.
