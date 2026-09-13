# StageMark macOS 2027.0.10

Codemagic a terminé la compilation Intel et Apple Silicon. Les deux DMG et leurs fichiers SHA-256 ont été téléchargés depuis la Release publique et comparés.

- Apple Silicon ARM64 : 146418172 octets, SHA-256 ecc32c4b1522512dcbee78fabe5fac56591256e6587c9a46f5167e2b8c9dc628.
- Intel x64 : 148525986 octets, SHA-256 a601c40925503c6299f446b2ff0ffa0316275776e10893177cc6d17d76cd2acc.
- Le paquet ARM64 a passé le contrôle d'exécution du pipeline sur Apple Silicon. Le paquet Intel a passé le contrôle d'architecture, sans lancement natif Intel.
- Pas de signature Apple Developer ID ni notarisation. Les essais physiques projecteur, téléphone, lunettes et réseau à deux PC restent nécessaires.
- Le suivi des groupes nécessite des mises à jour StageFlow/StageMon compatibles distinctes, non publiées dans cette livraison. Voir les notes 2027.0.10.

## English

Both Intel and Apple Silicon DMGs are available and their public downloads match the SHA-256 checksums above. Codemagic passed ARM64 runtime smoke tests and Intel architecture verification, not native Intel execution. No Developer ID signature or notarisation. No new projector, phone, glasses or two-PC hardware acceptance. Optional group following requires separate compatible StageFlow/StageMon updates, not released in this delivery.
