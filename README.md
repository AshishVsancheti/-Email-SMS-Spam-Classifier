# Email-SMS-Spam-Classifier
# PROJECT OVERVIEW
This project aims to develop a spam classifier utilizing machine learning methods to categorize emails and SMS messages as either spam or non-spam (ham). It encompasses tasks such as data cleaning, exploratory data analysis (EDA), preprocessing, and model construction to build an efficient spam detection system.
# STEPS
# 1. DATA LOADING
The dataset, sourced from Kaggle, formed the basis of this project.
# 2. DATA CLEANING
Unnecessary columns were removed from the dataset, and the remaining ones were renamed for better clarity. 
The target variable underwent label encoding to transform it into numerical values. 
Null and duplicate values were examined and managed, ensuring duplicate rows were retained only once.
# 3. EXPLORATORY DATA ANALYSIS (EDA)
The dataset was examined to detect any disparities between spam and ham categories. 
NLTK was imported for conducting Natural Language Processing (NLP) operations. 
Further attributes like character count, word count, and sentence count were extracted from each text. 
Tokenization of words and sentences was executed to aid in analysis. 
Descriptive statistics were utilized to investigate variances between spam and ham messages.
# 4. DATA PROCESSSING
Stopwords were obtained from the NLTK library and utilized to eliminate frequent, uninformative words. 
Text underwent conversion to lowercase, tokenization, and removal of special characters. 
Stemming was performed to standardize words. 
The processed text was saved in a new attribute named "transformed_text."
# 5. MODEL BUILDING
TF-IDF (Term Frequency-Inverse Document Frequency) vectorization was performed to convert the processed text into numerical attributes. 
The dataset was divided into training and testing subsets. 
Different machine learning algorithms such as Naive Bayes, Decision Tree, Random Forest, and Logistic Regression were implemented. 
Naive Bayes exhibited the highest precision compared to other models.

# IMPORTANT DETAILS
Data Cleaning: Identified null values in multiple columns led to the decision to eliminate columns with a significant null count. Column renaming and label encoding were executed for improved data clarity and model compatibility.

Tokenization and Text Preprocessing: Utilizing the NLTK library, tokenization separated text into words and sentences. Special characters were removed, and stopwords were filtered out to prep the text for analysis.

TF-IDF Vectorization: TF-IDF, chosen for its emphasis on unique words, was employed to vectorize the text. This technique, favoring uncommon words over common ones, is well-suited for text classification tasks.

Model Selection and Evaluation: Models such as Naive Bayes, Decision Tree, Random Forest, and Logistic Regression were selected for their adeptness with text data. Evaluation metrics encompassed accuracy, precision, recall, and F1-score, with precision prioritized due to dataset imbalance, focusing on minimizing false positives.

# CHALLENGES
Handling imbalanced data was essential, given the dominance of ham data over spam data. 
Ensuring thorough text preprocessing was vital for upholding data quality and maximizing model performance. 
Feature engineering played a pivotal role in improving model effectiveness. 
Addressing the challenge of minimizing false positives in a skewed dataset was a central focus during the analysis.

# CONCLUSION
The project effectively showcases the classification of emails and SMS messages into spam and ham categories. By employing TF-IDF vectorization and machine learning algorithms such as Naive Bayes, a robust spam classifier was developed.








