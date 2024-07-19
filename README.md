# Sentiment-Analysis

## Overview
This project involves performing sentiment analysis on the Yelp Academic Dataset, specifically the yelp_academic_dataset_tip.json file. The goal is to analyze the sentiments expressed in the tips provided by users and classify them as positive, negative, or neutral.

## Dataset
The dataset used for this project is **`yelp_academic_dataset_tip.json`**, which is part of the Yelp Dataset. This file contains user-generated tips about businesses listed on Yelp.

# Source
The dataset is sourced from:
1. Yelp Dataset

## Installation
To set up the project, follow these steps:

1. Clone the repository:
```
git clone https://github.com/gaytri9/Sentiment_Analysis.git
```
2. Navigate to the project directory:
```
cd yelp-sentiment-analysis
```
3. Create a virtual environment:
```
python -m venv venv
```
4. Activate the virtual environment:
   4.1 On Windows:
   ```
   venv\Scripts\activate
   ```
   4.2 On macOS and Linux:
   ```
   source venv/bin/activate
   ```
   
##Usage
To run the sentiment analysis, follow these steps:

1. Ensure your dataset file **`yelp_academic_dataset_tip.json`** is in the data directory.
2.Preprocess the dataset:
```
python preprocess.py
```
3. Train the sentiment analysis model:
```
python train.py
````
4. Perform sentiment analysis on the tips:
```
python analyze.py --input data/yelp_academic_dataset_tip.json --output output/sentiment_analysis_results.json
```

## Directory Structure
```
yelp-sentiment-analysis/
│
├── data/
│   └── yelp_academic_dataset_tip.json
│
├── output/
│   └── sentiment_analysis_results.json
│
├── src/
│   ├── preprocess.py
│   ├── train.py
│   └── analyze.py
│
├── models/
│   └── sentiment_model.h5
│
├── README.md
├── requirements.txt
└── .gitignore
```

## Files
**1. `preprocess.py`**: Preprocesses the dataset for training.
**2. `train.py`**: Trains the sentiment analysis model.
**3. `analyze.py`**: Analyzes the sentiments in the tips and generates results.
**4. `sentiment_model.h5`**: The trained sentiment analysis model.

## Model Architecture
The model architecture is based on a Recurrent Neural Network (RNN) with Long Short-Term Memory (LSTM) units. This architecture is well-suited for processing sequential data like text and capturing contextual information for sentiment analysis.
