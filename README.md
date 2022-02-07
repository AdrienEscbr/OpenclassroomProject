# OpenclassroomProject
Date : 07/02/2022

Dans ce projet, j'apprend à utiliser les fondamentaux de Git et Github !


• Git :

- Installer la dernière version de Git 

--> Configuration :

      - ouvrir GitBash
      
      - se positionner dans un dossier local (commande 'cd')
      
      - créer un dossier (commande 'mkdir')
      
      - écrire les commandes suivantes : 
      
          git config --global user.name "mon nom prénom utilisateur"
          git config --global user.email monAdresseMail@gmail.com
          git config --global color.diff auto
          git config --global color.status auto
          git config --global color.branch auto 
          git config --global core.editor vim
          git config --global merge.tool vimdiff
          git init
          
--> Premiers fichiers :

      - dans le dossier local : touch index.html 
                                touch styles.css
                                
      - écrire la structure de base html et lier le fichier css
      
      - commande : git status -> permet de voir les fichier 
          • si fichier en rouge : fichier créé, modifié ou supprimé mais pas encore indexé
          • si fichier en vert : fichier indexé 
          
      - commande : git add -> permet de mettre à jour les fichiers créés, modifiés ou supprimés
          exemple : git add nomdufichier.html/.css/... (on peut indexé plusieurs fichiers en une ligne de commande en les mettant à la suite)
      
      - commande : git commit -> permet de créer une nouvelle version du projet et passer les fichiers indexés dans le repository
          exemple : git commit -m "description du commit"
          
--> Envoyer son commit sur GitHub :

Après avoir créé un répository pour le projet sur GitHub :

      - copier le lien du repository au haut
      
Dans GitBash :

      - commande : git remote add origin https://github.com/leResteDuLien.git
      
      - commande : git branch -M main 
      
      - commande : git push -u origin main 
      

--> Les commandes à RETENIR : 

- Indexer le fichier HTML modifié grâce à la commande : 

      git add index.html
    
- Créer une nouvelle version grâce à la commande :

      git commit -m “Modification du titre H1”
    
- Envoyer la nouvelle version sur le dépôt distant grâce à la commande :

      git push origin main

