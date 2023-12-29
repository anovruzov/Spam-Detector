Spam Classification Using Naive Bayes
Overview
This Python script applies the Naive Bayes algorithm to classify emails into 'spam' or 'ham'.
It uses a dataset containing email texts and their corresponding labels.
The script features preprocessing of email data, training a Multinomial Naive Bayes classifier, evaluating its performance,
and saving the model for future predictions.

Requirements
Python 3.x
pandas
scikit-learn
joblib
Ensure you have the above Python libraries installed. You can install them using pip:

sh
Copy code
pip install pandas scikit-learn joblib
Dataset
Your dataset should be a CSV file with two columns:

text: Contains the content of the email.
label: Contains the labels ('spam' or 'ham') for each email.
Update the path to your CSV file in the script where indicated.

Usage
To run the script, navigate to the directory containing the script and execute the following command:

sh
Copy code
python naiveBayes.py
Output
The script will output:

The percentage of emails classified as spam.
The accuracy of the model.
A classification report including precision, recall, and F1-score for both 'ham' and 'spam' classes.
Additionally, the trained model and the CountVectorizer will be saved to the local directory as 'naive_bayes_spam_model.pkl' and 'count_vectorizer.pkl', respectively.

Model Saving
The script saves the trained classifier and the vectorizer using joblib for later use. You can load the model and vectorizer to classify new emails.

Contribution
Feel free to fork this project and submit pull requests. You can also open an issue if you find any bugs or have any suggestions for improvements.
