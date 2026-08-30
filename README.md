# StageMark 2026 — distribution officielle

StageMark est une application de bureau hors connexion destinée aux techniciens de plateau. Elle dessine des repères en dimensions réelles, gère plusieurs plans et projette uniquement les graphismes utiles sur fond noir au moyen d’une calibration projective à quatre points. La version Windows 2026.6 ajoute les licences V2 ; les DMG macOS publics restent en 2026.5, non signés et non notariés, jusqu’à une validation Apple dédiée.

Ce dépôt public distribue uniquement les installateurs vérifiés de **StageMark 2026** et leurs empreintes SHA-256.
Le code source, le Worker de licence, les outils d’émission et les secrets restent dans un dépôt privé séparé.

## Télécharger

Les versions stables actuelles sont **2026.6 sous Windows** et **2026.5 sous
macOS** :

- Windows 11 x64 : `StageMark-2026.6-Setup.exe` ;
- macOS Intel : `StageMark-2026.5-macOS-x64.dmg` ;
- macOS Apple Silicon : `StageMark-2026.5-macOS-arm64.dmg`.

Téléchargement : <https://github.com/Mamat79/StageMark/releases/latest>

Chaque installateur possède un fichier `.sha256` séparé. Les binaires sont publiés uniquement comme assets de Release et ne sont jamais ajoutés à l’historique Git.

## Licence

StageMark reste entièrement utilisable :

- 30 jours sans rappel ;
- après 30 jours, un rappel refermable au démarrage ;
- licence permanente à **49 € TTC**, paiement unique, pour supprimer le rappel ;
- les licences historiques restent valables après mise à jour, réinstallation
  compatible et changement entre Windows et macOS ;
- Windows 2026.6 accepte aussi les licences V2 : activation Internet initiale,
  trois installations par défaut, puis validation entièrement hors ligne et
  bouton de désactivation du poste.

Boutique officielle : <https://stagemark-license.mamat79-dce.workers.dev/buy>

Le paiement est traité hors de l’application par Stripe. StageMark n’accède à
aucune donnée bancaire. La boutique émet encore le format historique portable
compatible avec Windows et macOS ; le passage commercial à V2 attend une
version macOS signée et testée. Il n’existe plus de parcours PayPal dans
l’application.

## Mise à jour

StageMark vérifie la dernière Release GitHub sans bloquer le démarrage. Le téléchargement et l’installation exigent toujours une confirmation, puis l’empreinte SHA-256 de l’installeur est contrôlée avant exécution.

## Documentation et limites

Les notices française et anglaise sont embarquées dans l’application et accessibles depuis l’aide.

- L’installeur Windows n’est pas signé numériquement.
- Les DMG macOS sont non signés et non notariés ; macOS peut demander une confirmation manuelle.
- La validation sur vidéoprojecteur, MadMapper, téléphone et Stream Deck dépend du matériel réel et doit être effectuée sur site.

## Banque de vidéoprojecteurs

La banque distribuable se trouve dans [`projector-catalog/`](projector-catalog/README.md). Une fiche ou un visuel n’est accepté qu’après contrôle de sa source et de son droit de redistribution.

---

# StageMark 2026 — official distribution

This public repository contains only verified **StageMark 2026** installers and their SHA-256 files. Source code, licensing services, issuing tools, and secrets remain in a separate private repository.

The current stable versions are **2026.6 for Windows 11 x64** and **2026.5 for
macOS Intel and Apple Silicon**. Download them from
<https://github.com/Mamat79/StageMark/releases/latest>.

StageMark provides 30 reminder-free days, remains fully usable afterwards with
a dismissible startup reminder, and offers a permanent **€49 tax-included**
one-time license. Historical V1 licenses remain portable. Windows 2026.6 also
supports installation-bound V2 licenses with offline validation after initial
activation. Purchase at <https://stagemark-license.mamat79-dce.workers.dev/buy>.

Windows and macOS packages are currently unsigned; macOS DMGs are not notarized.
