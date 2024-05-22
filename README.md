# Merchant Category Code (MCC) Classification

This project aims to classify merchant transactions into appropriate MCC categories based on their merchant names using Natural Language Processing (NLP) techniques.

## Overview

Merchant Category Codes (MCCs) are four-digit numbers used to classify a business by the type of goods or services it provides. This project builds a model to automate this classification process, potentially aiding financial institutions, payment processors, or businesses in analyzing transaction data.

## Dataset

The model is trained on a dataset (`mcc_merchant_data.csv`) containing merchant names and their corresponding MCCs. 

## Methodology

1. **Data Preprocessing:**
   - Handled missing values and duplicates.
   - Converted merchant names to lowercase.
   - Tokenized and lemmatized merchant names using NLTK.
   - Encoded MCC categories into numerical labels.

2. **Model Development:**
   - Used a Support Vector Machine (SVM) classifier with a linear kernel.
   - Text features were vectorized using TF-IDF (Term Frequency-Inverse Document Frequency).
   - The model was trained on 80% of the data and validated on the remaining 20%.

3. **Model Evaluation:**
   - Evaluated using accuracy as the primary metric.
   - Achieved 0.33 accuracy on the validation set.

## How to Run

1. **Clone Repository:**
   ```bash
   git clone https://github.com/Rafay183/NLP_assesment_hugo.git


  2. Install Dependencies:

  pip install -r requirements.txt


3. Download NLTK Data:

```python -c 
import nltk; 
nltk.download('punkt'); 
nltk.download('stopwords'); 
nltk.download('wordnet')

   4. Run Notebooks:

Execute the following Jupyter Notebooks :
NLP_Model_development.ipynb

