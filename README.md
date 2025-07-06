# E_Com-Text-Classification

📌 Overview
This project aims to build a multilingual intent classification system for e-commerce platforms that can accurately understand customer queries in English, Hindi, and Spanish. The system processes user queries and predicts their intent (e.g., cancel_order, order_status, general_query) using a combination of Sentence Transformers and machine learning classifiers.

🔧 Key Features
Multilingual Support: Handles English, Hindi, and Spanish customer texts.

Preprocessing Pipeline: Cleans input text by removing punctuation, lowercasing, and language-specific stopwords.

Semantic Embeddings: Uses paraphrase-multilingual-MiniLM-L12-v2 from sentence-transformers to generate meaningful vector representations of sentences.

Intent Classification: Trained models (e.g., MLP, SVM, Logistic Regression) classify queries into one of several e-commerce intents.

Model Evaluation: 5-fold stratified cross-validation was used to evaluate model performance across intents.

Deployment-Ready: All components are saved as .pkl files and can be reused without retraining.

🧠 Dataset Highlights
Balanced across 7 intents:

cancel_order, confirm_order, order_status, change_address, contact_advisor, not_ecommerce, general_query

Text entries in 3 languages:

en (English), hi (Hindi), es (Spanish)

Preprocessed using custom tokenization and stopwords-iso filtering

 Conclusion
This project successfully demonstrates that:

Multilingual customer queries can be effectively understood using sentence embeddings.

Traditional machine learning models (with sentence transformer embeddings) perform well in intent classification tasks.

The use of language-specific preprocessing improves accuracy across diverse linguistic inputs.

The system is scalable and deployment-ready with all models and tools saved as reusable files (.pkl, .bin, etc.).
