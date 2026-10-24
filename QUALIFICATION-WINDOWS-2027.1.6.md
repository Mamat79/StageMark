# StageMark 2027.1.6 — qualification Windows / Windows qualification

Cette livraison concerne **Windows x64**. Le paquet a été construit localement, contrôlé puis installé en remplacement de 2027.1.5. Son premier démarrage personnel et sa fermeture normale ont été vérifiés.

## Identités et intégrité

| Élément | Identité |
| --- | --- |
| Source application compilée | `9e054678e3163c268b5e7cdd94555f8eae3cf14e` |
| Branche de construction | `fix/license-continue-visible-20261024` |
| Documentation embarquée | `7d776ee8c1a72dfc45a39959e665ec4e76a78b00` |
| Arbre documentaire vérifié ensuite | `75aee5601fb21f1f4ef25e8337d0ac06ecd4da27` |
| Intégration documentaire privée | `d8df1a2e8625949e8953e9e7abc7d81f1480022e` |
| Installeur | `StageMark-2027.1.6-Setup.exe`, 121864122 octets |
| SHA-256 de l’installeur | `6b1bd60da4b580b39f15352359295488b53f792f096f4e7cf1a22180a1d76630` |
| SHA-256 de StageMark.exe | `d3c9ef80f7beca21c212d66cb354547f31a11d5307be95f36c6d664073457b42` |
| SHA-256 de app.asar | `2e4753fc4b0088d35adb95839d6005a9cab36f9a1f459da02b5cf2f9581ea101` |

Le commit documentaire final contient les fichiers approuvés et la mise à jour factuelle de STATUS.md après les tests. Il ne devient pas la source du binaire déjà construit. Les deux notices PDF intégrées à l’installeur sont identiques aux notices jointes à cette Release. Les guides Suite 2027.3 restent inchangés.

## Vérifications réellement effectuées

- Recette complète `test.ps1` sur l’arbre documentaire exact : **1 278 tests Vitest réussis, 19 ignorés**, puis **90 tests Node réussis**, aucun échec, annulation ou saut Node. Sortie native de PowerShell zéro et capture complète des deux flux. Les 19 tests ignorés concernent des fixtures externes et un pipe QA optionnel absents ; ils ne sont pas présentés comme réussis.
- Source suivie et 18 302 fichiers de dépendances vérifiés avant/après ; seule la sortie de cache Vitest déclarée est générée. Aucun nouveau build, PDF ou changement de code n’a été réalisé pendant cette validation documentaire.
- Inspection du paquet : les **116 fichiers du payload** sont identiques au paquet décompressé ; ressources, version, notices, trois clés publiques et composants Spout contrôlés. L’installation comporte ces 116 fichiers et le désinstalleur correspondant exactement au Setup.
- Recette d’installation officielle : l’installeur et les quatre contrôles du programme installé ont chacun terminé avec le **code zéro** : démarrage logiciel, Spout synthétique, export d’équipe PDF/PNG et fermeture/échappement. Les deux exports ont été conservés et leur signature de fichier vérifiée.
- Matrice visuelle FR/EN, clair/sombre, fenêtres compacte/grande : acceptation de l’en-tête/pied fixe, du bouton Continuer entièrement visible et du défilement central. Les rapports bruts partiels de certains parcours fonctionnels restent partiels ; cette acceptation de style ne transforme pas toute la matrice en validation fonctionnelle complète.
- Remplacement local de 2027.1.5 par 2027.1.6 avec sauvegardes indépendantes et répétition de restauration isolée. Avant le premier lancement normal : réglages, projets, état de licence et métadonnées comparés ; seuls les nouveaux fichiers de sauvegarde de raccourcis prévus ont été ajoutés.
- Un seul lancement normal du binaire installé, profil personnel existant, sans argument ni profil de test : licence offerte existante affichée active, thème/langue et références de projets récents présents, sortie fermée/noire et AR arrêtée. Fermeture normale, vrai code natif zéro. Aucun achat, code saisi ou nouvelle activation.
- Après ce lancement : préférences JSON et clés de stockage utilisateur inchangées, début d’essai/token/clés/reçu de licence inchangés ; seule la dernière utilisation a avancé normalement. Les modifications de cache, journaux, session et minuteur interne Chromium ont été inventoriées et expliquées individuellement. Aucun fichier de projet n’a été modifié.

Le run global initial de construction reste enregistré en échec de supervision, malgré les sorties zéro des scripts de tests et de build : un processus de diagnostic résiduel empêchait sa clôture. Le paquet a ensuite fait l’objet de qualifications indépendantes statique, native, d’installation et de démarrage personnel. Cet échec initial et les essais documentaires interrompus ne sont pas renommés en succès ; la validation documentaire complète ci-dessus est une exécution ultérieure distincte.

## Limites

L’installeur Windows n’est pas signé numériquement. Aucun achat de certificat, changement de protection Windows ou contournement de dialogue de sécurité n’a été effectué.

Les contrôles de Spout et d’exports sont logiciels et synthétiques. Ils ne qualifient ni vidéoprojecteur, calibration, audio, réseau réel, AR, lunettes, précision physique ou conduite sur site. Les références de projets récents ont été consultées sans ouvrir ni enregistrer les projets. La validité d’une nouvelle activation payée et le fonctionnement avec un réseau effectivement coupé n’ont pas été testés. Certains parcours natifs de timing/clavier restent explicitement non vérifiés ; aucune campagne de répétition n’a été ajoutée.

V1 demeure le défaut. V2 exige une copie locale explicite ; V2 LIVE réseau/AutoCAD n’est pas qualifié par cette livraison.

**macOS est inchangé** : Apple Silicon reste en **2027.1.5**, Intel en **2027.1.3**. Les fichiers, identifiants, empreintes et liens des Releases Mac d’origine sont préservés. Aucun paquet ni job Mac n’a été créé pour cette livraison Windows. Les qualifications Mac historiques conservent leurs propres limites ; aucun lancement Intel n’est déduit de ces contrôles Windows.

## English

Windows 2027.1.6 was built locally, inspected, installed over 2027.1.5 and started once with the existing personal profile. The complete documentation-tree test run passed **1,278 Vitest tests with 19 skipped**, followed by **90 Node tests with no failure or skip**. The installer and all four installed software smokes returned zero; the normal personal process also exited normally with native code zero.

The source application, embedded documentation and later documentation integration have separate identities listed above. The initial build supervisor failure and interrupted documentation attempts remain recorded as failures; they are not relabelled as passes. The distributed payload was independently qualified afterwards.

Settings, projects and licence information were retained. Only the normal licence last-seen timestamp and individually reviewed runtime cache/log/session metadata changed during the personal launch. No purchase, activation, code issuance or licence reset was performed. Existing storage values and trial-start/token/key/receipt fields remained unchanged.

The Windows installer is unsigned. Hardware projection, calibration, audio, live network, AR accuracy, glasses, new paid-code activation and operation with networking actually disabled are not qualified here. Some native timing/keyboard paths remain unverified. Recent project references were viewed without opening or saving their projects. Keep real-world pre-show checks.

Existing Mac downloads stay at Apple Silicon **2027.1.5** and Intel **2027.1.3**, with their original assets and limits. No new Mac build, job, version or asset is part of this Windows release.
