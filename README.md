# Transaction Description Categorization using NLP

## Introduction
This project aims to develop a natural language processing (NLP) model to categorize transaction descriptions into predefined categories. The model utilizes techniques such as text preprocessing and LSTM-based neural networks to classify transaction descriptions accurately.

## Approach
The project follows these main steps:
1. Data Preprocessing: Clean and preprocess transaction descriptions by removing special characters, lowercasing, tokenization, and lemmatization.
2. Model Development: Build an LSTM-based NLP model using TensorFlow/Keras to classify transaction descriptions into categories.
3. Training and Validation: Train the model using the provided dataset, validating its performance on a subset of the data.
4. Model Evaluation: Evaluate the model's effectiveness in categorizing transaction descriptions using accuracy as the primary metric.

## Data Preprocessing
The text data undergoes several preprocessing steps:
- Removal of special characters and punctuation.
- Lowercasing of text.
- Tokenization of text into words.
- Lemmatization of words to their base form.

The NLTK library is utilized for tokenization and lemmatization.

## Model Development
The NLP model architecture consists of:
- Embedding layer: Converts text tokens into dense vectors.
- LSTM layers: Captures sequential patterns in text data.
- Dense layers: Perform classification based on LSTM outputs.

The model is compiled with the Adam optimizer and sparse categorical cross-entropy loss function.

## Training and Validation
The model is trained for 10 epochs with a batch size of 32, using a validation split of 20% of the training data. Training progress, including loss and accuracy metrics, is monitored during the process.

## Model Evaluation
The model's effectiveness is evaluated using accuracy as the primary metric. Additional evaluation metrics such as precision, recall, and F1-score may also be considered for a comprehensive analysis.

## Instructions for Running the Code
To run the code:
1. Install required libraries using `pip install pandas numpy nltk scikit-learn tensorflow`.
2. Download NLTK data by running `nltk.download('stopwords')` and `nltk.download('wordnet')`.
3. Ensure the dataset file `Spending_Pattern_Dataset.xlsx` is available in the same directory as the code.
4. Execute the code in a Python environment, following the instructions provided in the code comments.

## Conclusion
The NLP model demonstrates promising results in categorizing transaction descriptions accurately. Further optimization and fine-tuning may be explored to improve the model's performance and scalability.



