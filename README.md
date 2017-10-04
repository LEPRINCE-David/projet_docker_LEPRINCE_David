# projet_docker_LEPRINCE_David
Projet Cloud Infrastructure

#

Veiller à bien se placer à la racine de chaque partie avant de lancer *docker-compose build* puis *docker-compose up*

#

### 2.3 Partie Wordpress

Le docker-compose.yml construit une base de données et le nécessaire pour faire fonctionner Wordpress.

Un dossier db_data est créé et contiendra l'actuelle base de données.

```
Accès via localhost:8000
```

#

### 3. Partie Libre

Le docker-compose.yml construit une base de données et un serveur apache.

Comme dans la partie précédente, un dossier db_data est créé et contiendra l'actuelle base de données.

Le serveur est créé depuis une image sur le net mais on peut aussi le build avec le Dockerfile situé dans le dossier *apache*. Il suffit pour cela de supprimer la ligne contenant l'image, et de la remplacer par la ligne build en commentaire.

Le dossier web contient un fichier php simple que l'on peut modifier directement depuis l'host. Le lien est fait avec volumes dans le fichier .yml.

```
Accès via localhost:8080
```
