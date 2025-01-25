# Fake News Detection 

## Project Overview
This project implements a machine learning model to detect fake news using natural language processing techniques and a deep learning approach.

## Data Preprocessing
- **Data Sources**: Two CSV files - "True.csv" and "Fake.csv"
- **Data Combination**: 
  - Combined true and fake news datasets
  - Added binary label `isfake` (0 for true, 1 for fake)
  - Merged title and text into single 'original' column

## Text Preprocessing
- Utilized NLTK and Gensim for text cleaning
- Preprocessing steps:
  - Removed stopwords
  - Eliminated words with 2 or fewer characters
  - Tokenized text
- Total unique words: Approximately 9,000

## Exploratory Data Analysis
- Created visualizations:
  - Subject distribution plot
  - Fake vs. Real news distribution
  - Word clouds for fake and real news

## Model Architecture
- Deep Learning Model: Sequential Neural Network
- Key Components:
  - Embedding Layer (240 dimensions)
  - Bidirectional LSTM Layer (128 units)
  - Dense Layers with ReLU and Sigmoid activations
- Optimizer: Adam
- Loss Function: Binary Crossentropy

## Model Performance
- Validation Method: 80/20 train-test split
- Model Accuracy: Varies (determined by training run)
- Confusion Matrix generated to show performance metrics

## Key Libraries Used
- TensorFlow/Keras
- Pandas
- NumPy
- NLTK
- Gensim
- Matplotlib
- Seaborn

## Conclusion
The project demonstrates a deep learning approach to fake news detection using natural language processing techniques.
