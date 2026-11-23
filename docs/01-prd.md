# PRD — Site du mariage de Laly & Vincent

## Résumé

Site web statique, en une seule page, qui centralise toutes les informations du mariage de Laly et Vincent (1er mai 2027, Domaine du Prieuré Saint Pierre, Montjoyer) pour éviter aux invités de poser des questions répétées.

## Utilisateurs

- **Invités** : consultent le site via le lien partagé par les mariés. Aucune connexion, aucun compte.
- **Laly & Vincent** : seuls éditeurs du site. Ils modifient directement le code source (pas d'interface d'administration).

## Fonctions

| Fonction | Ce qu'elle fait | État |
|---|---|---|
| Compte à rebours | Affiche en direct le temps restant avant le 1er mai 2027 15h00 | Terminé |
| Ajout à l'agenda | Bouton qui ouvre Google Calendar pré-rempli avec l'événement | Terminé |
| Programme | Détaille les horaires du samedi (rendez-vous église, cérémonie, retour au domaine, vin d'honneur, dîner, dessert, soirée) et du dimanche (brunch & piscine) | Terminé |
| Infos pratiques du lieu | Parking, hébergement sur place, transport, liste de logements à proximité (campings avec coordonnées, mention Airbnb), liens d'itinéraire Google Maps | Terminé |
| Dress code | Présente une palette de couleurs pastel (bleu, vert, jaune) ; précise d'éviter le blanc et le noir | Terminé |
| RSVP | Bouton qui renvoie vers un formulaire Google Forms externe | Terminé |
| Cadeaux | Indique l'absence de liste de mariage et la présence d'une boîte sur place | Terminé |
| FAQ | Répond à 6 questions fréquentes (enfants, horaire d'arrivée, pluie, allergies, parking, musique) | Terminé |
| Galerie photo | Lien direct vers un album Google Drive ; aucun code d'accès requis | **En attente** — le bouton et l'état "en attente" sont fonctionnels, mais le lien (`DRIVE_URL`) est un placeholder tant que les photos du mariage ne sont pas disponibles. La fonction sera considérée terminée une fois ce lien renseigné. |
| Contact | Numéros de téléphone de Laly et Vincent, cliquables (`tel:`) | Terminé |
| Mentions légales & confidentialité | Informe sur la nature privée du site et l'absence de collecte de données propre au site | Terminé |
| Référencement (SEO) | Rend le site trouvable sur une recherche du type "mariage Laly et Vincent" : balises meta, données structurées (Event, FAQPage), sitemap, vérification Google Search Console | Terminé |

## Hors périmètre

- Le site ne stocke et n'affiche aucune réponse RSVP : les réponses existent uniquement dans le Google Form externe, consultable via le compte Google des mariés.
- Pas de compte invité, pas de connexion, pas d'espace personnalisé par invité.
- Pas d'interface d'administration : toute modification passe par l'édition du code source.
