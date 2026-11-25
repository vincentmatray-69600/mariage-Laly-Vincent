# App Flow — Site du mariage de Laly & Vincent

Site à page unique. Les "pages" ci-dessous sont des sections ancrées de cette même page, atteintes par clic sur la nav ou défilement.

## Navigation globale

- Barre de navigation fixe en haut, visible sur toutes les sections.
- Liens : Programme, Le lieu, Dress code, RSVP, Cadeaux, FAQ, Photos, Contact.
- Clic sur un lien → défilement fluide vers la section correspondante (`#id`).
- Clic sur "L & V" (logo) → retour à `#accueil`.

## `#accueil` — Accueil

- Photo du couple, prénoms, date, compte à rebours en direct (jours/heures/minutes/secondes). Une fois le mariage commencé (1er mai 15h00), affiche "C'est le grand jour !" à la place ; à partir du 3 mai, affiche "Merci !".
- Clic sur **"Ajouter au calendrier — Google"** → ouvre Google Calendar pré-rempli, dans un nouvel onglet (sortie du site).
- Clic sur **"Ajouter au calendrier — Apple"** → télécharge/ouvre un fichier `.ics` (assets/mariage-laly-vincent.ics) avec les mêmes informations, pour Apple Calendar et tout autre client compatible.

## `#programme` — Programme

- Deux cartes : Samedi 1er mai (rendez-vous église, cérémonie, retour au domaine & photos de groupe, vin d'honneur, dîner, dessert, soirée) et Dimanche 2 mai (brunch & piscine).
- Pas d'élément cliquable dans cette section.

## `#lieu` — Le lieu & infos pratiques

- Photo du domaine, infos parking/hébergement/transport, liste de logements à proximité (campings) + mention Airbnb.
- Clic sur **"Itinéraire — Église de Valaurie"** → ouvre Google Maps, nouvel onglet (sortie du site).
- Clic sur **"Itinéraire — Domaine de Montjoyer"** → ouvre Google Maps, nouvel onglet (sortie du site).
- Clic sur un numéro de téléphone de camping → ouvre l'application téléphone (`tel:`).

## `#dresscode` — Dress code

- Texte + 3 pastilles de couleur (bleu, vert, jaune pastel).
- Pas d'élément cliquable.

## `#rsvp` — RSVP

- Clic sur **"Répondre au RSVP"** → ouvre le Google Form externe, nouvel onglet (sortie du site).

## `#cagnotte` — Cadeaux

- Texte uniquement (pas de liste de mariage, boîte sur place).
- Pas d'élément cliquable.

## `#faq` — Questions fréquentes

- 6 questions/réponses affichées en liste (pas d'accordéon, tout est visible).
- Pas d'élément cliquable.

## `#photos` — Galerie photo

- Pas de code d'accès : accès direct par lien.
  - **Lien renseigné (`DRIVE_URL`)** → bouton **"Voir les photos"** visible → ouvre l'album Google Drive externe, nouvel onglet (sortie du site). *(État non encore actif — lien en attente, cf. PRD.)*
  - **Lien non renseigné** → le bouton est masqué, affiche à la place "Merci ! L'album sera mis en ligne juste après le mariage." *(État actuel du site.)*

## `#contact` — Une question ?

- Clic sur "Laly — 06 26 21 20 26" ou "Vincent — 07 60 64 50 73" → ouvre l'application téléphone (`tel:`).
- Clic sur "Mentions légales" → défilement vers `#mentions-legales`.
- Clic sur "Politique de confidentialité" → défilement vers `#confidentialite`.

## `#mentions-legales` et `#confidentialite`

- Texte uniquement.
- Clic sur "↑ Retour en haut" → défilement vers `#accueil`.

## Page d'erreur (`404.html`)

- Affichée automatiquement par GitHub Pages pour toute adresse qui ne correspond à rien (faute de frappe, lien cassé).
- Redirige immédiatement vers l'accueil (`/`), avec un lien de secours si la redirection automatique ne se déclenche pas.
