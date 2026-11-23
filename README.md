# site-mariage

Le site du mariage de Laly &amp; Vincent — 1er mai 2027, Domaine du Prieuré Saint Pierre (Montjoyer).

Page statique unique (`index.html` + dossier `assets/`), sans dépendance externe (polices auto-hébergées). Programme, infos pratiques, RSVP, FAQ, et une galerie photo accessible via un lien Google Drive.

## Aperçu en local

Ouvrez simplement `index.html` dans un navigateur, ou servez le dossier avec n'importe quel serveur statique.

## Hébergement (GitHub Pages)

Dans les réglages du dépôt : **Settings → Pages**, source **Deploy from a branch**, branche `main`, dossier `/ (root)`. Le site sera ensuite disponible à une adresse du type `https://vincentmatray-69600.github.io/site-mariage/`.

## À modifier vous-même après le mariage

Dans `index.html`, tout en bas du fichier, une variable est prévue pour ça :

```js
var DRIVE_URL = "#"; // remplacez "#" par le lien Google Drive de l'album
```

- `DRIVE_URL` : le lien vers l'album Google Drive une fois les photos disponibles. Tant qu'il vaut `"#"`, le site affiche un message d'attente à la place du bouton.

Le lien RSVP (`href` de la section RSVP) et le lien vers l'album pour les FAQ/mentions légales peuvent être modifiés directement dans le HTML si besoin.
