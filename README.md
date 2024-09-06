# Building_detect_with_deep_learning
L'apport du Deep Learning pour la détection d'adresses et le déploiement de la fibre optique en zone rurale
# L'apport du Deep Learning pour la Détection d'Adresses et le Déploiement de la Fibre Optique en Zone Rurale

## Description
Ce projet explore l'utilisation du Deep Learning, en particulier du modèle **U-Net**, pour améliorer la précision des bases de données d'adresses en zones rurales. En raison de l'urbanisation informelle et des inexactitudes des bases de données, la détection automatisée des adresses permet d'optimiser le déploiement de la fibre optique, avec un impact direct sur la réduction des coûts et l'amélioration de la satisfaction client.

## Objectifs du projet
- Améliorer la précision des adresses en zones rurales à l'aide de méthodes avancées de Deep Learning.
- Détecter les nouvelles constructions non répertoriées pour mettre à jour les bases de données d'adresses.
- Optimiser le déploiement de la fibre optique dans ces zones.

## Modèle Utilisé
Le modèle principal utilisé est **U-Net**, un réseau de neurones convolutifs adapté à la segmentation d'images. Ce modèle a été entraîné pour détecter les bâtiments à partir d'images satellites afin de compléter les données d'adressage.

## Méthodologie
1. **Préparation des données** : Découpage des images satellites en 256x256 pixels et création de masques de polygones des contours des bâtiments.
2. **Choix du modèle** : Utilisation du modèle **U-Net**, comparé à d'autres architectures telles que Mask R-CNN et SegNet.
3. **Entraînement du modèle** : Entraînement sur plusieurs itérations avec des images satellites de la commune d'Agnin, Isère.
4. **Évaluation des résultats** : Précision élevée du modèle avec des courbes de perte stables, indiquant une bonne généralisation.

## Bibliothèques Utilisées
- **TensorFlow**
- **PyTorch**
- **Keras**
- **rasterio** et **shapely** pour la manipulation des données géospatiales.

## Résultats
Le modèle U-Net, notamment la variante avec **EfficientNet-B4**, a montré une bonne précision dans la détection des bâtiments, ce qui a permis une meilleure gestion des données d'adressage dans les zones rurales. Cela a directement contribué à l'amélioration de la planification du déploiement de la fibre optique.

## Applications Futures
- **Optimisation du déploiement de la fibre** : Identifier les nouvelles constructions et planifier les extensions du réseau.
- **Correction des erreurs d'adressage** : Résoudre les erreurs en temps réel lors des phases de déploiement.

## Références
- [Smith et al. (2018)](https://www.tree-learning.fr) : Analyse des images aériennes avec CNN.
- [Li et al. (2017)](https://www.tree-learning.fr) : Détection des palmiers à huile à partir d'images de télédétection.
- [Ma et al. (2019)](https://www.tree-learning.fr) : Analyse des applications du Deep Learning en télédétection.
