# StageMark 2027.1.2 — livraison macOS / macOS delivery

## Français

Les DMG Intel et Apple Silicon ont été produits par Codemagic à partir de la même révision source que le paquet Windows 2027.1.2. Aucun ancien paquet n’a été renommé. La compilation déjà réussie a été récupérée sans être relancée. Electron reste à 43.7.7.

- Apple Silicon : `StageMark-2027.1.2-macOS-arm64.dmg`, 147673117 octets, SHA-256 `c7e63f7070a6136b85e425ddcac61a0e3080a6411e2d6e9fbea367a6e8a5f7ad`.
- Intel : `StageMark-2027.1.2-macOS-x64.dmg`, 151855222 octets, SHA-256 `2cc4a8175ff07c418ed4a878cf313f056824e299115cd7ff448ea967a6317ecf`.

Sur le runner Mac : 1085 tests Vitest réussis, 27 ignorés, 42 tests Node réussis. Le paquet Apple Silicon a été monté en lecture seule et exécuté nativement : renderer, commandes de sécurité, ouverture du projet StageFlow par CLI, projet inchangé, exports PDF et PNG vérifiés. Les notices FR/EN embarquées correspondent exactement aux notices publiées.

Limites : l’architecture Intel est vérifiée, sans exécution native Intel. Le décompte de cinq secondes pour un essai expiré n’a pas fait l’objet d’un scénario Mac natif dédié ; les tests de licence et d’interface ne valent pas recette manuelle Mac. Aucun essai terrain de téléphone, lunettes, projecteur, audio ou réseau entre deux PC n’est revendiqué. Les DMG ne sont ni signés Developer ID ni notarisés. La présence locale et les pipes de console restent réservés à Windows. Les 27 tests ignorés ne sont pas comptés comme réussis.

L’APK 0.1.1 build 18 est inchangée et reste disponible dans sa release existante. Les anciennes releases et conditions d’achat sont préservées.

## English

Intel and Apple Silicon DMGs were built by Codemagic from the same source revision as Windows 2027.1.2. No old package was renamed. The successful existing build was recovered without rebuilding. Electron remains at 43.7.7.

- Apple Silicon: `StageMark-2027.1.2-macOS-arm64.dmg`, 147673117 bytes, SHA-256 `c7e63f7070a6136b85e425ddcac61a0e3080a6411e2d6e9fbea367a6e8a5f7ad`.
- Intel: `StageMark-2027.1.2-macOS-x64.dmg`, 151855222 bytes, SHA-256 `2cc4a8175ff07c418ed4a878cf313f056824e299115cd7ff448ea967a6317ecf`.

On the Mac runner: 1085 Vitest tests passed, 27 skipped, 42 Node tests passed. The Apple Silicon package was mounted read-only and executed natively: renderer, safety controls, opening a StageFlow project through the CLI, unchanged project and PDF/PNG exports were verified. Bundled FR/EN manuals exactly match the published manuals.

Limits: Intel architecture was verified without native Intel execution. The expired-trial five-second countdown was not separately exercised by a dedicated native Mac scenario; licence and interface tests do not establish manual Mac acceptance. No physical phone, glasses, projector, audio or two-PC LAN acceptance is claimed. DMGs are not Developer ID signed or notarized. Local console presence and pipes remain Windows-only. The 27 skipped tests are not reported as passed.

APK 0.1.1 build 18 is unchanged and remains available in its existing release. Historical releases and purchase terms are preserved.
