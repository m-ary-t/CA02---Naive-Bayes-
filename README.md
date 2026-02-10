# CA02---Naive-Bayes-
CA02: Spam eMail Detection using Naive Bayes Classification Algorithm

This notebook trains a model using Gaussian Naive Bayes Classification Algorithm with a set of emails, 
labelling them as either Spam or Not Spam. The data includes 702 emails equally divided into spam and 
non spam categories. Two folders are provided, train-mails and test-mails, containing the emails that 
will be used to train the model and then test it. The model will use 260 emails to test the model and 
predict their category and then compare the accuracy with the correct classification that we already know.

**Summary**

This notebook trains a model using Gaussian Naive Bayes Classification Algorithm to determine whether or not an email is spam.
This notebook builds a spam vs. not‑spam classifier for emails using a Guassian Naive Bayes model. You'll train the model to determine the most common 3,000 words that appear in the files of emails, evaluate the frequency in which those words appear in each email, and having the classification of these emails provided to the model, the model will learn how to identify emails as spam or not. Then you will test the model to determine its overall accuracy.

**Data**

Two folders are provided, train-mails and test-mails. The model will be trained using the 702 emails, with an equal amount of spam and non-spam emails, in the train-mails folder.
The model will then be tested for its accuracy using the 260 emails in the test-mails folder. Files starting with spmsg... are spam and files like number-numbermsg[number].txt are not spam. The files were provided to us by Dr. Brahma. 

**Environment & Dependencies**

- Python 3.x
- The libraries needed to run this notebook include:
  - os: used for interacting with the operating systems to work with files and directories
  - numpy: used for numerical computing like mathematical computation and fast array and matrix operations
  - collections.Counter: used for count occurrences of items in a list, string, or other iterables
  - scikit-learn for 
      - GaussianNB: Gaussian Naive Bayes classifier
      - accuracy_score: function that calculates how accurate a classifier is
 
**How to Run**

- Download the test-mails and train-mails folders and the CA02_NB_assignment.ipynb file
- Save and place the folders & file into the same folder on your computer or Google Drive
- Ensure the data folders are present and named exactly: './train-mails' and './test-mails'
- Run the cells from top to bottom

**Sources**

- Utilized Google Copilot to determine what packages and funcitons were needed to run a Gaussian Naive Bayes classification algorithm. 
