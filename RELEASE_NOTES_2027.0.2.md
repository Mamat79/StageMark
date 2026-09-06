# StageMark 2027 — corrective Windows 2027.0.2

**Windows x64 uniquement / Windows x64 only.**
Les téléchargements Mac restent en [v2027](https://github.com/Mamat79/StageMark/releases/tag/v2027).
Public Mac downloads remain on [v2027](https://github.com/Mamat79/StageMark/releases/tag/v2027).

## Français

**Paquet Windows remplacé le 6 septembre 2026, même version 2027.0.2.**
Révision produit : `3bcc68c`. Les anciens tags sont conservés ; le nouveau build
est identifié par son empreinte ci-dessous. Si StageMark est déjà en 2027.0.2,
l’updater ne proposera pas ce lot comme une version supérieure : télécharger
et lancer explicitement le nouvel installeur, après sauvegarde et fermeture.

- Édition mobile enrichie : création nommée des formes natives, placement au toucher ou au centre, sélection par nom ou sur le dessin, mesures, déplacement coalescé et suppression confirmée. Les formes libres mobiles utilisent des segments droits ; la Plume/Bézier avancée reste sur le PC.
- Les verrous natifs, le plan cible et une modification concurrente sont vérifiés avant édition. Un geste continu conserve une étape d’historique. Le QR direct et le portail StageFlow utilisent le même éditeur et les mêmes droits ; la prise de contrôle reste explicite.
- Connexions clarifiées sans réorganiser le centre : sessions disponibles sur ce PC ou le réseau local, LIVE local actif, télécommande arrêtée ou active, lien privé copiable. Connexion, droit de piloter et diffusion sont indépendants.

- Télécommande ouverte depuis StageFlow : la présence reste renouvelable tant que l’accès est actif et autorisé, sans coupure systématique après cinq minutes. L’inactivité, la révocation ou la fin de session invalident l’accès ; une autorisation expirée ne peut pas être réactivée par renouvellement. Aucune prise de contrôle ou commande de projection n’est déclenchée implicitement.
- Les mises à jour sont désormais choisies parmi les Releases stables compatibles avec le système et l’architecture, indépendamment de la Release globale « Latest ». Aucun retour vers une version plus ancienne n’est proposé ; téléchargement et installation restent explicites, avec contrôle SHA-256.
- Bandeau SiLeMIO harmonisé : Connexion StageFlow, état textuel, alertes séparées, thème actuel, FR/EN, Guide et Aide. Les commandes AFFICHER et BLACKOUT restent directement accessibles.
- Le centre de connexion distingue clairement les projets locaux autonomes et la connexion volontaire à une Session StageFlow LIVE. Les noms complets et détails techniques sont consultables sans démarrer de service.
- L’écran Installation propose des accès directs à la calibration, au choix de la sortie et à la configuration de la télécommande. Les contrastes de la calibration et du sélecteur de thème ont été corrigés en thème clair.
- Notices StageMark FR/EN actualisées et guides communs SiLeMIO 2027.2 embarqués à l’identique, avec leur manifeste d’empreintes.

La marque reste **StageMark 2027** et le raccourci officiel **StageMark v2027**.
Le numéro technique de cette corrective est **2027.0.2**. Le logo officiel est
conservé, y compris l’icône séparée du raccourci Windows.

Projets, banques, préférences, profils de calibration et licences existantes
restent compatibles. Aucun changement du prix, des clés de licence, du Control
Hub ni de la géométrie en millimètres entiers. La sortie démarre noire et le
BLACKOUT demeure prioritaire ; aucune révision LIVE n’est adoptée automatiquement.

### Plateformes et vérification

Cette Release Windows contient deux fichiers :

- `StageMark-2027.0.2-Setup.exe` — **118 500 658 octets**.
- `StageMark-2027.0.2-Setup.exe.sha256` — fichier de contrôle de l’installeur.

SHA-256 de l’installeur :

```text
82D1B252A7AFA8384600F3E307F81B6340B51184E7B552C798F6C4E6C4B2BF88
```

Les paquets Mac existants ne sont pas remplacés par cette corrective Windows :
[Intel](https://github.com/Mamat79/StageMark/releases/download/v2027/StageMark-2027-macOS-x64.dmg)
et [Apple Silicon](https://github.com/Mamat79/StageMark/releases/download/v2027/StageMark-2027-macOS-arm64.dmg).
La Release globale « Latest » reste v2027. L’updater Windows corrigé à partir
de 2027.0.2 peut choisir les correctives Windows séparées ; les versions
Windows précédentes doivent utiliser le téléchargement direct de cette Release.

L’installeur Windows est non signé Authenticode. Les Mac existants ne possèdent
pas de signature Apple Developer ID ni de notarisation ; leurs signatures
d’intégrité restent conservées et les protections macOS ne doivent pas être
désactivées. Spout et l’intégration locale de présence/pipes StageMark restent
spécifiques à Windows.

Les vérifications logicielles incluent 857 tests Vitest et 15 tests Node,
trois parcours mobiles isolés dont deux handoffs avec le vrai producteur
StageFlow, et la comparaison de 71 fichiers runtime et 117 fichiers du paquet
Windows. Les notices FR/EN (12 pages chacune) sont rendues et relues.
La restauration du snapshot natif est testée, pas le bouton Undo dans Electron
installé. Ces contrôles ne constituent pas une
validation de deux PC physiques, d’un téléphone, du vidéoprojecteur, de la
latence du blackout ou de l’imprimante du spectacle : ces essais restent à
réaliser sur place. Les anciennes Releases restent disponibles. Aucun code
source produit ni donnée privée n’est publié dans le dépôt de distribution.

## English

**Windows files replaced on 6 September 2026, retaining version 2027.0.2.**
Product revision: `3bcc68c`. Existing tags remain intact; the new build is
identified by the checksum above. An installation already on 2027.0.2 will not
offer this as a newer version: explicitly download and run the replacement
after saving and closing the app.

- Expanded mobile editor: named native objects, touch/centre placement, selection by name or on the drawing, measurements, coalesced dragging and confirmed deletion. Mobile free shapes use straight segments; advanced Pen/Bézier editing stays on the PC.
- Native locks, the target plan and concurrent changes are checked before editing. A continuous drag uses one history step. The direct QR and StageFlow portal use the same editor and privileges; claiming control remains explicit.
- The existing centre distinguishes available sessions on this PC or the LAN, active local LIVE and stopped/active remotes, with a copyable private link. Connection, pilot rights and output are separate states.

- StageFlow handoff access remains renewable while active and authorized, avoiding a fixed five-minute interruption. Idle, revoked or ended sessions cannot be resurrected by renewal. Opening or renewing access never implicitly claims control or issues projection commands.
- Update checks select the newest complete stable release for the current OS and architecture independently of global “Latest”, without offering downgrades. Download and installation remain explicit, with SHA-256 verification.
- The shared SiLeMIO header provides StageFlow connection and textual state, separate alerts, current theme, FR/EN, Guide and Help. SHOW and BLACKOUT remain directly accessible.
- The connection centre clearly separates autonomous local projects from voluntary StageFlow LIVE pairing. Full project names and technical details are available without starting a service.
- Installation adds direct links to calibration, display/output selection and remote setup. Light-theme contrast is corrected for calibration and the current-theme selector.
- Updated French/English StageMark manuals and unchanged canonical SiLeMIO 2027.2 guides are included with their checksum manifest.

Branding remains **StageMark 2027**, with the permanent **StageMark v2027**
shortcut and official icon. This corrective's technical version is **2027.0.2**.
Existing projects, catalogues, preferences, calibration profiles and licences
remain compatible. Price, licence keys, Control Hub and integer-millimetre
geometry are unchanged. Output starts black; BLACKOUT retains priority and
LIVE revisions still require explicit operator adoption.

This release contains the Windows x64 installer (**118,500,658 bytes**) and its
SHA-256 sidecar; the exact installer hash is shown above. Mac downloads remain
on v2027: [Intel](https://github.com/Mamat79/StageMark/releases/download/v2027/StageMark-2027-macOS-x64.dmg)
and [Apple Silicon](https://github.com/Mamat79/StageMark/releases/download/v2027/StageMark-2027-macOS-arm64.dmg).
Global “Latest” stays v2027. The corrected Windows updater in 2027.0.2 can
select separate Windows correctives; earlier Windows versions should use this
release's direct download.

Windows is unsigned. Existing Mac packages have no Apple Developer ID signature
or notarization; their integrity signatures are preserved and macOS protections
must not be disabled. Spout and StageMark local presence/pipe integration remain
Windows-only. Checks include 857 Vitest and 15 Node tests, three mobile paths
(both handoffs use the real StageFlow producer), exact runtime/installer contents
and both 12-page manuals. Native snapshot restoration is tested, not the installed
Electron Undo button. Software and isolated-browser checks are not physical two-PC,
phone, projector, blackout-latency or printer acceptance. Validate the show’s
actual hardware on site. Previous releases remain available; no product source
or private data is included in the distribution repository.
