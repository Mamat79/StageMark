# StageMark AR 0.1.1 — build 18

## Français

AR disponible sur téléphone Android 10+ ARM64 compatible ARCore. Lunettes : intégration et essais en cours.

- Caméra plein écran après calibration, réglages accessibles et cohérence masquable.
- Visée manuelle du sol proposée par défaut, choix libre du point A/B/C à relever, relevé rapide et distances attendues/mesurées pour comprendre un écart. La reconnaissance reste disponible et nécessaire pour les cibles verticales sur pied.
- Une calibration terminée n’expire plus simplement parce que vous passez dans une autre application. Au retour, la connexion et la cohérence du suivi sont revérifiées avant confirmation de reprise. Si les ancres sont perdues ou Android a fermé le processus, une nouvelle calibration reste nécessaire.
- Avec Desktop 2027.0.11 : le PC peut autoriser un téléphone à déplacer un objet du plan actif. Déplacer puis valider ou annuler ; Annuler fonctionne aussi sur le PC. Pas encore de création, suppression, rotation ni redimensionnement depuis l’AR. Les groupes et objets verrouillés ne sont pas déplacés.

Installation manuelle, certificat de développement conservé pour la continuité des mises à jour. La caméra n’est ni enregistrée ni envoyée. Un réseau local permettant les échanges est nécessaire ; les Wi-Fi d’hôtel peuvent isoler les appareils. Vérifiez un emplacement connu après calibration : le pourcentage exprime une cohérence, pas une précision garantie. Les nouveautés de cette version demandent encore un essai sur votre téléphone et votre scène ; elles ne qualifient pas les lunettes.

## English

AR is available on ARCore-compatible Android 10+ ARM64 phones. Glasses integration and testing are ongoing.

- Full camera view after calibration, accessible settings and an optional consistency badge.
- Manual floor aiming by default, free A/B/C acquisition order, quick capture and expected/measured distance feedback. Image recognition remains available and is required for raised vertical targets.
- Completed calibration no longer expires just because another app was opened. Reconnection and tracking coherence are checked before confirmed recovery. Lost anchors or an Android process restart still require recalibration.
- With Desktop 2027.0.11, explicitly permit one phone to move an active-plan object, then confirm or cancel. PC undo remains available. No AR creation, deletion, rotation, resizing or grouped/locked-object movement yet.

Manual installation; the existing development certificate is retained for update continuity. Camera imagery is neither recorded nor sent. A local network allowing device communication is required; hotel Wi-Fi may isolate devices. Verify a known position after calibration: consistency is not guaranteed accuracy. New features still need testing on your phone and stage; these tests do not qualify glasses support.
