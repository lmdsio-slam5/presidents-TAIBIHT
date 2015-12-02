# Presidents

Projet Silex/MySQL pour le déploiement sur OpenShift

## Consignes d'installation

* Accepter [l'invitation Classroom for GitHub](https://classroom.github.com/assignment-invitations/f53e461faad9b5422b0283f9b5b0e5f9) pour obtenir le dépôt GitHub `presidents-VotreLogin`.
* Cloner ce dépôt dans le répertoire de travail de votre serveur Web local (exemple : `c:\xampp\htdocs` avec XAMPP pour Windows).
* Configurer Apache et le fichier `hosts` pour définir un hôte virtuel `presidents` (ET NON `presidents-VotreNom`) vers ce répertoire. Exemple avec XAMPP sous Windows :

```
<VirtualHost *:80>
    DocumentRoot "C:\xampp\htdocs\presidents-VotreLogin\web"
    ServerName presidents
    <Directory "C:\xampp\htdocs\presidents-VotreLogin\web">
        AllowOverride all
    </Directory>
</VirtualHost>
```

* Créer la base de données `presidents` à l'aide des scripts fournis.

* Télécharger les composants nécessaires avec la commande `composer install`.

* Tester l'application à l'URL http://presidents.


