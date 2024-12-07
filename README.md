# Sentiment-Analysis-Shopee-Review-Vietnamese

**I. Objective**
- This project aims to perform sentiment analysis on Vietnamese text
- Project uses PhoBERT for feature extraction, and choosing among Logistic Regression, Decision Tree and Random Forest for classification

**II. Dataset**
- [Kaggle | Vietnamese sentiment analyst](https://www.kaggle.com/datasets/linhlpv/vietnamese-sentiment-analyst/data?select=data.csv)
- Customer Shopee reviews are label positive, negative or neutral

**III. Steps** 

***1. Data Preprocessing***
- The dataset is loaded and cleaned by removing rows with missing values.
- Labels are converted to numerical values 

***2. Feature Extraction***
- PhoBERT, a pre-trained language model for Vietnamese, is used to extract text embeddings.
- The extract_embedding_batch function tokenizes the text and extracts embeddings using PhoBERT.

***3. Model Training***
- Logistic Regression is employed as the classification model.
- The model is trained on the extracted embeddings and corresponding labels.

***4. Evaluation***
- The model's performance is evaluated on a test set using accuracy and classification report metrics.

***5. Prediction***
- The trained model is saved and can be loaded for predicting sentiment on new text samples.
- The model predicts the sentiment label (Positive, Negative, or Neutral) for a given input.

**References**
- [Vietnamese correction](https://github.com/bmd1905/vietnamese-correction/?tab=readme-ov-file)
- [PhoBERT](https://github.com/VinAIResearch/PhoBERT?tab=readme-ov-file#introduction)
