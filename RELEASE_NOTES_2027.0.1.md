# StageMark 2027 — corrective Windows 2027.0.1

**Windows x64 uniquement / Windows x64 only.**
Les versions Mac publiques restent en [v2027](https://github.com/Mamat79/StageMark/releases/tag/v2027).
Public Mac downloads remain on [v2027](https://github.com/Mamat79/StageMark/releases/tag/v2027).

## Français

- Télécommande plus fiable : statut connecté conservé, observateur sans accès aux commandes, aucune action implicite à la prise de contrôle, erreurs visibles et reconnexion volontaire après coupure. Les confirmations et actions en attente sont annulées ; un événement retardé ne réactive pas le pilotage.
- Commandes différées protégées contre l’expiration, le changement de projet/session et le blackout. MIDI : relâchements et répétitions filtrés, retour dès le premier démarrage, ancien port détaché et reprise explicite. Les cues acceptent aussi un rang à partir de 1 ; une cible absente ne simule plus un succès.
- Interopérabilité StageFlow : présence LIVE réseau sans faux chemin local et délais/ACK tardifs alignés sur le maître. Les essais croisés ont utilisé le vrai moteur HTTP, avec projet synthétique et effets en mémoire uniquement.
- Notices FR/EN précisées : choix du paquet Windows, Mac Intel ou Apple Silicon, minimum macOS déclaré et distinction entre contrôles logiciels et recette sur le matériel réel.
- Guides communs SiLeMIO corrigés et inclus à l’identique, avec leur manifeste d’empreintes. Ils distinguent projet autonome, Projet StageFlow local et Session StageFlow LIVE, ainsi que les disponibilités et limites propres à chaque plateforme.
- L’aide de l’écran Installation renvoie désormais correctement le téléphone vers **Connexions**.
- Raccourci permanent **StageMark v2027** et logo officiel conservés. La marque reste StageMark 2027 ; le numéro technique de cette corrective est 2027.0.1.

Aucun changement des formats projet, de la géométrie métrique, des profils de
calibration ni des licences existantes. Le BLACKOUT reste prioritaire.
Chaque nouvelle révision LIVE reste soumise à une adoption explicite de
l’opérateur, même si le dessin ne contient aucune modification locale.

### Plateformes et limites

Cette Release contient uniquement l’installeur Windows x64 2027.0.1 accepté
et son fichier SHA-256. Windows 11 x64 est la plateforme de référence vérifiée.
L’EXE fait **118 486 867 octets** ; son SHA-256 est :

```text
3422A48EF0A4162F3D510C3949186146D15249E802139B6B0E1C9849E7A7EB20
```

Les DMG 2027.0.1 restent non publiés tant que leur recette visuelle n’est pas
acceptée. Les téléchargements Mac restent en version 2027 :
[Intel](https://github.com/Mamat79/StageMark/releases/download/v2027/StageMark-2027-macOS-x64.dmg)
et [Apple Silicon](https://github.com/Mamat79/StageMark/releases/download/v2027/StageMark-2027-macOS-arm64.dmg).
La Release commune « Latest » reste donc volontairement v2027 ; cette corrective
Windows est disponible en téléchargement direct, sans modification de l’updater.

Spout 2 et l’intégration de présence/pipes locale StageMark sont Windows-only.
La projection directe, les projets locaux, le LIVE réseau et la télécommande
web sont proposés sur les deux plateformes. Les paquets Mac n’ont pas de
signature Apple Developer ID ni de notarisation ; les signatures d’intégrité
existantes sont préservées et les protections macOS ne doivent pas être
désactivées. L’installeur Windows n’est pas signé numériquement.

Réseau à deux ordinateurs physiques, téléphone, vidéoprojecteur, latence de
blackout et imprimante restent à valider sur le matériel du spectacle.
Les anciennes Releases sont conservées. Aucun code source ni donnée privée
n’est inclus dans cette distribution.

## English

- More reliable remote: stable connected status, read-only observers, no implicit action when taking control, visible errors and manual reconnection. Pending confirmations/actions are cancelled; late events cannot reactivate control.
- Delayed commands are guarded against expiry, changed project/session and blackout. MIDI now filters releases and held repeats, returns feedback from the first start and detaches old inputs with explicit restart. Cues also accept one-based positions; missing targets no longer report success.
- StageFlow interoperability: pathless network LIVE presence and command deadlines/late acknowledgements aligned with the host. Cross-checks used the real HTTP engine with synthetic projects and memory-only effects.
- French and English manuals clarify Windows, Intel Mac and Apple Silicon packages, the declared macOS minimum and the difference between software checks and on-site hardware acceptance.
- Corrected canonical SiLeMIO suite guides are bundled unchanged with their checksum manifest. They distinguish standalone projects, Local StageFlow projects and StageFlow LIVE sessions, and state platform-specific availability and limits.
- The Installation screen now directs phone access to **Connections**.
- The permanent **StageMark v2027** shortcut and official logo are unchanged. Branding remains StageMark 2027; this corrective's technical version is 2027.0.1.

Project formats, integer-millimetre geometry, calibration profiles and existing
licences are unchanged. BLACKOUT remains the priority. Every later
LIVE revision still requires explicit operator adoption, even when the drawing
has no unsaved local changes.

This release contains only the accepted Windows x64 2027.0.1 installer and its
SHA-256 sidecar. Windows 11 x64 is the verified reference. The EXE is
**118,486,867 bytes**; its exact SHA-256 is shown above.

The 2027.0.1 DMGs remain unpublished pending visual acceptance. Public Mac
downloads remain on v2027: [Intel](https://github.com/Mamat79/StageMark/releases/download/v2027/StageMark-2027-macOS-x64.dmg)
and [Apple Silicon](https://github.com/Mamat79/StageMark/releases/download/v2027/StageMark-2027-macOS-arm64.dmg).
The shared “Latest” release deliberately remains v2027 to preserve Mac updates;
this Windows corrective is available by direct download, without changing the updater.

Spout 2 and StageMark local presence/pipe integration are Windows-only. Direct
display output, local projects, network LIVE and the web remote are offered
on both platforms, with the versions stated above.

Windows is unsigned. Mac packages have no Apple Developer ID signature or
notarization; existing integrity signatures are preserved and macOS protections
must not be disabled. Two-computer LAN, phone, projector, blackout latency and
printer checks remain on-site work. Previous Releases remain available; no
application source or private data is distributed.
