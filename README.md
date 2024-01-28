<body>
<h3>1- Data</h3>
  <p> 
-Les photos sont entièrement réelles.
<br><br>
-Les images ont une taille de 2448 x 3264 (haute résolution pour de meilleurs résultats)
<br><br>
-les images ont été prise dans différentes situations(intensité-éclairage-angles)
<br><br>
-apres la collection des images, ils ont été labelés sur l'application label img, lien : https://github.com/tzutalin/labelImg ,
un fichier .txt est généré pour chaque image.
<br><br>
-Ensuite la base d'images doit etre partitionné en test et train. 75% 25%, 687 pour le train et 224 pour le test
<br><br>
-La dataset est trandformée en .yaml à l'aide du site wandb : site ou on peut tracker les metrics et les trainings
par la commande suivante : 
    
    python utils/loggers/wandb/log_dataset.py --project custom_yolov5 --data data/custom_dataset.yaml
    
</p>
<h3>2- YOLO V5</h3>

```
!git clone https://github.com/ultralytics/yolov5
```
<h3>3- Train</h3>
Parameters : 

* `--project` : Le nom du projet
* `--upload_dataset` : Pour mettre à jour wandb par rapport aux résultats
* `--bbox_interval` : Intervals réguliers
* `--img` : Taille utilisée pour les images
* `--save_period`: Sauvegarder les epochs
* `--weights`: Type de yoloV5 utilisé : s, m, l ou x
<h3>4- SIFT Algorithm</h3>
<img src=https://github.com/sou-design/Licence-Plate-recognition/assets/62157910/08d06464-a4f0-490e-a096-828a38c55d1b" width = 400>
<br>
<img src="https://github.com/sou-design/Licence-Plate-recognition/assets/62157910/83972a18-26d7-47f3-91c6-3b9831f010d8" width = 800>
<h3>5- HOG Algorithm</h3>
<img src="https://github.com/sou-design/Licence-Plate-recognition/assets/62157910/0cd5e619-dcc9-4a9c-9b48-928f9c3f738b" width=400>
</body>
