# Spam Detection Using Naive Bayes

This project uses a Naive Bayes classifier to detect spam messages in SMS data. The model is trained on the `spam.csv` dataset, which contains labeled SMS messages as either "ham" (not spam) or "spam."

## Table of Contents

- [Overview](#overview)
- [Dataset](#dataset)
- [Dependencies](#dependencies)
- [How to Run](#how-to-run)
- [Preprocessing](#preprocessing)
- [Model Evaluation](#model-evaluation)
- [Sample Output](#sample-output)
- [Contributing](#contributing)
- [License](#license)

## Overview

The goal of this project is to classify SMS messages as either spam or not spam (ham). A Multinomial Naive Bayes classifier is used for text classification. The text data is preprocessed by converting it to lowercase, removing punctuation, and eliminating stopwords before being converted into numerical feature vectors using `CountVectorizer`.

## Dataset

The dataset used in this project is `spam.csv`, which contains SMS messages labeled as "ham" or "spam." You can download the dataset from the following link:

**Kaggle:** [SMS Spam Collection Dataset](https://www.kaggle.com/datasets/uciml/sms-spam-collection-dataset)

Place the `spam.csv` file in the root directory of this project.

## Dependencies

To run this project, you need the following Python libraries installed:

- `numpy`
- `pandas`
- `scikit-learn`
- `nltk`

You can install all dependencies using the following command:

```bash
pip install -r requirements.txt
```

Additionally, ensure that you have downloaded the NLTK stopwords corpus by running:

```bash
python -m nltk.downloader stopwords
```

## How to Run

1. Clone this repository:
   ```bash
   git clone https://github.com/jagadeepdandu/spam-detection.git
   ```
2. Change into the project directory:
   ```bash
   cd spam-detection
   ```
3. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```
4. Download the NLTK stopwords:
   ```bash
   python -m nltk.downloader stopwords
   ```
5. Place the `spam.csv` dataset in the root directory of the project.
6. Run the script:
   ```bash
   python spam_detection.ipynb
   ```

## Preprocessing

The text data undergoes the following preprocessing steps:

- **Lowercasing**: All text is converted to lowercase to ensure uniformity.
- **Punctuation Removal**: Punctuation marks are removed to reduce noise.
- **Stopword Removal**: Common English stopwords (e.g., "the", "is", "and") are removed using NLTK's stopwords list.

## Model Evaluation

The performance of the model is evaluated using the following metrics:

- **Accuracy**: Percentage of correctly classified messages.
- **Confusion Matrix**: Shows the number of true positives, true negatives, false positives, and false negatives.
- **Classification Report**: Includes precision, recall, F1-score, and support for each class.

## Sample Output

Example output from running the model:

```
Accuracy: 97.5%

```

## Contributing

Contributions are welcome! If you find any issues or have suggestions for improvement, feel free to open an issue or submit a pull request.

## License

This project is licensed under the **MIT License**. Feel free to use and modify it as needed.

