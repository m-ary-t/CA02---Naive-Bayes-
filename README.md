# CA02 – Spam Email Classification using Naive Bayes

**Overview**
This assignment implements a spam email classifier using the Gaussian Naive Bayes algorithm.
Emails are processed from training and testing folders, converted into numerical features based on word frequencies, and used to train and evaluate a machine learning model.

**Dataset Structure**

The dataset is organized into two main folders:
- train-mails/ – emails used to train the model
- test-mails/ – emails used to evaluate the model

The model will be trained using the 702 emails, with an equal amount of spam and non-spam emails, in the train-mails folder.
The model will then be tested for its accuracy using the 260 emails in the test-mails folder. 
Files starting with spmsg... are spam and files like number-numbermsg[number].txt are not spam. 
The files were provided to us by Dr. Brahma.

**Environment & Dependencies**

- Python 3.x
- The libraries needed to run this notebook include:
  - os: used for interacting with the operating systems to work with files and directories
  - numpy: used for numerical computing like mathematical computation and fast array and matrix operations
  - collections.Counter: used for count occurrences of items in a list, string, or other iterables
  - scikit-learn for 
      - GaussianNB: Gaussian Naive Bayes classifier
      - accuracy_score: function that calculates how accurate a classifier is
  
**Methodology**

Dictionary Creation (make_Dictionary)
  - Reads all training emails.
  - Extracts words from the email body.
  - Removes non-alphabetic tokens and single-character words.
  - Keeps the 3,000 most frequent words to form the dictionary.

Feature Extraction (extract_features)
  - Converts each email into a numeric feature vector.
  - Each feature represents the frequency of a dictionary word in the email.
  - Assigns labels:
      - 1 → spam
      - 0 → non-spam

Model Training
  - Trains a Gaussian Naive Bayes classifier using the training feature matrix and labels.

Prediction and Evaluation
  - Uses the trained model to predict labels for test emails.
  - Computes classification accuracy by comparing predicted labels to true labels.

**Results**

The model achieves an accuracy of approximately:
Accuracy ≈ 96.5%
This indicates strong performance in distinguishing spam emails from non-spam emails using word-frequency features.

**How to Run**

- Download the test-mails and train-mails folders and the CA02_NB_assignment.ipynb file
- Save and place the folders & file into the same folder on your computer or Google Drive
- Ensure the data folders are present and named exactly: './train-mails' and './test-mails'
- Run the cells in order from top to bottom:
    - Setting File Path (if using Google Colab)
    - Dictionary creation
    - Feature extraction
    - Pulling Training and Testing Folders
    - Model training
    - Prediction and accuracy evaluation
- The final output will display the model accuracy and indicate successful completion.

**Conclusion**
This project demonstrates a complete machine learning pipeline for text classification, including preprocessing, feature engineering, model training, and evaluation. Gaussian Naive Bayes performs effectively for spam detection when combined with a frequency-based text representation.

**Sources**

- Utilized Google Copilot to determine what packages and funcitons were needed to run a Gaussian Naive Bayes classification algorithm. 
