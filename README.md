CHERRY LINE — correctif ciblé final

Contient app.js, index.html et styles.css issus de la version consolidée, avec deux corrections ciblées :
1. Average Rob : le conteneur 9:16 et l’iframe sont superposés dans une seule boîte, sans espace résiduel sous la vidéo.
2. Sport Content 1 : l’embed utilise le lien YouTube Shorts déjà communiqué pour cette vidéo (ID ZQB1K4hWO2s), au lieu de l’ancien ID.

Installation : remplacer ces trois fichiers dans le dépôt existant. Conserver le dossier Media/ avec son M majuscule et tous ses fichiers.

Contrôles effectués : syntaxe JavaScript avec node --check, présence des chemins Media/ et intégrité ZIP. La lecture en direct doit encore être vérifiée sur le site publié, car elle dépend aussi de la disponibilité/permissions du lecteur YouTube.
