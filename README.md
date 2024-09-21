# Programming Tag Generator from Quora Questions
Project Overview<br>
This project aims to process and analyze a large dataset of questions sourced from Quora, specifically focusing on programming-related questions. The goal is to extract meaningful tags (or keywords) from each question, including both its title and body, using Natural Language Processing (NLP) techniques and machine learning models. These tags can then be used to categorize and index questions effectively, enhancing searchability and organization.<br>

The project involves cleaning, preprocessing, and transforming the raw text data into useful features, followed by tag generation using both statistical methods (e.g., TF-IDF) and machine learning approaches. It specifically handles questions that may include programming code and aims to preserve relevant keywords while excluding unnecessary information such as HTML tags.<br>

Key Features<br>
Data Preprocessing:  

Cleaning raw text by removing HTML tags, special characters, and unnecessary code blocks.  
Tokenizing and stemming words for more efficient text processing.  
Removing stopwords to retain only meaningful keywords.  
Handling Programming Code:  

Detecting and extracting programming code segments embedded in questions.  
Separating code from the question content to ensure accurate tag extraction.  
Counting and analyzing questions containing code.  
TF-IDF Vectorization:  

Converting the cleaned questions into numerical features using the TF-IDF (Term Frequency-Inverse Document Frequency) vectorizer.  
Using n-grams (unigrams, bigrams, trigrams) to capture both individual words and multi-word phrases.  
Tag Extraction:  

Generating tags based on keyword frequency across the entire dataset.  
Employing multilabel classification techniques to assign the most relevant tags to each question.  
Selecting the top n most frequent tags for a more focused analysis.  
Performance Metrics:  

Calculating and reporting statistics such as the average length of questions before and after processing.  
Measuring the percentage of questions that contain programming code.  
Evaluating how many questions are explained by the top n tags.  

Technologies Used  
Python: Primary programming language.  
NLTK: Natural Language Toolkit for text processing.  
scikit-learn: For machine learning, specifically for TF-IDF vectorization and multilabel classification.  
SQL: For storing processed data (optional).  
pandas: For data manipulation and handling.  
NumPy: For numerical operations.  
re: Regular expressions for text cleaning.  
Dataset  
The dataset used in this project consists of questions and answers from Quora, with a focus on programming-related content. Each entry in the dataset includes the following fields:  

Title: The title of the question.  
Question: The body of the question, which may include embedded code.  
Tags: Pre-existing tags or labels for the question.  
Future Enhancements  
Improve the tag recommendation system by training more advanced machine learning models like BERT or GPT.  
Enhance code snippet extraction and handling to better categorize questions with significant code content.  
Incorporate deep learning techniques to automatically generate more sophisticated tags based on question content.  
License  
This project is licensed under the MIT License. See the LICENSE file for details.  
