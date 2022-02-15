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
      
      
--> Gérer les branches :


Les branches permettent de développer une partie du projets sans altérer le reste du travail qui a été réalisé et validé.


Pour connaitre les branches présentes dans le projet : 

      - commandde : git branch
      
REMARQUE : 

Le caractère '*' devant le nom de la branche correspond à la branche dans laquelle on se situe. 

Pour créer une branche : 
      
      - commande : git branche NomDeLaBranche
      
Pour basculer sur une autre branche : 

      - commande : git checkout NomDeLaBranche

REMARQUE : 

Dans une nouvelle branche, on peut créer autant de répertoires et de fichiers que l'on souhaite.


Pour créer une nouvelle version du projet comprenant les évolutions réalisées sur la branche (même chose que précédemment, il faut commit) :

      - commande : git commit -m "Description de ce qu'apporte cet enregistrement"
      
Il faut ensuite push les modifications : 

      - commande :  git push -u origin NomDeLaBranche  


--> Fusionner notre travail :

Par la suite, on veut pouvoir ajouter le travail treminé et validé dans notre branche pour la rajouter au projet dans notre branche principale.
Pour ce faire on utilise le 'merge'. On se positionne dans la branche main (avec git chechout main) puis :

      - commande : git merge  NomDeLaBrancheAFusionner
      
Voilà, le tour est joué !




--> Les commandes à RETENIR : 

- Indexer le fichier HTML modifié grâce à la commande : 

      git add index.html
    
- Créer une nouvelle version grâce à la commande :

      git commit -m “Modification du titre H1”
    
- Envoyer la nouvelle version sur le dépôt distant grâce à la commande :

      git push origin main

- Connaitre les branches présentes dans le projet : 

      git branch

- Créer une branche : 
      
      git branche NomDeLaBranche
      
- Basculer sur une autre branche : 

      git checkout NomDeLaBranche

- Créer un fichier texte : 

      echo > NomDuFichier.txt









