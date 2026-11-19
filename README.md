# Automobiles Etcetera — refonte immersive

Prototype d'un site vitrine immersif pour Automobiles Etcetera (Montréal) : showroom, club privé, entreposage et esthétique automobile.

## Contenu

- `index.html` : le site complet, en un seul fichier (HTML, CSS et JavaScript, sans dépendance à installer).
- `assets/video/intro.mp4` : la vidéo d'introduction, pilotée par le scroll. Elle est encodée « toutes images clés » pour que chaque position s'affiche sans saccade.
- `assets/images/intro-poster.jpg` : l'image affichée pendant le chargement de la vidéo.

## Voir le site

Ouvrir `index.html` dans un navigateur. Pour un test plus proche de la mise en ligne, lancer un petit serveur local :

```
python3 -m http.server 8000
```

puis aller sur http://localhost:8000.

## Effets

- Intro : la Ferrari sort de l'allée au rythme du scroll, puis zoom caméra.
- Défilement amorti à la molette et au trackpad.
- Compteur de vitesse (0 à 330 km/h) sur la voiture vedette.
- Indicateur de rapport engagé sur le côté, un rapport par section.
- Chargement en voyants de passage de rapport.
- Services en défilement horizontal, Le Club en masque qui s'ouvre, cartes 3D pour l'inventaire.

Les photos des voitures sont chargées depuis automobilesetcetera.com.

## Rangement des fichiers

```
index.html                     le site
assets/                        tout ce que le site charge
  video/intro.mp4              vidéo de l'intro (1920 px, toutes images clés)
  images/intro-poster.jpg      image d'attente de l'intro
  audio/intro.mp3              son de l'intro (pas encore branché sur le site)
  audio/intro-audio.js         le même son, intégré en JavaScript
archives/                      tout le reste, gardé pour ne rien perdre
  videos-sources/              vidéos d'origine de l'intro (4K et 480p)
  intro-images/                les 121 images de l'ancienne intro image par image
  captures/                    captures d'écran des versions du site
  maquettes/                   maquettes des idées d'intro (page + images)
  references/                  images de référence envoyées pendant le travail
outils/scroll-video.html       modèle réutilisable de vidéo au scroll
```

Les photos des voitures et des sections (Le Club, Services, Inventaire) ne sont pas dans le dépôt : elles sont chargées directement depuis automobilesetcetera.com.
