Application web de gestion d'un dispensaire basée sur React, Redux, Redux-Form et Django

Fonctionnement général:

    Le serveur principal fonctionne sur localhost:8000 après la compilation du projet.
    localhost:3000 ne sert qu'à afficher l'interface du frontend.

Objectifs:

    Permettre à un dispensaire de collecter efficacement les données de ses patients via un portail d'enregistrement, afin de gérer et de suivre correctement leur état.
    Aider la direction de l'hôpital à superviser les différents services et à gérer son personnel.

Sécurité:

    Les portails d'inscription et de connexion ne sont normalement accessibles qu'au personnel du dispensaire, qui devra s'authentifier avant de pouvoir accéder à d'autres sections privées.
    À des fins de test uniquement, les liens ont été ajoutés à la barre de navigation.


Structure des dossiers:

accounts (Django)
Dashboard (Django)
Departments (Django)
media (Django)
Patients (Django)
public (React)
ReactDjango (Django)
src (React)
.gitignore
manage.py (Django)
package.json (React)
Procfile  

 (Heroku)
README.md
requirements.txt (Django)
runtime.txt (Heroku)
yarn.lock (React)

Intérêt pour le frontend React uniquement:

    Vous pouvez créer un dossier personnalisé et y déplacer tous les composants React. Votre structure ressemblera alors à ceci :

accounts
Dashboard
Departments
Frontend (public/src/package.json/yarn.lock)
media
Patients
ReactDjango
manage.py
Procfile
requirements.txt  


README.md
runtime.txt

Exécution de l'application:

    Assurez-vous d'avoir Python et Node.js installés.

    Créez un dossier et activez un environnement virtuel à l'intérieur.

    Clonez le projet dans votre dossier principal.

    Naviguez dans le dossier cloné et exécutez les commandes suivantes :
        pip install -r requirements.txt
        python manage.py makemigrations
        python manage.py migrate
        python manage.py createsuperuser (pour créer un superutilisateur)   

        npm install
        npm run-script build
        python manage.py runserver
        npm start (pour démarrer le frontend React)

Note importante:

    Après toute modification des composants React, n'oubliez pas de relancer npm run-script build.
