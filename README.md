# exam_automation
The goal is to automate the paper correction process even for lengthy answers for different subjects.
### THE END GOAL
Building a conceptual , semantic similarity machine learning model and wrap a scoring above it.
Plug it wih the web-app and develop a strategy for model maintenance and monitoring
The current experiment is being done for Operating Systems subject in SRM university
## MODEL CONSTRUCTION USING SIAMESE-LSTM
Inspired from Tensorflow Implementation of https://github.com/dhwajraj/deep-siamese-text-similarity <br /> 
### Referrences:
https://colah.github.io/posts/2015-08-Understanding-LSTMs/ <br /> 
https://colah.github.io/posts/2014-07-NLP-RNNs-Representations<BR />
Using MaLSTM model(Siamese networks + LSTM with Manhattan distance) to detect semantic similarity between question pairs. Training dataset used is a subset of the original Quora Question Pairs Dataset(~363K pairs used).<BR />
<B>FOR THE SAKE OF MODEL CONSTRUCTION AND SELECTION, WE ARE USING KAGGLE'S QUORA QUESTION PAIRS TO TRAIN THE MODEL INITIALLY, WHILE THE DATA COLLECTION IS BEING DONE.</B><BR />
<B>Data</B><BR />
GoogleNews-vectors-negative300.bin.gz<BR />
Kaggle's Quora Question Pairs Dataset<BR />
Kaggle's test.csv is too big, so I had extracted only the top 20 questions and created a file called test-20.csv and It is used in the predict.py.

## DATA COLLECTION
OVERVIEW :<BR />

This is a common platform for simulating and uploading sentence pairs and answer keys for model training and testing.<BR />

Features:<BR />

<B>Add Subject and exam:</B> Feature to add any subject and exam<BR />
<B>Add Question:</B> Feature to add question for given subject for exam/simulation<BR />
<B>Simulate Question:</B> Fetch the questions with type = simulation and simulate different sentences for the answers with various type of variations and upload back to the training collection.<BR />
<B>Type Answers:</B> For given question with type = exam upload the answers written by students for that question<BR />
<B>Correct Answers:</B> For a given student, given exam, given question, correct answers. Match the following sentences pairs and submit back to test collection set.<BR />
LINK TO THE PORTAL: http://157.245.100.55/ <BR />
<B>SCREENSHOT.DOC CONSISTS OF THE A FEW SNAPS OF OUR DATA COLLECTION PLATFORM</B><BR />
Data collection has already been done by collecting examination answers written by students.
