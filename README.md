# Credit_Risk_Analysis

##Purpose:

Credit Risk is inherently a classification problem, as to what qualification and standards a company takes in order to approve or denied loans is where data comes into play. The purpose of this Project is to run several analysis and machine learning language to create a system that can predict the credit risk taken on by the company. For this purpose we run the following analysis and machine learning techniques:

Undersample the data using the ClusterCentroids algorithm.
RandomOverSampler and SMOTE algorithms to oversample the data.
Use the LogisticRegression Classifier to make predictions and evaluate the model accuracy.
Compare two machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier

After running this modesl we hope to be able to use them for recomendation on whether they can be used for predicting credit risk or not.

##Results:
##RandomOverSampler
<img width="960" alt="Screen Shot 2022-01-16 at 11 05 15 PM" src="https://user-images.githubusercontent.com/90356052/149716264-f0161901-fc71-48bd-aed7-5bf418768998.png">
as you can see with the results of our over sample our precision score for high_risk is only 1% with a 62% sensitivity for the high riks. Comparing to the low risk where we got a precision score of 100% and sensitivity of 68%. Looking at the f1 Score we can see that that for high risk this model was only succesfull at 2% for high risk and 81% for our low risk
<img width="960" alt="Screen Shot 2022-01-16 at 11 32 34 PM" src="https://user-images.githubusercontent.com/90356052/149719153-0100ef83-ef24-4374-a0e3-bbbd9fe0060c.png">
<img width="537" alt="Screen Shot 2022-01-16 at 11 33 01 PM" src="https://user-images.githubusercontent.com/90356052/149719211-d422509b-4d7f-4251-86c7-9ccb07f1b65b.png">
 
 as you can see by the images above almost all of our models seem to suggest that it is good at predicting credit risk on the lower spectrum but not so effective at predicting the high risk.
<img width="537" alt="Screen Shot 2022-01-16 at 11 35 20 PM" src="https://user-images.githubusercontent.com/90356052/149719509-53eef3d8-1aeb-4ead-abc5-aa10a3afdb90.png">

in our assemble models our precision score for high risk increased by 3% recall didn't really change and stay in an average of 67%. We can see that precision did not change for low risk and recall actually increased for low risk as well to 91%.
##summary

All the models used to perform the credit risk analysis show weak precision in determining if a credit risk is high. However in almost all of our models the precission for low risk was 100% in all cases. the sensitivity in almost all of our models, however was above 50%. In conclusion our models are doing good at predicting low risk. They are not performing precision wise at high risk. Although this models are insightfull, due to the models precision score being to low on the high risk spectrum i would not suggest using this module. This module would cause the bank to let more high risk borrowers to fall through the cracks and be seeing as low risk. 

