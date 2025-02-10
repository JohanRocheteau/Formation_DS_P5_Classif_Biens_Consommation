# 📊 Projet N°5 : Classifiez automatiquement des biens de consommation

## **📌 Contexte et Objectif**

**Entreprise :** Place de marché  
**Logo :** ![Logo](PhotosReadme/LogoP5.png)

### **🎯 Objectif**
L'objectif est d'attribuer automatiquement des catégories aux produits vendus par les clients sur une plateforme e-commerce en utilisant leurs descriptions et images.

### **📂 Jeux de données**
- **Données :** [Les Données](https://s3-eu-west-1.amazonaws.com/static.oc-static.com/prod/courses/files/Parcours_data_scientist/Projet+-+Textimage+DAS+V2/Dataset+projet+pre%CC%81traitement+textes+images.zip)
- **Missions du projet :**
  - Automatiser l'attribution de catégories de produits, qui est actuellement effectuée manuellement par les vendeurs.
  - Étudier la faisabilité d'un moteur de classification des produits basé sur les images et descriptions.
  - Analyser la possibilité de récupérer des informations sur les produits via une API.

---

## **🚀 Réalisations et Méthodologie**

### **1️⃣ Prétraitement des données**
- **Ouverture des données :** Analyse du contenu et nettoyage de la DataFrame pour préparer les données pour le traitement.
- **Nettoyage des données textuelles :** 
  - Tokenisation, suppression des mots vides, ponctuation, stemming et lemmatisation.
  
  - **Visualisations :**
    - Distribution du nombre de mots dans la DataFrame :
    
      ![TopFlop](PhotosReadme/TopFlopWords.png)
    
    - Nuage de mots pour visualiser les mots les plus fréquents :
    
      ![Nuage](PhotosReadme/nuages.png)

### **2️⃣ Analyse NLP (Traitement du langage naturel)**
- **Techniques utilisées :** CountVectorizer, Tfidf, Word2Vec, BERT et USE.
  
- **Visualisation des résultats :** Pour chaque modèle NLP, une étude visuelle des groupes créés via **KMeans** avec **t-SNE** et une matrice de confusion pour observer la qualité de la classification.
  
  ![GraphsNLP](PhotosReadme/GraphiquesNLP.png)
  
- **Modèles de Machine Learning :** Application de plusieurs modèles pour tester la faisabilité de la classification via le NLP.
  
  ![MLNLP](PhotosReadme/MLNLP.png)

### **3️⃣ Analyse d'Images**
- **Techniques utilisées :** SIFT et CNN (Transfert Learning).
  
- **Visualisation des groupes créés :** Comme pour le NLP, les résultats des groupes réels vs les groupes créés sont analysés via **KMeans** et **t-SNE**.

  ![GraphsImages](PhotosReadme/GraphiquesImages.png)
  
- **Modèles de Machine Learning :** Utilisation de différents modèles pour tester la faisabilité de la classification via les images des produits.

  ![MLImages](PhotosReadme/MLImages.png)

### **4️⃣ API Epicerie Fine**
- **API utilisée :** [Edamam Food and Grocery Database](https://rapidapi.com/edamam/api/edamam-food-and-grocery-database)
  
- **Exemple d'extraction des informations sur un produit spécifique (champagne) :**
  
  ![Champagne](PhotosReadme/APIChampagne.png)

---

## **📈 Résultats et Insights**

- **Prédiction via NLP et Images :** Les résultats sont mitigés, avec certains modèles montrant des erreurs de classification dues à des limitations dans les données disponibles (manque de diversité dans les descriptions et images).
- **API de données :** L'intégration de l'API permet de récupérer des informations externes utiles pour enrichir la classification des produits.

---

## **🛠️ Technologies et Outils Utilisés**

- **Langage :** Python 🐍
- **Librairies :** Pandas, Seaborn, Matplotlib, Scikit-learn, Keras, TensorFlow, PIL, Numpy, requests
- **Méthodes utilisées :** NLP, Machine Learning, Computer Vision (CNN, SIFT), Data Cleaning, API Integration

---

## **📬 Contact et Feedback**

💡 Ce projet a été réalisé dans le cadre de ma **formation Data Science**. N’hésitez pas à **laisser vos suggestions** ou à **me contacter** pour en discuter !  

📩 **Contact :**  
📧 [johan.rocheteau@hotmail.fr](mailto:johan.rocheteau@hotmail.fr)  
🔗 [LinkedIn](https://www.linkedin.com/in/johan-rocheteau)
