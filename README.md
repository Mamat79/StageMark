<p align="center">
  <img src="branding/stagemark-logo.png" width="256" alt="StageMark 2027">
</p>

<h1 align="center">StageMark 2027</h1>

<p align="center">
  <strong>Dessinez l’implantation. Calibrez la projection. Affichez uniquement les repères utiles.</strong><br>
  Hors ligne · Français / English · Windows 11 · macOS Intel / Apple Silicon · préversion AR Android
</p>

<p align="center">
  <a href="#downloads"><strong>⬇ Télécharger StageMark</strong></a>
  · <a href="guides/StageMark-Notice-FR.pdf">Notice FR</a>
  · <a href="guides/StageMark-Notice-EN.pdf">Guide EN</a>
  · <a href="guides/Guide-Suite-SiLeMIO-FR.pdf">Guide de la suite</a>
</p>

<p align="center">
  <em>Interface 2027.0.6 — présentation commentée / Narrated presentation</em><br>
  <a href="https://github.com/Mamat79/StageMark/releases/download/v2027.0.6/stagemark-2027.0.6-presentation-fr.mp4"><img src="https://github.com/Mamat79/StageMark/releases/download/v2027.0.6/stagemark-2027.0.6-presentation-fr-poster.png" width="820" alt="StageMark 2027.0.6 : dessin du plateau et nouveau parcours"></a><br>
  <a href="https://github.com/Mamat79/StageMark/releases/download/v2027.0.6/stagemark-2027.0.6-presentation-fr.mp4">Présentation · FR</a>
  · <a href="https://github.com/Mamat79/StageMark/releases/download/v2027.0.6/stagemark-2027.0.6-presentation-fr.vtt">Sous-titres FR</a>
  · <a href="https://github.com/Mamat79/StageMark/releases/download/v2027.0.6/stagemark-2027.0.6-presentation-en.mp4">Presentation · EN</a>
  · <a href="https://github.com/Mamat79/StageMark/releases/download/v2027.0.6/stagemark-2027.0.6-presentation-en.vtt">EN captions</a>
</p>

Captures du vrai renderer, projet fictif, sorties arrêtées. Montage commenté par voix synthétique ; aucune démonstration de précision AR ou de projection réelle. / Actual renderer captures, fictional project, outputs stopped. Synthetic narration; not a hardware or AR-accuracy demonstration.

