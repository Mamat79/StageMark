# StageMark 2026 — distribution officielle

Ce dépôt distribue uniquement les installateurs vérifiés de **StageMark 2026**.
Le code source, les outils d’émission de licences et les secrets de publication
restent dans un dépôt privé séparé.

Le dépôt est lui-même **privé pendant la préparation du logiciel**. Il pourra
devenir public au lancement sans déplacer les Releases ni modifier les liens de
mise à jour intégrés à StageMark.

## État actuel

- dernière version stable : `2026.4` ;
- Windows 11 x64 : disponible dans la Release `v2026.4` ;
- macOS Apple Silicon et Intel : packaging en préparation, non publié à ce jour ;
- licence commerciale : préparation technique en cours, aucune vente active.

Chaque installateur est accompagné de son fichier SHA-256. Les binaires sont
publiés comme assets de Release et ne sont jamais ajoutés à l’historique Git.

## Licence prévue

StageMark proposera 30 jours d’essai sans rappel. Après cette période,
l’application restera entièrement utilisable et affichera uniquement un rappel
refermable. Une licence permanente à **49 € TTC**, en paiement unique, supprimera
ce rappel et restera valable sous Windows, macOS et après les mises à jour.

Le paiement sera traité hors de l’application par Stripe. Le code reçu sera
validé localement et hors ligne ; StageMark ne recevra aucune donnée bancaire.
La boutique n’est pas encore activée.

## Banque de vidéoprojecteurs

La banque distribuable se trouve dans [`projector-catalog/`](projector-catalog/README.md).
Une fiche ou un visuel n’est accepté qu’après contrôle de sa source et de son
droit de redistribution.

---

# StageMark 2026 — official distribution

This repository contains only verified **StageMark 2026** installers. Source
code, license-issuing tools, and publication secrets remain in a separate
private repository.

The distribution repository is also **private while the application is being
prepared**. It may become public at launch without moving Releases or changing
the update URLs embedded in StageMark.

- latest stable version: `2026.4`;
- Windows 11 x64: available in Release `v2026.4`;
- macOS Apple Silicon and Intel: packaging in progress, not released yet;
- commercial licensing: technical preparation only, no active sales.

The planned trust-based license provides a 30-day reminder-free trial. The app
will remain fully usable afterwards, with a dismissible reminder only. A
permanent **€49 including tax** one-time license will remove that reminder and
remain valid on Windows, macOS, and future compatible updates.

