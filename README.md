# Automobiles Etcetera — refonte immersive

Prototype d'un site vitrine immersif pour Automobiles Etcetera (Montréal) : showroom, club privé, entreposage et esthétique automobile.

## Contenu

- `index.html` : le site complet, en un seul fichier (HTML, CSS et JavaScript, sans dépendance à installer).
- `intro.mp4` : la vidéo d'introduction, pilotée par le scroll. Elle est encodée « toutes images clés » pour que chaque position s'affiche sans saccade.

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
