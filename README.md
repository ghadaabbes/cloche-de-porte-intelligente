# cloche-de-porte-intelligente
La cloche de porte intelligente basé sur un système de reconnaissance faciale reconnaît toute personne pré-autorisée et ouvre la porte pour qu'elle puisse entrer sans aucune interaction manuelle ou contrôlée. Il suffit de montrer votre visage et Smart Door ouvrira la voie. Plus besoin de se souvenir de porter une clé, qui peut être perdue ou volée. 


Il existe de nombreux algorithmes et méthodes de reconnaissance des visages.
Nous avons choisi les méthodes d’apprentissage automatique pour la reconnaissance faciale, car elles résolvent en réalité une série de problèmes connexes:

- D'abord, regarde une image et trouve tous les visages qu'elle contient
- Deuxièmement, concentrez-vous sur chaque visage et soyez en mesure de comprendre que même si un visage est tourné dans une direction étrange ou sous un mauvais éclairage, il reste la même personne.
- Troisièmement, soyez en mesure de choisir les caractéristiques uniques du visage que vous pouvez utiliser pour le distinguer des autres personnes - comme la taille des yeux, la longueur du visage, etc.
- Enfin, comparez les caractéristiques uniques de ce visage à toutes les personnes que vous connaissez déjà pour déterminer le nom de cette personne.
Les ordinateurs ne sont pas capables de ce type de généralisation de haut niveau (du moins pas encore…), nous devons donc leur apprendre à effectuer chaque étape de ce processus séparément.

Installer:
- Raspbian Jessie 
- Dlib library
- python 2.7 ou 3 and numpy
- OpenCV
- face recognition library 
- NodeJS
- ReactJS
- MongoDB server
- Webcam driver dépend de genre et marque de caméra

Instructions pour les connexions de circuit
Voici les étapes pour les connexions de circuit -
Fixez le module de caméra Raspberry Pi
 
Ajoutez un bouton (agit comme sonnette) sur la broche 27 de GPIO.
Comment configurer et exécuter le code
 Raspberry Pi - Passerelle
1. Connecter le circuit
2. Connectez-vous à Raspberry Pi via SSH.
3. Installez vncserver sur votre PC et sur votre framboise pi, connectez-vous à framboise via VNC.
4. Le code Raspberry Pi contient un fichier, usbcamera.py, qui prend les photos et transmet l’image à notre serveur d’applications. Exécutez le fichier à l’aide de la commande "sudo python usbcamera.py".
5. Assurez-vous que le fichier ci-dessus est en cours d'exécution.
 Serveur -
1. Installez le module npm.
2. Installez les dépendances suivantes à l’aide de npm -
 
•	Express
• bcrypt
•	Express
• json webtoken
• mangouste
• morgan
• nodemon
• analyseur de corps
 
3. activer mongodb avec la commande “sudo service mongodb start”
4. Exécuter dans le répertoire du serveur npm run dev
 Frontend

1. Exécuter dans le répertoire frontend npm start
2. Accès au site via le lien: http: // localhost: 8080
