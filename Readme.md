# Tweets Sentiment Analysis

## Overview
This project implements a sentiment analysis model to classify tweets as positive or negative using a Random Forest classifier. The model leverages Natural Language Processing (NLP) techniques to preprocess text data and extract meaningful features for classification.

## Table of Contents
- [Installation](#installation)
- [Usage](#usage)
- [Data](#data)
- [Model Training](#model-training)
- [Results](#results)
- [Contributing](#contributing)
- [License](#license)

## Installation
To set up the project, clone the repository and install the required packages:

```bash
git clone https://github.com/akshargrover/tweet-sentiment-analysis
cd tweet-sentiment-analysis
pip install -r requirements.txt
```

## Usage
To run the sentiment analysis model, execute the following command in your terminal:

```bash
python twitter-sentiment-analysis.ipynb
```

This will train the model on the training dataset and evaluate it on the test dataset.

## Data
The dataset used for training and testing consists of tweets labeled as positive or negative sentiment. The data is split into training and test sets to evaluate the model's performance.

- **Training Data**: Contains tweets used to train the model.
- **Test Data**: Contains tweets used to evaluate the model's accuracy.

## Model Training
The model is built using the following steps:

1. **Data Preprocessing**: 
   - Text normalization (lowercasing, removing punctuation, etc.)
   - Tokenization and lemmatization using spaCy
   - Vectorization using TF-IDF to convert text into numerical features.

2. **Model Selection**: 
   - A Random Forest classifier is used for its robustness and ability to handle high-dimensional data.

3. **Hyperparameters**:
   - `n_estimators`: 200 (number of trees in the forest)
   - `max_depth`: 15 (maximum depth of the trees)
   - `class_weight`: 'balanced' (to handle class imbalance)

## Results
The model's performance is evaluated using accuracy, precision, recall, and F1-score metrics. The results are printed in the console after running the model.

### Example Output:

## Contributing
Contributions are welcome! Please open an issue or submit a pull request for any improvements or bug fixes.

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
