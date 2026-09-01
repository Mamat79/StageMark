# StageMark 2026.8

Cette version ajoute le suivi en lecture seule des sessions StageFlow LIVE V1
pour maintenir le patch et le fond CAD de StageMark à jour pendant la
préparation d'un spectacle.

- Une session LIVE compatible est détectée automatiquement dans le projet
  `.stageflow`, sans créer ni modifier la session ou son verrou.
- Lorsque le suivi est activé et que l'éditeur est propre, les révisions
  natives compatibles peuvent être adoptées automatiquement après une
  validation complète de la session et du cache courant.
- En présence de modifications locales, StageMark signale un conflit LIVE et
  ne remplace rien. L'opérateur conserve la maîtrise de ses changements.
- Le suivi est activable ou désactivable dans l'interface et son état reste
  visible : connecté, disponible mais désactivé, autonome ou en conflit.
- Une session absente, expirée, invalide ou étrangère laisse StageMark en mode
  autonome, sans bloquer le travail hors ligne.
- Une actualisation LIVE ne peut jamais afficher l'image, retirer le BLACKOUT,
  changer l'écran de projection, rappeler une cue ni envoyer quoi que ce soit
  vers la projection.

StageFlow reste gratuit et optionnel. StageMark continue de créer,
ouvrir et enregistrer directement les projets `.stageflow` sans dépendre de
l'application StageFlow.

Cette Release contient l'installateur Windows x64
`StageMark-2026.8-Setup.exe` et son fichier de contrôle SHA-256. Le numéro
technique complet, `2026.8.0`, reste consultable dans À propos ; l'identité
affichée dans l'application demeure StageMark 2026.

Aucun paquet macOS 2026.8 n'est publié sans construction, signature,
notarisation et recette sur Mac.
