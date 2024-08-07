# Module 21 Challenge - SMS Spam Detector

## Background
In the assignment,, you'll be refactoring code from an SMS text classification solution into a function that constructs a linear Support Vector Classification (SVC) model. Once the model is created and trained, you will create a Gradio app to host the application, enabling users to test text messages. The application will provide feedback to users, indicating whether the text is classified as spam or not, based on the model's performance.

## Code Source
The code location is: [Click Here to view](https://github.com/jaidevkler/sms_spam_detector)

## Files
gradio_sms_text_classification.ipynb [Click here to view](https://github.com/jaidevkler/sms_spam_detector/blob/main/gradio_sms_text_classification.ipynb)<br />
sms_text_classification_solution.ipynb [Click here to view](https://github.com/jaidevkler/sms_spam_detector/blob/main/sms_text_classification_solution.ipynb)<br />
SMSSpamCollection.csv [Click here to view](https://github.com/jaidevkler/sms_spam_detector/blob/main/Resources/SMSSpamCollection.csv)<br />

## How to run the program
Download the files and then use jupyter notebook or jupyter lab to open the gradio_sms_text_classification.ipynb file.<br />

## Challenge Instructions


### 1. Create the SMS Classification Function
* Using the code in the sms_text_classification_solution.ipynb file, create the sms_classification function in the gradio_sms_text_classification.ipynb by doing the following:
    * Set the features variable to the text message column of the DataFrame.
    * Set the target variable to the "label" column of the DataFrame.
    * Split data into training and testing and set the test_size to 33%.
    * Build a pipeline to transform the test set to compare to the training set.
    * Fit the model to the transformed training data and return model.<br />
* Load the SMSSpamCollection.csv into a DataFrame and call the sms_classification function with the DataFrame, and set the result to the "text_clf" variable.

### 2. Create the SMS Prediction Function

* Use the sms_prediction function to predict the classification of a new text by doing the following:
    * Create a variable that will hold the prediction of a new text.
    * Use a conditional statement that determines if the text message is "ham" or “spam”.
        * If the message is “ham”, the function should return the following message: f'The text message: "{text}", is not spam.'
        * If the message is spam, the function should return the following message: f'The text message: "{text}", is spam.'

### 3. Create the Gradio Interface Application

* Create a Gradio Interface application that takes a textbox for the inputs and has a textbox for the output. The textboxes should have labels that describe what each textbox contains.
* Launch the application and provide the URL to share the application.

* Use the following text messages to test your application.
    * You are a lucky winner of $5000!
    * You won 2 free tickets to the Super Bowl.
    * You won 2 free tickets to the Super Bowl. Text us to claim your prize.
    * Thanks for registering. Text 4343 to receive free updates on medicare.

## Reference
Columbia AI Bootcamp - Module 21 Challenge<br />
