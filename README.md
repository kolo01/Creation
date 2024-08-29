#  _CREER UN PROJET DJANGO DE LA CREATION DU PROJET A L'INTEGRATION DES TEMPLATES_
##
##

## 1- Creation d'un environnement virtuel et activation

            Creation: python -m venv le_nom_de_l'environnement_virtuel
            Activation :  le_nom_de_l'environnement_virtuel\Scripts\activate 
            
            
## 2- Installation de Django

            python -m pip install Django
            
## 3- Creation de projet Django

             django-admin.exe  startproject le_nom_du_projet
             
## 4- Creation d'une application django

            mv le_nom_du_projet  src
            cd src
            python.exe manage.py startapp le_nom_de_l'application
            
## 5- Integration de notre application, des dossiers templates et static

            - Afin d'integrer notre application et y avoir acces dans notre projet, nous devons l'enregistrer dans les applications installées contenus dans le fichier settings.py du dossier de notre project.
            
            - Dans settings rechercher "INSTALLED_APPS" parmi les variables presentes.
            
            - ajouter l'application en ecrivant dans le tableau :
                    - 'nom_de_l'application',
                    
            Toujours dans Settings
            
                - Rechercher "TEMPLATES" 
                - Puis "DIRS"  
                - Ajouter comme valeur "[ BASE_DIR / 'templates'],"
                
                - Enfin tout en bas ajouté cela :
                    STATICFILES_DIRS = [os.path.join(BASE_DIR, 'static')]
                
                - Importer os tout en haut du fichier Settings en ajoutant "import os"
                
                
 
## 6-  Insertion du template choisi

        - Creer un dossier templates et un dossier static dans le dossier qui contient notre application
        - Inserer les fichiers HTML dans le dossier templates
        - Inserer les fichiers css, js et les images dans le dossier static

## 7- Insertion
 
