# Robot-Mobile-ROS2



Programmation d’un robot et son interface de commande pour obtenir plusieurs modes de fonctionnement.


Trois modes sont possibles:

- Mode Manuel : commande à distance de la direction et de la vitesse de déplacement, avec détection d’obstacles.
- Mode Aléatoire : Le robot se déplace librement, avec détection d’obstacles, et change régulièrement de direction.
- Mode Tracking : Le robot suit une cible ( couleur ) détectée par la caméra.


Le systeme est constitue de plusieurs elements:

- La carte STM32 Nucleo F411 gère :

La commande des moteurs en boucle fermée.
L'acquisition des capteurs de distance.
L'affichage sur l' écran LCD.
La communication avec le Raspberry PI.

- La Raspberry PI gère :
L' acquisition de l'image de la Webcam.
Le traitement de l'image de la Webcam.
La communication avec le PC via la liaison WIFI.

- Une IHM est présente sur PC Host afin de :
Définir les modes de fonctionnement du robot.
transmettre les ordres de direction et de vitesse.
Afficher la valeur des capteurs.
Afficher l' image de la Webcam.

