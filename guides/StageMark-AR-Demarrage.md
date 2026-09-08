# StageMark AR — premier essai sur téléphone

Préversion **0.1.1 build 3**, Android 10 minimum, ARM64 et téléphone [compatible ARCore](https://developers.google.com/ar/devices), dont le Galaxy A54 5G. La caméra et la précision doivent encore être validées sur chaque appareil. Les repères sont visibles sur l'écran du téléphone, pas réellement projetés au sol.

1. Installez la nouvelle [APK build 3](https://github.com/Mamat79/StageMark/releases/download/v2027.0.5/StageMark-AR-0.1.1-Development.apk?build=3) par-dessus l'ancienne, puis vérifiez **build 3** à l'accueil. Ne désinstallez pas l'application pour cette mise à jour.
2. Sur le PC, créez une scène de **2 m de large × 2 m de profondeur**, dans un espace dégagé réellement mesuré. Ajoutez une croix MIC 1 à **X 0 / Y 1 m** et enregistrez normalement.
3. Matérialisez les centres **A : X -1 m / Y 0**, **B : X +1 m / Y 0**, **C : X 0 / Y 2 m** avec de petits repères adhésifs mesurés. A et B sont les coins avant, C le milieu du fond. La mesure réelle doit correspondre à celle du logiciel.
4. Sur le PC : **Connexion → Réalité augmentée → ACTIVER STAGEMARK AR**. PC et téléphone doivent utiliser le même Wi-Fi privé.
5. Dans l'APK : **CAMÉRA DU TÉLÉPHONE**, puis autorisez la caméra. Si proposé, **INSTALLER LES SERVICES AR** ; cette installation Google initiale peut nécessiter Internet. StageMark ne filme ni n'envoie les images de caméra.
6. Saisissez le code à six chiffres du PC, puis **CONNECTER**. Déplacez doucement le téléphone pour détecter un sol horizontal éclairé et texturé, sans reflets. Ne visez pas une table.
7. Visez le centre A avec la croix centrale. Lorsqu'elle devient turquoise, touchez **RELEVER LE POINT A**. Répétez pour B et C, puis **CALIBRER LA SCÈNE**. Le téléphone ne reconnaît pas les lettres : vous choisissez les bons centres.
8. Contrôlez physiquement MIC 1 à l'endroit mesuré. Marchez doucement puis revenez : constatez l'écart. Un faible résidu mathématique ne certifie pas la précision du suivi.
9. **RÉGLAGES** ouvre le panneau complet. **RECOMMENCER A / B / C** efface la calibration. Pause, perte de suivi ou de réseau et changement de géométrie demandent de recalibrer. **QUITTER L'AR** libère la caméra ; le PC ne l'allume pas à distance.

Le mode **LUNETTES XREAL** est distinct : XREAL Air 2 Ultra + Beam Pro, APK ouverte depuis MyGlasses, marqueurs A/B/C imprimés à 100 % (carrés 160 mm) et placés aux positions indiquées dans StageMark. Relancez l'APK pour changer de mode. Les images XREAL doivent encore être qualifiées sur le matériel réel.

**Limites :** prototype de primitives, pas de garantie de rendu complet de tous les symboles complexes, de précision ou de stabilité après déplacement. Ne pas utiliser pour du positionnement critique. L'APK reçoit le plan en lecture seule ; aucune modification du projet, commande de projection ou levée de BLACKOUT. Pour des marques visibles par toute l'équipe, il faut un ou plusieurs vidéoprojecteurs.

## English — first phone test

Install **0.1.1 build 3** over the previous companion and check the build number on its home screen. Requires Android 10+, ARM64 and ARCore support. Real-device camera, accuracy and drift testing is still required.

1. Prepare a measured 2 × 2 m floor area. In StageMark create the matching stage and a MIC 1 cross at X 0 / Y 1 m.
2. Mark measured centres A(-1 m, 0), B(+1 m, 0), C(0, 2 m) on the floor. Their coordinates must match the project.
3. Start StageMark AR from the Desktop Connection panel. Use the same private Wi-Fi on both devices.
4. In the companion choose **CAMÉRA DU TÉLÉPHONE**, allow camera access and explicitly install Google AR Services if requested. Initial installation may need Internet. StageMark does not record or upload camera images.
5. Enter the PC's six-digit code and connect. Slowly scan a textured, well-lit horizontal floor.
6. Aim at A with the centre reticle; when turquoise, capture A. Repeat for B and C, then validate calibration. This is manual centre selection, not letter recognition.
7. Physically check MIC 1, walk away and return. Tracking/network loss, pause or changed geometry hides marks and requires recalibration. Quit AR to release the camera. Restart the APK to switch between phone and XREAL modes.

This is a personal screen overlay, not light projected onto the floor. Debug-signed primitive-rendering preview, not suitable for critical positioning. The companion cannot edit projects, start projection or remove BLACKOUT. See the [bilingual release notes](../RELEASE_NOTES_AR_0.1.1.md).
