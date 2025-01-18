# 🎥 Anime Recommendation System

This repository contains an end-to-end machine learning pipeline for an anime recommendation system. The project employs **Singular Value Decomposition (SVD)** and **K-Means clustering** to predict and recommend anime to users based on their ratings and preferences. The dataset contains ratings from 73,516 users for over 12,000 anime.

🧠 **Problem Statement**

The goal of this project is to create a recommendation system that suggests anime to users based on their ratings. The data consists of user ratings for various anime, and the challenge involves predicting ratings for anime the user hasn't watched yet. The system uses matrix factorization and clustering techniques to provide recommendations tailored to user preferences.

⚙️ **Key Features**

- **Exploratory Data Analysis (EDA)**:
    - Distribution analysis of anime ratings.
    - Genre and type analysis using visualizations.
    - Handling missing values and duplicates in the dataset.

- **Data Preprocessing**:
    - Label encoding for categorical features (genre, type).
    - Scaling and PCA for dimensionality reduction.
    - Hyperparameter tuning for KMeans clustering.

- **Model Training**:
    - **SVD Model**: Used for collaborative filtering-based recommendations.
    - **K-Means Clustering**: Grouped users and anime for cluster-based recommendations.
    - **Evaluation**:
        - **SVD Model RMSE**: 0.0769 (Low error indicating good model performance).
        - **K-Means Clustering RMSE**: 0.29 (Indicates room for improvement but still reasonable predictions).

- **Recommendation System**:
    - **SVD-based Recommendations**: Suggest anime based on predicted ratings.
    - **Cluster-based Recommendations**: Recommend anime based on user’s assigned cluster.

🔍 **Results**

- **SVD Model** achieved an RMSE of 0.0769, indicating effective prediction of anime ratings.
- **K-Means Clustering** achieved an RMSE of 0.29, with more interpretable results and group-based recommendations.

💻 **Tools & Libraries**

- **Python**: Core programming language used for the project.
- **Pandas, NumPy**: For data manipulation and preprocessing.
- **Scikit-learn**: For machine learning algorithms, preprocessing, and evaluation.
- **Surprise**: For SVD-based collaborative filtering.
- **Matplotlib, Seaborn**: For data visualization.
- **GridSearchCV**: For hyperparameter optimization of KMeans clustering.

🔧 **Installation**

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/anime-recommendation-system.git
   cd anime-recommendation-system
