# Real-Time-Object-Notifier

Ce programme Python utilise le modèle YOLOv8 pour la détection d'objets en temps réel via une webcam et annonce les objets détectés à l'aide d'une synthèse vocale (TTS).

#Fonctionnalités

Détection d'objets en temps réel avec YOLOv8.
Affichage des objets détectés avec des cadres de délimitation et des scores de confiance.
Annonce vocale des objets détectés et leur nombre toutes les 3 secondes.
Support des voix anglaises (Zira ou David) si disponibles.

#Pré-requis

Python 3.9 (recommandé)

#Fonctionnement

Le programme initialise le moteur TTS et sélectionne une voix anglaise si disponible.
Il ouvre ensuite le flux de la webcam et charge le modèle YOLOv8.
Les images capturées par la webcam sont traitées pour détecter les objets et dessiner des cadres de délimitation autour d'eux.
Toutes les 3 secondes, les objets détectés et leur nombre sont annoncés via la synthèse vocale.
Le flux vidéo est affiché dans une fenêtre que tu peux fermer en appuyant sur la touche q.

#Résolution des problèmes

Si le flux de la webcam ne s'ouvre pas, vérifie que ta caméra est bien connectée et accessible.
Si le moteur TTS ne sélectionne pas une voix anglaise, cela signifie qu'elle n'est peut-être pas disponible sur ton système ; dans ce cas, une voix par défaut sera utilisée.
Assure-toi que le fichier de poids YOLOv8 est dans le bon répertoire (yolo-Weights/) si le téléchargement automatique échoue.

#Contribution

N'hésite pas à ouvrir des issues ou des pull requests si tu découvres des bugs ou si tu as des suggestions pour améliorer le projet.


