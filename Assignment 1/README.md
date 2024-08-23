# CS689A- Computational Linguistics for Indian Languages


## Assignment 1

### Name - Nitish Kumar
### Roll No - 231110033
### Dept. - M.Tech(C.S.E)

Note: I performed the whole operation on the corpus named as hi_100.txt due to constraints of my system.

It can be run on the original corpus file also named as hi_1000.txt present in the zip file.

## Libraries Used:
numpy  
matplotlib.pyplot   
pandas      
re   
transformers   
sentencepiece  
sklearn


## Steps to Run Assignment:

1. Extract the 231110033_assignment1.zip in your local system.

2. Open 231110033.ipynb file in your any environment either can be jupyternotebook, googlecollab or VisualStudioCode. Change the data path according to your file location(second cell).

3. Now run accordingly to each questions specified below.

## Question 1 :

To perform Unicode Correction-

Before performing unicode correction, I have taken a list of words from the extracted data file and 
cleaned it.

Step1: Firstly I have taken a list of space, vowel, special, matra, consonant along with a dictionary of matra that maps the matra's to the corresponding vowel.

Step2: If the word at position 'i' is a vowel (vowel) or space , there's no need for Unicode correction.

 
Step3: If word[i] is a consonant or in a special character then a '्' is added to word[i] then I will check the following conditions:

       
       a) If the next character after 'word[i]' is a consonant or a vowel, I'll correct it by appending the vowel 'अ' .

       b) If the next character after 'word[i]' is a matra, I'll match the matra to its corresponding vowel and append that vowel to 'word[i]'.

       c) If 'word[i]' corresponds to the last consonant in the word, I'll append the vowel 'अ' to it.

       d) If the next character after 'word[i]' is '्' or any other diacritic mark, I'll skip it.

Step4: If 'word[i]' represents a matra, I'll verify whether 'word[i-1]' is one of the following characters: [',','_','|','-','(',')','[',']','!','?','"','{','}','^','*','%','/',':-','।','.','़']. If it is, then I'll associate the matra with its corresponding vowel.

Example: त् आ र् ई ख् अ  is the unicode corrected word for तारीख

## Question 2 :

Here token is considered as a white-spaced separated sequence of characters
and for each token the characters and syllables are found out and storing a list of them and the tokens 
in descending order of their frequencies.

For obtaining syllables 2 methods have been defined get_syllables and get_Vyanjan
for otaining the syllables in a word
if word[k] is a vowel it will be considered a syllable
if word[k] is a consonant then to obtain the syllables check the following conditions 
by using method get_Consonant:

1. if work[k+1] is a consonant then return word[k] as syllable
2. if work[k+1] is a vowel or a matra  then return word[k]+word[k+1] as syllable
3. if word[k+1] is a '्'  then return word[k]+word[k+1]+get_Vyanjan as a syllable
 i.e recurssively call the get_Vyanjann method to obtain the syllable
4. if word[k] is last character simply return it as a syllable
5. if k exceeds word length return null

After obtaining the list of characters and syllables I stored a list of them in descending order of their
frequencies and then I finded the top-20 frequent uni-gram and bi-gram frequencies of characters and syllables. 

## Question 3 :


3rd question I did on the website provided to us at https://bangla.iitk.ac.in/cs689/main where I formed word groups by taking consideration of semantic unit that includes inflections, verb auxiliaries, and compounds in a hindi language sentence.

## Question 4 :

I performed the operations Unigram, BPE (vocabulary sizes, V = 1k, 2k), mBERT (max length = 1k,
2k), IndicBERT (max length = 1k, 2k), and White-space tokenizers on the entire corpus. 
Then I find the unigram frequencies of tokens and bi-gram frequencies of tokens, syllables, and characters for each of the tokenizers with the libraries available mentioned above.

## Question 5 :

Now I stored my ground truth set in a text file named as ground_truth_value, Then For each tokenizer in Question 4, 
I find the precision, recall and F-score for the 25 sentences provided to us. 

## Question 6 :

It contains the comparison info about all the models that I used. 



