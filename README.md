<p align="center">
  <img src="branding/stagemark-logo.png" width="520" alt="StageMark 2026">
</p>

<h1 align="center">StageMark 2026</h1>

<p align="center">
  <strong>Dessinez l’implantation. Calibrez la projection. Affichez uniquement les repères utiles.</strong><br>
  Hors ligne · Français / English · Windows 11 · macOS Intel / Apple Silicon
</p>

<p align="center">
  <a href="https://github.com/Mamat79/StageMark/releases/latest"><strong>⬇ Télécharger StageMark</strong></a>
  · <a href="guides/StageMark-Notice-FR.pdf">Notice FR</a>
  · <a href="guides/StageMark-Notice-EN.pdf">Guide EN</a>
  · <a href="guides/Guide-Suite-SiLeMIO-FR.pdf">Guide de la suite</a>
</p>

<p align="center">
  <a href="https://github.com/Mamat79/StageMark/releases/download/v2026.9.3/stagemark-presentation-fr.mp4"><img src="https://github.com/Mamat79/StageMark/releases/download/v2026.9.3/stagemark-presentation-fr-poster.png" width="820" alt="Présentation vidéo StageMark"></a><br>
  <a href="https://github.com/Mamat79/StageMark/releases/download/v2026.9.3/stagemark-presentation-fr.mp4">Présentation · FR</a>
  · <a href="https://github.com/Mamat79/StageMark/releases/download/v2026.9.3/stagemark-presentation-fr.vtt">Sous-titres FR</a>
  · <a href="https://github.com/Mamat79/StageMark/releases/download/v2026.9.3/stagemark-presentation-en.mp4">Presentation · EN</a>
  · <a href="https://github.com/Mamat79/StageMark/releases/download/v2026.9.3/stagemark-presentation-en.vtt">EN captions</a>
</p>

---

## StageMark, à quoi ça sert ?

StageMark est un outil de préparation et de projection destiné aux techniciens
de plateau, régisseurs, scénographes et équipes de production.

Il permet de dessiner une implantation en dimensions réelles, d’organiser
plusieurs plans et d’envoyer sur le plateau uniquement les repères nécessaires :
positions, axes, formes, textes, groupes d’affichage ou éléments de conduite.

La projection reste sur fond noir et un **BLACKOUT** permanent permet de couper
immédiatement l’image.

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

### Préparer le vidéoprojecteur

La banque intégrée aide à comparer des vidéoprojecteurs et objectifs pour la
préparation d’une location ou d’une installation : luminosité, poids, rapport
optique, orientation et informations utiles.

Le choix final et la calibration doivent toujours être validés avec le matériel
réel et les conditions du lieu.

## Le même projet que le patch et le plan technique

Par défaut, StageMark crée, ouvre et enregistre ses propres projets autonomes
<code>.stagemark</code>. Aucun autre logiciel n’est nécessaire. L’ouverture
d’un projet partagé <code>.stageflow</code> est un parcours supplémentaire et
StageFlow reste entièrement optionnel.

Il peut lire le patch commun, placer des sources sans les ressaisir et reprendre
un plan provenant de StageFlow ou d’AutoCAD.

Avec StageFlow LIVE, StageMark peut suivre automatiquement les nouvelles
révisions de patch et de plan CAD lorsque l’éditeur est propre. Les changements
locaux ne sont jamais écrasés : un conflit est signalé et reste à arbitrer. Ce
suivi ne peut jamais afficher une image, retirer le **BLACKOUT**, changer
l’écran de projection ou rappeler une cue.

~~~mermaid
flowchart LR
    SF["StageFlow<br/>Patch + plan"] <--> P[("Projet .stageflow")]
    SMT["StageDesk<br/>Save My Time"] <--> P
    SM["StageMark<br/>Implantation + projection"] <--> P
    MON["StageMon<br/>Matrice d’écoute live"] <--> P
    DCE["Dante Config Editor<br/>Réseau Dante"] <--> P
    CAD["AutoCAD<br/>Plan technique"] <--> P
~~~

- [StageFlow — patch, groupes, Excel et plan de scène](https://github.com/Mamat79/SiLeMIO-StageFlow-Distribution/releases/latest)
- [StageDesk — transfert entre consoles et logiciels](https://github.com/Mamat79/StageDesk/releases/latest) — sous-titre **Save My Time**
- [StageMark — implantation et projection scéniques](https://github.com/Mamat79/StageMark/releases/latest)
- [StageMon — matrice d’écoute live](https://github.com/Mamat79/StageMon/releases/latest)
- [Dante Config Editor — préparation Dante hors ligne](https://github.com/Mamat79/Dante-Config-Editor/releases/latest)
- [AutoCAD — plan technique et connecteur StageFlow](https://github.com/Mamat79/SiLeMIO-StageFlow-Distribution/releases/latest)

Chaque logiciel reste autonome. Vous installez uniquement les outils utiles à
votre production.

## Télécharger StageMark

La version stable actuelle est **StageMark 2026.9.3** pour Windows 11 x64,
macOS Apple Silicon et macOS Intel.

**[Télécharger la dernière version](https://github.com/Mamat79/StageMark/releases/latest)**

Les notices française et anglaise sont intégrées à l’application et accessibles
depuis le bouton **Aide**. Elles sont aussi disponibles directement :
[français](guides/StageMark-Notice-FR.pdf),
[English](guides/StageMark-Notice-EN.pdf) et
[guide de la suite](guides/Guide-Suite-SiLeMIO-FR.pdf).

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
- Direct output or Spout output on Windows.
- Four-point calibration and test pattern.
- Permanent DISPLAY and BLACKOUT controls.
- Cue workflow, keyboard shortcuts and Stream Deck profiles.
- A4 plan export.
- Local phone, tablet or browser controller.
- Offline projector and lens catalogue.

By default, StageMark creates, opens and saves its own standalone
<code>.stagemark</code> projects. No other application is required. Opening a
shared <code>.stageflow</code> project is an additional workflow and StageFlow
remains entirely optional. The shared project can be used, in the canonical
suite order, with StageFlow, StageDesk (subtitle: Save My Time), StageMark,
StageMon, Dante Config Editor and AutoCAD.

StageFlow LIVE can refresh Patch and CAD data automatically while the editor is
clean. Local changes are never overwritten: StageMark reports a conflict for
the operator to resolve. LIVE following can never show an image, remove
**BLACKOUT**, change the projection display or recall a cue.

### Download

The current stable release is **StageMark 2026.9.3** for Windows 11 x64,
macOS Apple Silicon and macOS Intel.

**[Download the latest StageMark release](https://github.com/Mamat79/StageMark/releases/latest)**

French and English guides are included in the application.

### Use and license

StageMark starts with 30 reminder-free days. Afterwards, the application and
all its features remain usable; only a startup reminder is displayed.

A permanent **€49 tax-included** one-time license removes this reminder.

**[Buy a permanent StageMark license](https://stagemark-license.mamat79-dce.workers.dev/buy)**

### Before a show

The current Windows installer is unsigned. The macOS disk images are not signed
with an Apple Developer ID and are not notarized, so Gatekeeper may display a
warning. Always validate the projector, calibration, output, blackout and
controls with the real hardware before a production.

---

<p align="center"><strong>SiLeMI/O · By Mamat----[]---</strong></p>
