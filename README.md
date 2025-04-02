
# 🧬 Classification d’Images de Cancer de la Peau (Bénin vs Malin)

## 📝 Description du Projet

Ce projet vise à développer un système de classification d’images dermatologiques afin de déterminer si une lésion cutanée est **bénigne** ou **maligne**. Il s’inscrit dans une démarche de soutien au diagnostic médical à l’aide de méthodes d’apprentissage automatique et de traitement d’image.

---

## 🔍 Étapes du Projet

### 1. **Segmentation des images**
Les images brutes sont d’abord segmentées afin d’isoler la zone d’intérêt (la lésion) pour un traitement plus ciblé.

### 2. **Extraction des caractéristiques**
Deux types de descripteurs sont utilisés pour représenter les images :
- **Local Binary Patterns (LBP)** : pour capturer la texture locale des lésions.
- **Percentiles de couleur** : pour résumer les informations chromatiques présentes dans chaque image.

### 3. **Entraînement et évaluation des modèles**
Les modèles sont entraînés sur l’ensemble **`seg_train`** (images segmentées) et évalués pour identifier le plus performant. Les modèles testés sont :
- **Nearest Neighbor (NN)**
- **Nearest Mean Classifier (NMC)**
- **Classifieur Linéaire**
- **Support Vector Classifier (SVC)**

L’évaluation des performances permet de sélectionner le modèle le plus adapté à la tâche de classification.

### 4. **Prédiction finale**
Le modèle retenu est utilisé pour prédire les classes des images contenues dans le dossier **`Predict_test`**. Les résultats sont enregistrés dans le dossier **`Prediction_Results`**.

---

## 👩‍💻 Auteur

**Asmae EL MAHJOUBI**  
Master Statistiques et Sciences des Données  
📅 2020