![Conduite StageMark 2027.0.6 : plans, cues et commandes indépendantes](https://github.com/Mamat79/StageMark/releases/download/v2027.0.6/stagemark-2027.0.6-live-fr.png)

---

## StageMark, à quoi ça sert ?

StageMark est un outil de préparation et de projection destiné aux techniciens
de plateau, régisseurs, scénographes et équipes de production.

Il permet de dessiner une implantation en dimensions réelles, d’organiser
plusieurs plans et d’envoyer sur le plateau uniquement les repères nécessaires :
positions, axes, formes, textes, groupes d’affichage ou éléments de conduite.

La projection reste sur fond noir et un **BLACKOUT** permanent permet de couper
immédiatement l’image.

## Quel matériel faut-il ?

- **Pour dessiner et préparer un plan**, aucun vidéoprojecteur n’est requis : StageMark fonctionne seul sur l’ordinateur et enregistre ses projets autonomes `.stagemark`.
- **Pour faire apparaître les marques sur le sol**, il faut relier l’ordinateur à **un ou plusieurs vidéoprojecteurs**. Une grande scène, une puissance lumineuse limitée ou la réduction des ombres peut demander plusieurs appareils ou un logiciel de mapping.
- **Pour voir personnellement les marques en réalité augmentée**, la préversion StageMark AR propose la caméra d'un [téléphone compatible ARCore](https://developers.google.com/ar/devices), dont le Galaxy A54 5G, ou les [XREAL Air 2 Ultra](https://developer.xreal.com/) avec un [XREAL Beam Pro](https://www.xreal.com/beampro). La superposition n'est visible que sur l'écran ou dans les lunettes : elle ne remplace pas la projection destinée à toute l'équipe.

StageMark fournit l’image à projeter, mais ne commande pas l’alimentation physique du vidéoprojecteur. La sortie reste noire tant que l’opérateur n’utilise pas **AFFICHER**, et **BLACKOUT** reste prioritaire.

## Un exemple concret

Vous préparez un changement de plateau avec une batterie, un piano, des wedges,
des pieds de micro et plusieurs positions d’artistes :

1. créez le plan aux dimensions du plateau ;
2. placez les objets et repères en millimètres ;
3. regroupez les éléments qui doivent apparaître ensemble ;
4. préparez plusieurs plans ou états d’affichage ;
5. raccordez le vidéoprojecteur et affichez la mire ;
6. calibrez les quatre coins de la zone utile ;
7. affichez uniquement le groupe nécessaire pendant le changement ;
8. déclenchez le blackout dès que la projection n’est plus utile.

L’équipe de plateau voit des repères clairs, sans exposer l’interface de travail
ni le fond du plan.

## Ce que StageMark permet de faire

### Dessiner une implantation précise

- Plans en dimensions réelles.
- Plusieurs unités d’affichage, avec mesures cohérentes.
- Points, croix, cercles, carrés, triangles, lignes, flèches et rectangles.
- Textes et objets personnalisables.
- Symboles de plateau : wedges, pieds de micro, amplis, batterie, piano,
  chaises et risers.
- Cotations persistantes.
- Alignement, distribution, duplication et groupes d’objets.
- Fond de plan estompé pour servir de référence sans être projeté.

### Organiser le spectacle

- Plusieurs plans dans un même projet.
- Groupes d’affichage instantanés.
- Calque permanent pour le site et les obstacles.
- Cues de conduite.
- Annulation, rétablissement et récupération après une interruption.
- Export ou impression des plans en A4.

### Projeter en sécurité

- Fenêtre de sortie séparée de l’éditeur.
- Projection directe ou sortie Spout sous Windows.
- Mire de calibration.
- Correction géométrique par quatre points.
- Commandes permanentes **AFFICHER** et **BLACKOUT**.
- Raccourcis clavier et profils Stream Deck.
- Prévol avant diffusion.

### Contrôler depuis le plateau

Un contrôleur local peut être ouvert depuis le navigateur d’un téléphone, d’une
tablette ou d’un autre ordinateur connecté au même réseau local.

Il permet de rappeler les plans et les cues utiles sans transformer StageMark
en service cloud.

StageMark 2027.0.5 enrichit aussi le dessin mobile : créer un objet natif
nommé, le placer au toucher, le sélectionner par nom, modifier ses mesures,
le déplacer et confirmer sa suppression. Les verrous du plan sont respectés.
Le QR direct et le portail StageFlow ouvrent le même éditeur ; la prise de
contrôle reste explicite et aucune connexion ne démarre la projection.

### Préparer le vidéoprojecteur

La banque intégrée aide à comparer des vidéoprojecteurs et objectifs pour la
préparation d’une location ou d’une installation : luminosité, poids, rapport
optique, orientation et informations utiles.

Le choix final et la calibration doivent toujours être validés avec le matériel
réel et les conditions du lieu.

### Préversion technique StageMark AR

**Nouveau : interface Desktop simplifiée en 2027.0.6 et APK 0.1.1 build 12.** « Connexion StageFlow » regroupe le réseau et la télécommande ; « Sorties & installation » regroupe vidéo, AR et calibration. La Conduite conserve plans, cues et commandes de diffusion. « Démarrer l’AR » crée la session et autorise les repères en une action ; l’association et la calibration restent obligatoires. Un guide pas à pas est facultatif.

Le compagnon **0.1.1 build 12** propose une interface tactile défilante, des boutons accessibles et des réglages séparés. Il corrige l’entrée native de pose caméra et n’ajoute plus le nom interne « Cross » aux objets sans étiquette. Le rendu d’une croix et le changement de couleur ont été observés sur A54 ; précision, dérive et relocalisation restent à mesurer. XREAL reste à qualifier physiquement. **AFFICHER AR / MASQUER AR** sont indépendants de la vidéo ; **MASQUER POUR MOI** concerne seulement une personne. Feuilles A/B/C réutilisables et fiche de placement facultative par projet. [Démarrage rapide](guides/StageMark-AR-Demarrage.md) · [Parcours et limites](RELEASE_NOTES_2027.0.6.md).

**Écran noir qui recouvre le bureau ? Ctrl+Maj+F12**, Échap dans la sortie ou **FERMER SORTIE** ferment vidéo/rideau noir/Spout sans quitter le projet ni arrêter l’AR. BLACKOUT garde volontairement une fenêtre noire ouverte ; fermer peut montrer le bureau sur le projecteur.

Le compagnon reçoit le plan actif en lecture seule sur le réseau local et s'associe par code éphémère. Le mode téléphone nécessite Android 10 minimum, ARM64 et la compatibilité ARCore ; la première installation des services AR Google peut demander Internet. Les images caméra ne sont ni enregistrées ni envoyées par StageMark. Le mode XREAL conserve ses marqueurs imprimables A/B/C.

L’APK est signé avec une clé de développement. Sa compilation, son identité, sa signature et son protocole ont été contrôlés ; le démarrage caméra, la précision, la dérive et la relocalisation doivent encore être testés sur le matériel réel avant tout usage critique. Il ne peut ni modifier le projet, ni afficher la sortie vidéoprojecteur, ni retirer un **BLACKOUT**.

## Le même projet que le patch et le plan technique

Par défaut, StageMark crée, ouvre et enregistre ses propres projets autonomes
<code>.stagemark</code>. Aucun autre logiciel n’est nécessaire. L’ouverture
d’un projet partagé <code>.stageflow</code> est un parcours supplémentaire et
StageFlow reste entièrement optionnel.

Il peut lire le patch commun, placer des sources sans les ressaisir et reprendre
un plan provenant de StageFlow ou d’AutoCAD.

Avec StageFlow LIVE, StageMark peut suivre automatiquement les nouvelles
révisions de patch et de plan CAD ; leur adoption reste toujours une action
explicite de l’opérateur, même lorsque l’éditeur est propre. Les changements
locaux ne sont jamais écrasés : un conflit est signalé et reste à arbitrer. Ce
suivi ne peut jamais afficher une image, retirer le **BLACKOUT**, changer
l’écran de projection ou rappeler une cue.

Le centre **Connexion StageFlow** réunit l’association volontaire à une session LIVE
et la vraie télécommande StageMark. L’ouverture du centre ne lance aucun
service ni recherche. Un bandeau orange présente les changements de labels ;
les acquittements restent locaux au poste et limités aux alertes présentes
au clic. La pause des notifications de StageFlow est distincte du choix local.

La déclaration de présence de StageMark et ses commandes par pipes locales
sont réservées à Windows. Sur Mac, StageFlow peut lancer StageMark sur un
projet local ; rejoindre LIVE reste explicite dans StageMark. Les projets
locaux `.stageflow`, le LIVE réseau et la télécommande restent utilisables.

~~~mermaid
flowchart LR
    SF["StageFlow<br/>Patch + plan"] <--> P[("Projet .stageflow")]
    SMT["StageDesk"] <--> P
    SM["StageMark<br/>Implantation + projection"] <--> P
    MON["StageMon<br/>Matrice d’écoute live"] <--> P
    DCE["Dante Config Editor<br/>Réseau Dante"] <--> P
    CAD["AutoCAD<br/>Plan technique"] <--> P
~~~

- [StageFlow — patch, groupes, Excel et plan de scène](https://github.com/Mamat79/StageFlow/releases/latest)
- [StageDesk — transfert entre consoles et logiciels](https://github.com/Mamat79/StageDesk/releases/latest)
- [StageMark — implantation et projection scéniques](https://github.com/Mamat79/StageMark#downloads)
- [StageMon — matrice d’écoute live](https://github.com/Mamat79/StageMon/releases/latest)
- [Dante Config Editor — préparation Dante hors ligne](https://github.com/Mamat79/Dante-Config-Editor/releases/latest)
- [AutoCAD — plan technique et connecteur StageFlow](https://github.com/Mamat79/StageFlow/releases/latest)

Chaque logiciel reste autonome. Vous installez uniquement les outils utiles à
votre production.

<a id="downloads"></a>

## Télécharger StageMark

**StageMark 2027.0.6 pour Windows 11 x64, macOS Intel et Apple Silicon** et **StageMark AR 0.1.1 build 12** sont disponibles. Les DMG sont construits par Codemagic depuis le même tag source que Windows et leurs SHA-256 sont vérifiés.

- [Windows x64 — 2027.0.6](https://github.com/Mamat79/StageMark/releases/download/v2027.0.6/StageMark-2027.0.6-Setup.exe) · [SHA-256](https://github.com/Mamat79/StageMark/releases/download/v2027.0.6/StageMark-2027.0.6-Setup.exe.sha256)
- [macOS Intel — 2027.0.6](https://github.com/Mamat79/StageMark/releases/download/v2027.0.6/StageMark-2027.0.6-macOS-x64.dmg)
- [macOS Apple Silicon — 2027.0.6](https://github.com/Mamat79/StageMark/releases/download/v2027.0.6/StageMark-2027.0.6-macOS-arm64.dmg)
- [StageMark AR 0.1.1 build 12 — APK de développement](https://github.com/Mamat79/StageMark/releases/download/v2027.0.6/StageMark-AR-0.1.1-Development.apk) · [SHA-256](https://github.com/Mamat79/StageMark/releases/download/v2027.0.6/StageMark-AR-0.1.1-Development.apk.sha256)

Les paquets de bureau et leurs SHA-256 sont réunis dans la même Release stable.
L’APK reste explicitement expérimental et ne constitue pas une application
Android de production. Les anciennes Releases restent disponibles pour un
retour à une version antérieure.

[Manifeste SHA-256 complet de la version 2027.0.6](SHA256SUMS-2027.0.6-complete). Mettre à jour le Desktop pour la nouvelle organisation ; l’APK build 12 remplace la précédente sans désinstallation.
Les notices et guides propres à chaque paquet sont embarqués dans l’application.
Les anciennes Releases restent disponibles pour un retour à une version antérieure.

**[Release StageMark 2027.0.6](https://github.com/Mamat79/StageMark/releases/tag/v2027.0.6)**

Les notices française et anglaise sont intégrées à l’application et accessibles
depuis le bouton **Guide** ; **Aide** propose aussi le guide de la suite.
Elles sont également disponibles directement :
[français](guides/StageMark-Notice-FR.pdf),
[English](guides/StageMark-Notice-EN.pdf),
[guide de la suite FR](guides/Guide-Suite-SiLeMIO-FR.pdf) et
[suite guide EN](guides/SiLeMIO-Suite-Guide-EN.pdf).
Le [manifeste des guides communs](guides/suite-guides-manifest.json) donne
leurs tailles et empreintes pour vérifier les copies.

## Utilisation et licence

StageMark offre 30 jours sans rappel au premier lancement. Ensuite,
l’application et toutes ses fonctions restent utilisables ; un rappel apparaît
simplement au démarrage.

Une licence permanente à **49 € TTC**, en paiement unique, supprime ce rappel.

**[Acheter une licence permanente StageMark](https://stagemark-license.mamat79-dce.workers.dev/buy)**

## À savoir avant un spectacle

- L’installeur Windows actuel n’est pas signé numériquement ; Windows peut
  afficher un avertissement.
- Les images macOS actuelles ne sont ni signées avec un certificat Developer ID
  ni notariées par Apple ; macOS peut donc afficher un avertissement Gatekeeper.
- Le minimum macOS déclaré est 12. Pour 2027.0.6, le paquet Apple Silicon a été lancé sur le runner M2 ; l’architecture Intel a été contrôlée, sans lancement natif Intel. Toutes les versions de macOS ne sont pas qualifiées.
  Les signatures d’intégrité existantes sont préservées ; ne désactivez pas les
  protections macOS.
- La calibration doit être vérifiée sur le vidéoprojecteur et dans le lieu réel.
- Testez le blackout, la sortie, le contrôleur et les raccourcis avant
  l’exploitation.

---

## English

### What is StageMark for?

StageMark is an offline stage-placement and projection tool for stage
technicians, production teams and designers.

It provides a real-size drawing workspace, multiple plans and a dedicated
projection output. Only the required markers are displayed on a black
background: positions, axes, shapes, labels, display groups and cues.

A permanent **BLACKOUT** control immediately cuts the projected image.

### Required hardware

- No projector is needed to draw and prepare a standalone `.stagemark` project.
- To make floor marks visible to the team, connect the computer to **one or more projectors**. Large stages, limited brightness or shadow reduction may require several projectors or mapping software.
- The StageMark AR technical preview offers a camera overlay on an [ARCore-compatible phone](https://developers.google.com/ar/devices), including Galaxy A54 5G, or [XREAL Air 2 Ultra](https://developer.xreal.com/) with [XREAL Beam Pro](https://www.xreal.com/beampro). Only the phone user or glasses wearer sees this overlay; it does not replace shared projection.

StageMark supplies the video image but does not power the projector on or off. The output starts black, **DISPLAY** is explicit and **BLACKOUT** remains the priority control.

### Typical workflow

1. Create a plan using the real stage dimensions.
2. Place objects and markers in millimetres.
3. Group the elements that must appear together.
4. Prepare several plans or display states.
5. Connect the projector and show the calibration pattern.
6. Align the four corners of the useful projection area.
7. Display only the required group during the stage change.
8. Trigger blackout as soon as the markers are no longer needed.

### Main features

- Real-size stage plans and persistent dimensions.
- Stage symbols, geometric shapes, text and custom objects.
- Multiple plans, layers and instant display groups.
- Reference background that is never projected by default.
- Separate projection window.
- Direct display output on Windows and macOS; Spout output on Windows only.
- Four-point calibration and test pattern.
- Permanent DISPLAY and BLACKOUT controls.
- Cue workflow, keyboard shortcuts and Stream Deck profiles.
- A4 plan export.
- Local phone, tablet or browser controller.
- Offline projector and lens catalogue.

StageMark 2027.0.5 also supports named native objects, touch
placement, selection by name, measurement editing, dragging and confirmed
deletion on a phone. Native locks remain effective. The direct QR and StageFlow
portal open the same editor; claiming control stays explicit and connecting
never starts projection.

By default, StageMark creates, opens and saves its own standalone
<code>.stagemark</code> projects. No other application is required. Opening a
shared <code>.stageflow</code> project is an additional workflow and StageFlow
remains entirely optional. The shared project can be used, in the canonical
suite order, with StageFlow, StageDesk, StageMark,
StageMon, Dante Config Editor and AutoCAD.

StageFlow LIVE detects new Patch and CAD revisions, but adopting one always
requires an explicit operator action, even while the editor is clean.
Local changes are never overwritten: StageMark reports a conflict for
the operator to resolve. LIVE following can never show an image, remove
**BLACKOUT**, change the projection display or recall a cue.

The **StageFlow connection** centre brings voluntary LIVE pairing and the existing
StageMark Remote together. Opening it starts no service or discovery.
Orange label-change notifications can be acknowledged on this workstation
only; later arrivals remain pending. StageFlow notification pause and local
reception are shown separately.

StageMark presence registration and local pipe commands are Windows-only.
On Mac, StageFlow can launch StageMark on a local project; joining LIVE remains
explicit inside StageMark. Local `.stageflow` projects, Network LIVE and the
Remote remain available on Mac.

### Download

**StageMark 2027.0.6 for Windows 11 x64, Intel Mac and Apple Silicon Mac** and **StageMark AR 0.1.1 build 12** are available. Codemagic built both DMGs from the same source tag as Windows; their SHA-256 hashes are verified.

- [Windows x64 — 2027.0.6](https://github.com/Mamat79/StageMark/releases/download/v2027.0.6/StageMark-2027.0.6-Setup.exe) · [SHA-256](https://github.com/Mamat79/StageMark/releases/download/v2027.0.6/StageMark-2027.0.6-Setup.exe.sha256)
- [Intel Mac — 2027.0.6](https://github.com/Mamat79/StageMark/releases/download/v2027.0.6/StageMark-2027.0.6-macOS-x64.dmg)
- [Apple Silicon Mac — 2027.0.6](https://github.com/Mamat79/StageMark/releases/download/v2027.0.6/StageMark-2027.0.6-macOS-arm64.dmg)
- [StageMark AR 0.1.1 build 12 — development APK](https://github.com/Mamat79/StageMark/releases/download/v2027.0.6/StageMark-AR-0.1.1-Development.apk) · [SHA-256](https://github.com/Mamat79/StageMark/releases/download/v2027.0.6/StageMark-AR-0.1.1-Development.apk.sha256)

Desktop packages and SHA-256 files are grouped in one stable Release. The APK
is debug-signed and remains a technical preview: software checks passed, but
physical accuracy, drift and relocalisation still require real phone and XREAL testing.

[Complete 2027.0.6 SHA-256 manifest](SHA256SUMS-2027.0.6-complete). Update Desktop for the reorganised workflow; APK build 12 updates the previous companion in place.

Companion **0.1.1 build 12** offers ARCore and XREAL, scrollable touch UI, accessible actions, separate settings and A/B/C calibration. **SHOW AR / HIDE AR** are independent of video; **hide for me** cannot override PC hide. Reusable marker sheets and an optional project placement PDF simplify setup. **Ctrl+Shift+F12** closes video/black curtain/Spout without quitting the project or stopping AR. Android 10+, ARM64 and ARCore support are required for phone mode; initial Google AR Services setup may need Internet. No camera recording/upload. [Workflow and limitations](RELEASE_NOTES_2027.0.6.md).

[StageMark 2027.0.6 release](https://github.com/Mamat79/StageMark/releases/tag/v2027.0.6).

**New workflow:** StageFlow connection contains network/remote tools; Outputs & setup contains video, AR and calibration. Live mode concentrates on plans, cues and visibility controls. Start AR creates the session and authorises marks in one action; pairing/calibration remain mandatory and the guided path is optional. APK 12 includes the native camera-input fix and removes fallback internal labels such as Cross. A cross and colour updates were observed on A54; physical accuracy, drift, relocalisation and XREAL remain to be qualified.

French and English manuals and common suite guides are included in the
application. The [guide manifest](guides/suite-guides-manifest.json) records
the exact common-guide sizes and checksums.

### Use and license

StageMark starts with 30 reminder-free days. Afterwards, the application and
all its features remain usable; only a startup reminder is displayed.

A permanent **€49 tax-included** one-time license removes this reminder.

**[Buy a permanent StageMark license](https://stagemark-license.mamat79-dce.workers.dev/buy)**

### Before a show

The current Windows installer is unsigned. The macOS disk images are not signed
with an Apple Developer ID and are not notarized, so Gatekeeper may display a
warning. The declared macOS minimum is 12. For 2027.0.6, the Apple Silicon package was smoke-tested on the M2 runner; Intel architecture was checked without a native Intel launch. Not every macOS release is qualified. Existing integrity signatures
are preserved; do not disable macOS protections. Always validate the projector,
calibration, output, blackout and controls with real hardware before a production.

---

<p align="center"><strong>SiLeMI/O · By Mamat----[]---</strong></p>
