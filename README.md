# AI-Powered-Food-Recommendation-System
🔍 Overview
Modern diets are often unbalanced due to lack of nutritional awareness and meal planning tools. This system leverages machine learning to help users make healthier choices by:

Predicting the caloric content of foods using a Random Forest Regressor
Recommending similar foods based on user preferences using K-Means Clustering and Cosine Similarity
The system is built on a reliable dataset from the USDA (via Kaggle) containing over 5,000 food items with 20+ nutritional attributes.

🧠 Key Features
1. Calorie Prediction Model
Built using Random Forest Regression for high accuracy
Achieved R² score: 0.9939 , MSE: 171.3 , showing excellent predictive performance
Trained on macronutrient data including protein, lipids, carbohydrates, fiber, and sugar
2. Food Recommendation Engine
Used K-Means Clustering to group foods by nutritional profiles
Implemented Cosine Similarity to rank and recommend top 20 food items based on user input
Metrics used: Silhouette Score (0.55) , Davies-Bouldin Index (0.63) , and WCSS
3. Data Mining Pipeline
Dataset preprocessing including:
Missing value handling via median imputation
Outlier detection using Z-Score
Feature selection and scaling (Min-Max Normalization , StandardScaler )
📁 Project Structure


1
2
3
4
5
6
7
8
9
AI-Powered-Food-Recommendation-System/
│
├── data/                   # USDA food dataset (ABBREV.csv)
├── models/                 # Trained ML models (Random Forest, K-Means)
├── notebooks/              # Jupyter Notebooks for EDA and model training
├── presentation/           # PowerPoint slides (.pptx) explaining the project
├── src/                    # Python scripts for data processing and recommendation logic
├── app.py                  # Optional: Flask/FastAPI backend placeholder
└── README.md               # You're here!
🚀 Future Work / Full-Stack Integration
This system can be extended into a full-stack application with:

A frontend interface (e.g., Streamlit, React, Vue.js) for user inputs and recommendations
A backend API (e.g., FastAPI, Flask) to serve model predictions
Real-time user interaction for:
Custom food preference entry
Instant calorie estimation
Personalized food suggestions
📊 Dataset Source
Name : Nutritional Content of Food (ABBREV.csv)
Source : Kaggle – U.S. Department of Agriculture (USDA)
Size : ~5,000 food items
Features : Calories, Protein (g), Lipids (g), Carbohydrates (g), Fiber, Sugar, and more
📙 Presentation Included
A PowerPoint presentation is included in the presentation/ folder, summarizing:

Motivation & problem statement
Data preprocessing steps
Model building and evaluation
Results and future enhancements
🛠️ Technologies Used
Python (scikit-learn, pandas, numpy, matplotlib)
Machine Learning Algorithms : Random Forest, K-Means Clustering
Similarity Matching : Cosine Similarity
Evaluation Metrics : MSE, R², Silhouette Score, WCSS
Optional Tech for Full Stack Extension : FastAPI / Flask, Streamlit, React / Vue.js
📌 Why This Matters
Helps users understand the nutritional value of their meals
Promotes healthier eating habits through personalization
Demonstrates how data science and ML can be applied to everyday wellness challenges
✅ How to Use
Run the Jupyter Notebook to explore the data analysis and model training
Try out the recommendation engine with custom food inputs
Extend it into a web app using your preferred frontend/backend stack
