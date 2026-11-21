ISOMETRIC SCANNER — PROTOTYPE WEB v0.3

Nouveautés : affichage PDF avec PDF.js, navigation entre pages, tracé manuel d’un rectangle de repérage pour le spool sélectionné, sauvegarde locale des zones (localStorage), export JSON.

Utilisation : décompresser le ZIP, ouvrir index.html dans Safari/Chrome/Edge, importer le PDF, choisir un spool, cliquer « Définir la zone du spool » et tracer le rectangle sur le plan. Exporter les zones JSON pour les conserver ou les transférer.

Connexion Internet requise pour charger PDF.js depuis cdnjs.

Limites : rectangles MANUELS, pas de détection automatique des limites physiques. Les zones doivent être vérifiées sur le plan. Les 22 repères sont préchargés selon le relevé initial. Calculs de tubes indicatifs sur hypothèse SCH40 ; accessoires non inclus dans les totaux. Supports exclus ; peinture sur acier extérieur avant isolation. Pas de serveur ni base de données ; sauvegarde locale au navigateur courant.


CORRECTIF v0.3.1 (iPhone / Safari)
- Lecture du fichier local via FileReader puis transmission des octets PDF à PDF.js.
- Évite le chargement direct du fichier local via une URL blob, qui peut échouer selon Safari.
- En cas d'échec, affiche désormais le détail de l'erreur au lieu d'un message générique.
- PDF.js reste chargé depuis CDN : une connexion Internet est nécessaire.
