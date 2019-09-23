# README pour tester Flask  
Le service web permet d'uploader une image puis de détecter les déchets qui sont dessus. Le résultat de la prédiction est enregistré sous image dans "FlaskSurfrider/static/img/" et sous forme de json dans "FlaskSurfrider/static/json/"  

Prérequis :  
1) Avoir git bash  
2) Avoir python 

Etapes pour tester flask :  
1) Ouvrez git bash  
2) Clonez le repository  
	> git clone https://github.com/ShareAI-SF/FlaskSurfrider.git  
3) Déplacez vous dans le bon répertoire  
	> cd FlaskSurfrider

4) Installez les librairies nécessaire
	> pip install -r requirements.txt

5) Téléchargez le model à cette adresse : https://drive.google.com/file/d/1AXs7w3uj58VGBUlNLSgdGXGFG8dUcL6-/view?usp=sharing

6) Déplacez le model téléchargé dans le dossier models (FlaskSurfrider/models/frozen_inference_graph.pb)

7) Lancez le serveur  
	> python flasksurfrider.py  

8) 	Accédez à http://127.0.0.1:5000/ dans un navigateur  
	Cliquez sur "Choisir un fichier", il y a déjà trois images dans "FlaskSurfrider/static/img/" pour tester   
	Après avoir choisi l'image, cliquez sur "Valider"  
	Après 1 ou 2 min l'image prédite s'affichera et sera enregistrée dans "FlaskSurfrider/static/img/", le résultat en json sera aussi enregistré dans "FlaskSurfrider/static/json/"  
	Vous pouvez tester une autre image en cliquant sur "Essayer une autre image"  