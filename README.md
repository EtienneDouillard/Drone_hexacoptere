# Drone hexacoptère

## Présentation

Ce projet de drone a été commencé en Septembre 2018 par un groupe d'étudiant ingénieur de l'ISEN nantes. Il évolue depuis avec les différents étudiants motivés pour l'améliorer.

Le but de ce projet était de créer un drone qui puisse servir de base à d'autres projets étudiant. Il correspond donc en termes de taille et d'autonomie à un compromis entre nos attentes, notre budget et le temps que nous y accordons.

Vous pourez retrouver dans les dossiers les assemblages et pièces concue sur SolidWorks 2017. Vous y retrouverez aussi les références des pièces utilisées ainsi que les liens pour la configuration du logiciel et le cablage de l'ensemble.

![alt text](https://github.com/iRobotEam/Drone_hexacoptere/blob/master/images/IMG_3299.JPEG?raw=true)

## Composants et pièces

* Raspberry pi 3b
* Navio 2
* Moteur Brushless MT3506 650kv - TMOTOR
* ESC .........
* hélices .........
* Voltmètre FS-CVT01
* Récepteur RC FS-iA10B
* Radiocommande RC Flysky FS-i6X 10CH
* Navio 2 Power module
* Batterie ..........
* carte de distribution de courant
* Chassis :
  * plaques de pvc
  * supports moteur en ABS
  * bras en tubes de carbonne
  * fixation bras en ABS
  * support raspberry pi

## Bloc Moteur

Pour le trio ESC, moteur, hélice, nous avons choisis un ensemble commercialisé par T-MOTOR nous permetant d'avoir des données fiables sur la consomation, le rendement et la force de portance produite.

Voir le tableau descriptif des données moteur dans le dossier moteur.

## Electronique de bord

Nous utilisons une raspberry pi et un module navio 2 comme controleur de bord. Ce n'est pas l'option la plus économe en énergie et en poid mais cela nous permet une très grande modularité. Nous pouvons ajouter une très large gamme d'options.

### Raspberry pi

Flashé avec raspbian, nous utilisons ardupilot comme logiciel de vol. La modularité et la facilité d'instalation étant notre priorité. Nous pouvons passer sur ROS pour une adaptabilité supérieur.

[documentation ardupilot](https://ardupilot.org/copter/index.html)


Pour le moment le raspberry se connecte à un partage de connexion préconfiguré. Il faudrait configurer le raspberry pour qu'il crée son propre réseau et que l'ordinateur ou le smartphone qui le commande se connecte dessus. La première solution a été choisis pour faire des mises à jours facilement.

### Navio 2

Elle est quipé de multiples capteurs et ports d'extantion pour les améliorations futur.

[documentation navio 2](https://docs.emlid.com/navio2/)

[documentation navio 2 github](https://github.com/emlid/emlid-docs/tree/master/docs/autopilots/navio2)

Voir le cablage des moteurs avec leurs sens de rotation et leurs numéro de sortie dans les images.

### Voltmètre

Permet un retour en direct de la charge de la batterie sur la télecomande.

## Radiocommande

Nous avons opté pour une télécomande milieu / bas de gamme pour le budget et car nos exigences de porté ne sont pas très grande. **obligation de voler à vue**

Les impératifs que nous avons concernent la sorties PPM qui est le seul moyen de communiquer avec la navio 2. Cela regroupe les 10 canaux sur un seul fil de donnée.

## Sponsors

**Merci à nos sponsors pour leurs soutien**

[hynoxelis](https://www.hynoxelis.com/)

[axandus](https://www.axandus.fr/)

[kinematiq](https://www.kinematiq.net/)

[mptruck](https://www.mptruck.fr/)



