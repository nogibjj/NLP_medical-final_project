# Document Classification on Patient Discharge Summaries

**Contributors**: Simrun Sharma (SS1486) | Titus Robin Arun (TRA29)

## Abstract

We employ Natural Language Processing (NLP) to categorize medical discharge summaries by smoking status into four categories: current smokers, non-smokers, past smokers, and unknown. Our study leverages a Naive Bayes model for its efficiency in textual classification and BERT Clinical for its deep understanding of medical language nuances. The Naive Bayes model reached an 80% accuracy with an F1 score of 0.8031, while BERT Clinical demonstrated a notable accuracy improvement on real data from 61.2% to 98.5%. This project underscores the potential of combining classical and advanced NLP methods in medical document classification.

## Dataset

Sourced from the i2b2 NLP data sets, our dataset addresses the challenge of identifying patient smoking status from medical discharge records, marked by fragmented English free text. De-identified and annotated by pulmonologists, the dataset includes five smoking status categories and presents a unique challenge for linguistic processing and retrieval in medical language processing technologies.

## Preprocessing Steps

Our preprocessing pipeline involved:

- **Label Encoding**: Conversion of "Smoking Status" into numerical labels.
- **Text Cleaning**: Standardization of text data and extraction of relevant information via regex.
- **Class Modification**: Merging similar classes to address imbalance, resulting in four distinct categories.

| Step                | Description                                                                 |
|---------------------|-----------------------------------------------------------------------------|
| Label Encoding      | Convert "Smoking Status" to numerical labels                                |
| Text Cleaning       | Lowercase conversion and regex for relevant info extraction                 |
| Class Modification  | Merge "SMOKER" with "PAST SMOKER" to reduce class imbalance                 |

## Models Overview

### Naive Bayes

- **Purpose**: Establish a quick analytical baseline for smoking status classification.
- **Performance**: Achieved 80% accuracy with an F1 score of 0.8031 on unseen test data.

### BERT Clinical

- **Purpose**: Deeply understand medical language nuances for accurate classification.
- **Performance**: Improved accuracy on real data to 98.5% but demonstrated limitations with synthetic data.

## Evaluation Metrics

- **Accuracy**
- **Precision**
- **Recall**
- **F1 Score**

## Future Directions

- **Data Refinement**: Focus on cleaner, more specific data related to patient smoking and social history.
- **Dataset Expansion**: Larger datasets to leverage models like BERT more effectively.
- **Model Exploration**: Consideration of RNNs or LSTM models for future iterations.

