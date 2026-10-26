# StageMark 2027.1.7 — qualification Windows

**Cette livraison concerne Windows 2027.1.7. Les paquets et notices macOS restent en 2027.1.6.** Les nouveaux paquets Mac seront publiés après leur propre qualification. Les anciennes releases sont conservées.

**This release delivers Windows 2027.1.7. macOS packages and specific manuals remain at 2027.1.6.** New Mac packages will be published after their separate qualification. Previous releases are preserved.

## Français

Paquet construit localement depuis le produit et la recette privée
`ea2d449d8ae1045806ba971cf470903fbadf7e3b`, avec le script officiel
`build-windows.ps1`. Aucun build Windows GitHub Actions utilisé. L'installeur
Windows x64 est non signé.

La refonte place plans/calques à gauche, propriétés à droite et palette
contextuelle sous le canevas. Les panneaux restent repliables et détachables.
La bande fixe conserve AFFICHER, BLACKOUT et FERMER SORTIE ; AFFICHER est
indisponible tant que la sortie est fermée. L'autorisation AR reste distincte
du blackout vidéo.

Les contrôles du propriétaire du code comprennent lint, types, 95 tests Node,
12 rendus FR/EN clair/sombre et des vérifications de géométrie à trois largeurs.
La première suite Vitest a donné 1285 réussites, 14 cas ignorés et l'échec d'une
ancienne assertion statique qui cherchait la sécurité dans l'ancien en-tête.
Après adaptation de cette assertion à la nouvelle bande, 25 tests ciblés ont
réussi. Le bilan couvre 1286 identifiants de tests distincts validés ; aucune
seconde exécution intégrale n'est revendiquée. Les quatre notices produit ont
été actualisées, rendues et relues par leur propriétaire : 17 pages en français
et 16 en anglais pour chaque plateforme.

Le véritable installeur a été extrait : ses 116 fichiers correspondent aux
sorties de construction. L'archive applicative contient la bonne version et
les composants attendus. Le programme extrait a démarré avec un profil et une
présence de suite isolés, puis son contrôle interne s'est terminé avec le code
0. Une séance visible distincte a montré la vraie fenêtre, les panneaux, le
canevas et la bande de sécurité. La sortie est restée fermée, AFFICHER désactivé,
sans projection ni télécommande. La fermeture normale s'est terminée avec le
code 0, sans arrêt forcé.

La mise à jour de l'installation existante a réussi après deux sauvegardes
privées indépendantes sur C: et D: : 373 fichiers, 476489373 octets par copie,
avec un fichier restauré dans un dossier d'essai. Les 116 fichiers applicatifs
installés correspondent au paquet ; les 202 fichiers personnels comparés sont
inchangés. La version du registre Windows réel, les raccourcis et leur cible
ont été vérifiés. L'installation Beta séparée est préservée. Le programme
installé a ensuite passé son démarrage de contrôle sur un profil isolé et
quitté avec le code 0. Aucun projet personnel n'a été ouvert pour cette séance.

Limites : pas de recette physique de vidéoprojecteur, sortie audio, Spout,
lunettes AR, matériel MIDI/Stream Deck ou réseau entre postes. Pas de matrice
complète de changements de DPI Windows ni de validation exhaustive de toutes
les commandes par clic humain. Les observations macOS appartiennent à leur
qualification séparée. Les licences, formats et données existants ne sont pas
réinitialisés par cette recette.

## English

Locally built Windows x64 package from product/recipe
`ea2d449d8ae1045806ba971cf470903fbadf7e3b`, using the official PowerShell
recipe. No Windows GitHub Actions build. The Setup is unsigned.

The Drawing layout moves plans/layers left, properties right and the contextual
palette below the canvas. Foldable/floating panels remain available. The fixed
SHOW/BLACKOUT/CLOSE OUTPUT strip remains visible, with SHOW disabled until an
output is open; AR visibility remains independent of video blackout.

Source-owner checks included lint/types, 95 Node tests, 12 light/dark FR/EN
renders and geometry checks at three widths. Initial Vitest results were
1285 passes, 14 skips and one obsolete static header expectation failure.
After adapting that expectation to the fixed safety strip, 25 targeted tests
passed. This validates 1286 distinct test IDs; no second full suite is claimed.
All four product manuals were updated, rendered and reviewed: 17 French and
16 English pages per platform.

All 116 files extracted from the actual Setup matched the qualified build.
The packaged application passed its internal startup with isolated profile and
suite presence. A separate visible native session showed the canvas, panels
and safety strip with output closed and SHOW disabled. No projection or remote
control was enabled. Normal close returned 0 without forced termination.

The existing installation was upgraded after independently verified private
backups on two volumes. Installed payload, actual Windows registry, version and
shortcuts passed; all 202 compared personal files and the separate Beta
installation were preserved. Installed startup with an isolated profile exited
0. A backup sample was restored into a test directory, without real-profile
rollback or opening a personal project.

Physical projection, audio, Spout, AR glasses, MIDI/Stream Deck and cross-machine
networking were not tested. No exhaustive human command or OS-DPI transition
matrix is claimed. macOS evidence is separate. This qualification performs no
licence reset or existing-data reset.

## SHA-256

```text
d05a18dd131f1903a0d4f578e839317e730b1e8e1da2a3c974689c8f6be154e7  StageMark-2027.1.7-Setup.exe
```
