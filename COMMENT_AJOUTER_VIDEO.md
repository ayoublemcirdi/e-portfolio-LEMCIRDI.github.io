# Ajouter ta vidéo de présentation (portfolio V9)

Ton site fonctionne déjà, même sans vidéo. Dans ce cas, la page **Vidéo pitch** affiche un emplacement élégant « arrive bientôt ».

## MÉTHODE A — MP4 (la plus simple pour une courte vidéo)

1. Exporte ou convertis ta vidéo en **MP4 (H.264 + AAC)**, idéalement **1080p / 16:9**.
2. Renomme-la exactement **pitch.mp4** (sans majuscule).
3. Sur ton PC, place-la dans le dossier **assets** : `assets/pitch.mp4`.
4. Le fichier `video-config.js` est déjà réglé sur `source: "mp4"` et `mp4: "assets/pitch.mp4"`. **N'y touche pas.**
5. Sur GitHub, ouvre ton dépôt **ayoublemcirdi/e-portfolio-LEMCIRDI.github.io**, puis le dossier **assets**.
6. Clique sur **Add file → Upload files**, choisis `pitch.mp4`, puis valide avec **Commit changes**.
7. Ouvre `https://ayoublemcirdi.github.io/e-portfolio-LEMCIRDI.github.io/#/fr/pitch` et actualise (Ctrl + F5).

**Attention : GitHub limite l'upload depuis le navigateur à 25 Mio par fichier.** Si ta vidéo dépasse cette limite, préfère la méthode B (YouTube). Évite d'importer un fichier de plusieurs centaines de Mo dans ton dépôt.

## MÉTHODE B — YouTube non répertoriée (conseillée pour une grosse vidéo)

1. Sur YouTube Studio, importe ta vidéo ; choisis **Non répertoriée** (Unlisted) si tu ne veux pas qu'elle apparaisse dans les recherches.
2. Copie l'URL complète, par exemple `https://www.youtube.com/watch?v=XXXXXXXXXXX`.
3. Sur GitHub, ouvre **video-config.js** (à la racine du dépôt) et clique sur le **crayon / Edit this file**.
4. Modifie uniquement ces lignes :

```js
source: "youtube",
youtube: "https://www.youtube.com/watch?v=XXXXXXXXXXX"
```

5. Clique sur **Commit changes**. Sur le site, la vidéo s'affichera dans la page **Vidéo pitch**.
6. Ne mets pas ton MP4 dans `assets` si tu choisis cette méthode.

## Importer / mettre à jour cette VERSION sur GitHub

1. Décompresse l'archive `eportfolio-ayoub-v9-pitch-final.zip` sur ton ordinateur.
2. Ouvre `https://github.com/ayoublemcirdi/e-portfolio-LEMCIRDI.github.io`.
3. À la racine du dépôt (onglet **Code**), importe **index.html**, **video-config.js** et **.nojekyll** via **Add file → Upload files**. Si GitHub te signale des doublons, accepte leur remplacement.
4. Dans le dossier `assets`, ajoute les fichiers des CV du ZIP uniquement s'ils ne sont pas déjà présents. Conserve le dossier `assets` à la racine.
5. Valide avec **Commit changes**. Dans **Settings → Pages**, vérifie que `main` et `/(root)` sont choisis.
6. Ouvre l'adresse publique : `https://ayoublemcirdi.github.io/e-portfolio-LEMCIRDI.github.io/`.

> Important : n'importe qui visitant ton portfolio pourra consulter la vidéo, même si elle est « non répertoriée » sur YouTube. Vérifie également que tu es à l'aise avec la publication publique de ta photo et de tes coordonnées.

## Contrôles finaux

- Accueil → bouton **Voir ma vidéo / Watch my video** → page Vidéo pitch.
- Menu **Vidéo pitch / Video pitch** → même page.
- Contact → bouton **Voir ma vidéo de présentation** → même page.
- FR / EN : les deux langues fonctionnent sur la même page.
- CV français, CV anglais et TIPE accessibles depuis le site.

## Petit conseil pour le pitch

Une vidéo de **60 à 90 secondes** suffit généralement : présente-toi, raconte ton parcours à ENSEEIHT, tes projets techniques, puis ce qui te motive en Big Data / IA et pour une mobilité à l'international. Tu peux faire la vidéo en anglais et conserver la page en français et en anglais.
