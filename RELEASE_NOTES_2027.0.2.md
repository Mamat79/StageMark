# StageMark 2027 — corrective Windows 2027.0.2

**Windows x64 uniquement / Windows x64 only.**
Les téléchargements Mac restent en [v2027](https://github.com/Mamat79/StageMark/releases/tag/v2027).
Public Mac downloads remain on [v2027](https://github.com/Mamat79/StageMark/releases/tag/v2027).

## Français

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

- `StageMark-2027.0.2-Setup.exe` — **118 492 712 octets**.
- `StageMark-2027.0.2-Setup.exe.sha256` — fichier de contrôle de l’installeur.

SHA-256 de l’installeur :

```text
6FFD4E68D3C416D9FA6A77C80F765E2E01E74AE16071F51D478A70EB883C6F71
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

Les vérifications logicielles incluent 827 tests Vitest et 15 tests Node,
ainsi que des scénarios en navigateurs isolés. Elles ne constituent pas une
validation de deux PC physiques, d’un téléphone, du vidéoprojecteur, de la
latence du blackout ou de l’imprimante du spectacle : ces essais restent à
réaliser sur place. Les anciennes Releases restent disponibles. Aucun code
source produit ni donnée privée n’est publié dans le dépôt de distribution.

## English

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

This release contains the Windows x64 installer (**118,492,712 bytes**) and its
SHA-256 sidecar; the exact installer hash is shown above. Mac downloads remain
on v2027: [Intel](https://github.com/Mamat79/StageMark/releases/download/v2027/StageMark-2027-macOS-x64.dmg)
and [Apple Silicon](https://github.com/Mamat79/StageMark/releases/download/v2027/StageMark-2027-macOS-arm64.dmg).
Global “Latest” stays v2027. The corrected Windows updater in 2027.0.2 can
select separate Windows correctives; earlier Windows versions should use this
release's direct download.

Windows is unsigned. Existing Mac packages have no Apple Developer ID signature
or notarization; their integrity signatures are preserved and macOS protections
must not be disabled. Spout and StageMark local presence/pipe integration remain
Windows-only. Software and isolated-browser checks are not physical two-PC,
phone, projector, blackout-latency or printer acceptance. Validate the show’s
actual hardware on site. Previous releases remain available; no product source
or private data is included in the distribution repository.
