# Email-Spam-Classification-ML
This project aims to utilize Python text classification techniques to identify or classify spam emails. By applying suitable algorithms such as Naive Bayes, Multinomial Naive Bayes, and J48 on an email dataset, we will determine the accuracy, processing time, and error rate to compare which algorithm performs best for text classification.  
The dataset was collected from Kaggle(Email Spam classification Dataset)  
Then punctuation and "Subject" was removed from the dataset.  
Used Countvectorizer and TF-IDF as part of the preprocessing step, to convert word into numerical repreentation.  
TF-IDF: convert the words into vector based on the frequency of the word.  
Split the data set into 30% testing data and 70% training datatset.  
Then provided the training dataset to NaiveBayesMultinomial model.  


## Project Structure

- `emails.csv`: Dataset containing email texts labeled as spam (1) or ham (0).
- `email_classifier.ipynb`: Jupyter notebook containing the code for preprocessing, training the classifier, and evaluating its performance.
- `README.md`: This file, providing an overview of the project.

## Setup

### Libraries Used

- `numpy`
- `pandas`
- `matplotlib`
- `seaborn`
- `sqlite3`
- `sklearn`
- `nltk`

### Installation

To run the code, install the required libraries:

```bash
pip install numpy pandas matplotlib seaborn scikit-learn nltk
```

## Dataset
The dataset (emails.csv) contains email texts and their corresponding labels (spam or ham). It is loaded and processed using pandas.

## Data Preprocessing
- HTML tag removal, lowercase conversion, punctuation removal, and other text preprocessing steps are applied using regular expressions and NLTK.
## Feature Extraction
- CountVectorizer: Used to convert text data into numerical feature vectors based on word counts.
## Model Training
- Multinomial Naive Bayes: A probabilistic classifier suitable for text classification tasks, trained on the feature vectors derived from the email texts.
## Model Evaluation
- **Confusion Matrix:** Visualized using seaborn's heatmap to show true positives, true negatives, false positives, and false negatives.
- **Classification Report:** Provides precision, recall, F1-score, and support metrics for both spam and ham classes.
## Results
After training and evaluation:

**Accuracy:** Achieved accuracy of 98.69% on the test set.
**Best Parameters:** Found using GridSearchCV for TF-IDF and MultinomialNB pipeline.
**Example Predictions:** Demonstrated classification of sample emails into spam or ham categories.
## Usage
1. Clone the repository:
   ```
   git clone https://github.com/your-username/email-classifier.git
cd email-classifier```
2. Open and run `email_classifier.ipynb` in Jupyter notebook.
3. Modify `new_email` and `dummy_emails` variables to test the classifier on new inputs.

