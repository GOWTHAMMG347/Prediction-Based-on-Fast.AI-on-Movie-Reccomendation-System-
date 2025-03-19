# Prediction-Based-on-Fast.AI-on-Movie-Reccomendation-System-
# FastAI - Tabular and Collaborative Filtering Example

This repository demonstrates how to use FastAI for both **tabular data** processing and **collaborative filtering** for movie recommendations. The code utilizes FastAI's powerful data processing and model training features to handle various machine learning tasks.

## Prerequisites

Ensure you have the following libraries installed:

- **fastai** (install via `pip install fastai`)
- **pandas** (install via `pip install pandas`)
- **torch** (install via `pip install torch`)

---

## Contents

1. **Tabular Data Processing**
2. **Collaborative Filtering for Movie Recommendations**

---

## 1. Tabular Data Processing

### Overview

This section demonstrates how to use FastAI to process and train a model on tabular data. Specifically, we use the **Adult Income Dataset**, which contains demographic data and aims to predict whether an individual earns more than $50,000 a year based on their characteristics.

### Key Steps

1. **Data Loading & Preprocessing:**  
   The Adult Income dataset is loaded and preprocessed by filling missing values, categorifying the categorical variables, and normalizing continuous variables.

2. **Data Splitting & Dataloaders:**  
   A `TabularDataLoaders` object is created to handle the training and validation sets.

3. **Model Training:**  
   A model is trained on the tabular data, with an emphasis on predicting income based on the provided attributes. We use FastAI's tabular learner for model creation and training.

---

## 2. Collaborative Filtering for Movie Recommendations

### Overview

This section demonstrates how to use FastAI’s collaborative filtering capabilities to build a movie recommendation system using the **MovieLens 100K dataset**. The goal is to predict movie ratings based on user and movie features.

### Key Steps

1. **Data Loading & Preprocessing:**  
   The **MovieLens 100K dataset** is loaded, and the movie ratings are merged with movie metadata (titles, genres, etc.).

2. **Data Splitting & Dataloaders:**  
   The ratings dataset is split, and a `CollabDataLoaders` object is created, ready for training.

3. **Model Training:**  
   A collaborative filtering model is trained using FastAI's `collab_learner()` function, which predicts ratings based on latent factors.

---

## Results and Evaluation

After training the models for both tasks, the resulting models can be used for predictions:

- **Tabular Model:** Predictions are made to classify whether an individual earns more than $50,000 annually based on attributes.
- **Collaborative Filtering Model:** The model is capable of predicting user ratings for movies and making personalized recommendations.

---

## Conclusion

This code provides a foundation for working with both tabular data and collaborative filtering models using FastAI. By leveraging FastAI's efficient data loading, processing, and model training features, you can quickly build and evaluate machine learning models for both supervised and unsupervised tasks.

---

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
