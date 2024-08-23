# CS689A- Computational Linguistics for Indian Languages


## Assignment 2

### Name - Nitish Kumar
### Roll No - 231110033
### Dept. - M.Tech(C.S.E)

Note: Due to the limitations of the system, I selected the value of epochs to 3 and model training data size to 20000



## Libraries Used:
numpy    
pandas      
transformers   
sklearn   
accelerate  
datasets
seqeval


## Steps to Run Assignment:

1. Extract the 231110033_assignment2.zip in your local system.

2. Now there are two ipynb files separately(one for IndicBert and one for IndicNER, with their name respectively)

3. Now run each cell either in kaggle(more preferably) or google collaboratory

## Question 1 :

Identify the named entities for a set of 25 sentences and mark them in BIO format.


Step1: As discussed in the class I have assigned named entities to all the words with the help of classes PER (person), LOC (location), ORG (organisation), MISC (miscellaneous)
and O (for others, i.e., non NEs)

Step2: As mentioned in the question there is a file called "1 Ans) Manually Annotated Sentences" inside the zip folder and also I have submitted that on the website given https://bangla.iitk.ac.in/cs689/



## Question 2 :

In the second question we had to Fine-tune IndicBERT and IndicNER model on the Naamapadam corpus, I chose my mother tongue HINDI with train 70%, 10% validation, and 20% test set splits as already given in the
corpus. 

I used GPU from Kaggle for this.
IndicNER model is available at https://huggingface.co/ai4bharat/IndicNER whereas IndicBERT
is available at https://huggingface.co/ai4bharat/indic-bert.


This is done in two python notebook files (IndicBERT and IndicNER).

Inside itself comparison is done and macro-F1 score is mentioned.


## Question 3 :


For 3rd question I passed the all 25 sentences mentioned on the website where we manually annotated NER tags to the ChatGPT which is present inside the zip folder with name "3 Ans) ChatGPT"

## Question 4 :

I did this part in the both notebook filese itself, which can be checked via going at the last of the code.

## Question 5 :

For this question I submitted the report.pdf file which is present inside the zip folder.




