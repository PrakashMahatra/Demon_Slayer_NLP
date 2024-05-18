# Demon Slayer Classification and Relationship Analysis Project
![Demon Slayer Logo](https://fictionhorizon.com/wp-content/uploads/2021/05/Dizajn-bez-naslova-1024x576.jpg)

## Overview

This project combines machine learning techniques for character classification and Natural Language Processing (NLP) analysis of relationships between characters from the "Demon Slayer" series. The classification aspect identifies characters as either human or demon based on their characteristics such as name, breathing style, and description. The relationship analysis extracts and visualizes interactions between characters from subtitles.

## Dataset

The dataset consists of information about various characters from the "Demon Slayer" series, including their names, whether they are human or demon, their breathing style, and a description of their abilities and characteristics. Additionally, subtitles from the series are processed to extract relationships between characters.

## Model and Training

### Classification (Project 1.1)

We use the AutoTokenizer to tokenize the text data and prepare it for input to the sequence classification model. The model used for classification is AutoModelForSequenceClassification from the Transformers library. We define a custom Trainer class for training the model, where we compute a custom loss function and metrics using DataCollatorWithPadding and evaluate module from Hugging Face.

#### Training Arguments

We define the training arguments including output directory, learning rate, batch size, number of epochs, weight decay, and evaluation and logging strategies.

### Relationship Analysis (Project 1.2)

In addition to classification, this project processes subtitles from the "Demon Slayer" series to extract relationships between characters using NLP techniques. The subtitles are cleaned using regular expressions, and named entities are extracted using spaCy. Relationships between characters are then analyzed and visualized.

## Results

After training the classification model and analyzing the relationships between characters, we evaluate the model's performance on a separate test dataset using metrics such as accuracy. We provide a classification report to summarize the model's performance in terms of precision, recall, and F1-score for each class.

## Usage

To replicate the experiment, follow these steps:

1. Install the required libraries: `transformers`, `evaluate`, `numpy`, `torch`, `pysubs2`, `glob`, `spacy`, `nltk`.
2. Prepare the dataset with the required columns: name, human/demon, breathing style, and description.
3. Tokenize the dataset using the AutoTokenizer.
4. Define the model, data collator, training arguments, and custom Trainer.
5. Train the model using the Trainer object.
6. Process subtitles using the provided script and extract named entities and their relationships.
7. Visualize the relationships between characters using the extracted data.

## Conclusion

This project demonstrates the application of machine learning techniques to classify characters from the "Demon Slayer" series and analyze relationships between characters using NLP techniques. By leveraging pre-trained models and custom training strategies, we achieve accurate classification results and gain insights into the interactions between characters.

## License

This project is licensed under the [MIT License](LICENSE).

 
