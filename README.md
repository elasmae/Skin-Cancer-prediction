# Classification des Images de Cancer de la Peau (Bénin ou Malin)

## Description du Projet
Ce projet a pour objectif de classifier des images de la peau en identifiant si elles correspondent à un cas bénin ou malin de cancer. Le processus est divisé en plusieurs étapes clés :
1. **Segmentation des Images** :
2. **Extraction des Caractéristiques** :
   - Utilisation de **Local Binary Pattern (LBP)** pour extraire des textures locales.
   - Utilisation des **percentiles de couleur** pour capturer les informations chromatiques.
3. **Entraînement et Évaluation des Modèles** :
   Les modèles suivants sont entrainées sur seg_train ( données d'entrainemnt aprés Segmentation)
   - **Nearest Neighborhood (NN)**
   - **Nearest Mean Classifier (NMC)**
   - **Linear Classifier**
   - **Support Vector Classifier (SVC)**

   L'évaluation permettra de sélectionner le modèle offrant les meilleures performances pour la prédiction.

4. **la prédiction**: Prédire les images dans *Predict* et enregistrer les prévisions dans *Prediction.csv*.