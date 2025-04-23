# sms_spam_detector
# Description
This program uses data in the ./Resources directory called SMSSpamCollection.csv.  In this file are example texts with labeled data identifying if the message is spam or ham.  A sms_classification function is defined and uses TfidfVectorizer and SVM to model the presence of spam.  A sms_prediction function is also defined such that a user can input a text and have the model determine if it is spam.  In addition to using the sms_prediction function in the notebook, the user can also use two Gradio interfaces to get the prediction.  One Gradio interface uses HTML and one does not.  To enable one function for everything, the sms_prediction function takes the message, mode, and html inputs.  The message is a string, the mode is either "full", "message", or empty.  Full returns the whole message and the classification, message returns just the message, and empty returns just the classification.
# Data source
- SMSSpamCollection.csv
# Dependencies
- pandas
- sklearn.model.selection
- sklearn.pipeline
- sklearn.feature_extraction.text
- sklearn.svm
#Python version
- 3.12.7
