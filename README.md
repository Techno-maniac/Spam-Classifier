# Spam-Classifier
Spam classifier is a program that uses a machine-learning algorithm to classify a mail as a spam or a no spam.
# Step by step instructions:
1. Download and extract Spam Classifier.zip file. (3 directories and 4 files)<br />
<br />
  Directories:<br />
1.sample_mails Dir: Five emails as txt files. These emails are completely unknown to our model and will get classified one by one<br />
2.Spam Dir: Should be empty before execution. This dir will store the emails classified as spam<br />
3.Non Spam Dir: Should be empty before execution. This dir will store the emails classified as non spam<br />
<br /> 
<br />
  Files:<br />
1. spam_classifier.py: Main python code to execute<br />
2. spamTest.mat: File has testing data set "Xtest" and it's labels as "ytest". Xtest has data of 1000 emails and each mail has 1899 features. ytest has 1000 labels. Xtest Dimension = (1000, 1899) and ytest Dimension = (1000, 1)<br />
3. spamTrain.mat: File has training data set "X" and it's labels as "y". X has data of 4000 emails and each mail has 1899 features. y has 4000 labels. X Dimension = (4000, 1899) / y Dimension = (4000, 1)<br />
4. vocab.txt: Our vocabulary list was selected by choosing all words which occur at least a 100 times in the spam corpus, resulting in a list of 1899 words.In practice, a vocabulary list with about 10,000 to 50,000 words is often used.<br />
<br />
<br />

  Data:<br />
1. In our program we have combined spamTest.mat and spamTrain.mat so the combined data has 5000 mails and each mail has 1899 features. Dimension of our data is (5000, 1899) and Dimension for labels is (5000, 1)<br />
2. Each mail has 1899 features and value of each feature will be either 0 or 1 depends on the presence or the absence of the words in our email.<br />
3. Value of each label is either 0 or 1. y=0 is non spam and y=1 is spam.<br />
