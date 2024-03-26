The first step is retrieving the CSV file's data into the Data frame. After retrieving the data, we done the data preprocessing to improve the model's performance.

Before creating the word cloud, we cleaned the output variable, removed the HTML entities using the BeautifulSoup function, and then used a regular expression to replace the 
hashtags, @, URLs, and non-alphabetic characters with whitespace. Then created a new column in the data frame with a cleaned output variable. Finally, we concatenated all the 
values from the output variable into a single variable and converted them into lowercase using the string function.

We have created a word cloud for each genre with the frequency of the top 15 words using the Word Cloud Library. To display the word cloud diagram, we used matplotlib. Plot 
library. Also created a word cloud for all the genres with a total of 60 words.

Next, we created a simple classification model using the Naïve Bayes Classifier algorithm. Then we split the data into train and test data. To evaluate the performance of the 
model, we used metrics like accuracy, precision, recall, and f1-score. Also, find the confusion matrix for the model. To find those metrics we used the StratifiedFold library 
with 10-fold cross-validation.
