# CS689A - Computational Linguistics for Indian Languages

### Name: Nitish Kumar  
### Roll No: 231110033  
### Dept.: M.Tech (C.S.E)

This repository contains the code and reports for three assignments completed as part of the Computational Linguistics for Indian Languages course. The assignments involve various tasks such as Unicode correction, tokenization, Named Entity Recognition (NER), and machine translation using state-of-the-art models like IndicBERT, IndicNER, and ChatGPT.

## Assignment 1

### Overview:
The first assignment focused on Unicode correction, tokenization, and frequency analysis of tokens, characters, and syllables in a Hindi corpus. It also included the implementation and comparison of different tokenization techniques.

### Libraries Used:
- `numpy`
- `matplotlib.pyplot`
- `pandas`
- `re`
- `transformers`
- `sentencepiece`
- `sklearn`

### Steps to Run Assignment:

1. Extract the `231110033_assignment1.zip` in your local system.
2. Open the `231110033.ipynb` file in any environment such as Jupyter Notebook, Google Colab, or Visual Studio Code. Update the data path in the second cell according to your file location.
3. Run the notebook cell by cell as per the questions specified below.

### Questions:

1. **Unicode Correction:**
   - Implemented a function to correct Unicode errors in a Hindi corpus by analyzing the sequence of vowels, consonants, and matras.
   - Example: The corrected form of the word `त् आ र् ई ख् अ` is `तारीख`.

2. **Tokenization and Frequency Analysis:**
   - Performed tokenization and extracted syllables using custom methods.
   - Computed top-20 frequent uni-gram and bi-gram frequencies of tokens, syllables, and characters.

3. **Word Group Formation:**
   - Grouped words based on semantic units such as inflections, verb auxiliaries, and compounds using the provided website tool.

4. **Tokenization Techniques:**
   - Evaluated Unigram, BPE, mBERT, IndicBERT, and White-space tokenizers.
   - Computed unigram and bi-gram frequencies for each tokenizer.

5. **Evaluation of Tokenizers:**
   - Compared the performance of different tokenizers by calculating precision, recall, and F-score for 25 sentences.

6. **Model Comparison:**
   - Summarized the comparative performance of the models used in the assignment.

## Assignment 2

### Overview:
The second assignment focused on Named Entity Recognition (NER) in Hindi using IndicBERT and IndicNER models, along with manual annotation and evaluation of NER tags.

### Libraries Used:
- `numpy`
- `pandas`
- `transformers`
- `sklearn`
- `accelerate`
- `datasets`
- `seqeval`

### Steps to Run Assignment:

1. Extract the `231110033_assignment2.zip` in your local system.
2. The zip file contains two separate `.ipynb` files for IndicBERT and IndicNER models.
3. Run each notebook either in Kaggle (preferred) or Google Colab.

### Questions:

1. **Named Entity Annotation:**
   - Manually annotated 25 sentences with NER tags in BIO format using classes PER, LOC, ORG, MISC, and O.

2. **Fine-tuning NER Models:**
   - Fine-tuned IndicBERT and IndicNER models on the Naamapadam corpus for Hindi.
   - Performed training using a 70-10-20 train-validation-test split.

3. **ChatGPT NER:**
   - Passed the 25 manually annotated sentences to ChatGPT and recorded the results.

4. **Model Comparison:**
   - Evaluated the models and recorded macro-F1 scores within the respective notebooks.

5. **Report Submission:**
   - Submitted a detailed report in the `report.pdf` file included in the zip folder.

## Assignment 3

### Overview:
The third assignment involved evaluating three machine translation models: NLLB-200, IndicTrans, and ChatGPT, on a set of sentences in Hindi, English, and Gujarati.

### Libraries Used:
- `numpy`
- `random`
- `nltk`
- `rouge`
- `torch`
- `transformers`

### Steps to Run Assignment:

1. Extract the `231110033_assignment3.zip` in your local system.
   - This folder contains the benchmarks folder, assignment3 PDF file, 3 `.ipynb` files (one for each model), one `README.md` file, and one `Report.pdf` file.
2. The `.ipynb` files correspond to different models:
   - NLLB-200 with 600M
   - IndicTrans
   - ChatGPT
3. Run the first two models on Kaggle and the ChatGPT model on Google Colab.
   - Follow the sequence in the notebooks and ensure all required datasets and files are loaded correctly.

### Questions:

1. **Machine Translation Evaluation:**
   - Evaluated the following translations using the models:
     - English to Hindi
     - Hindi to English
     - Gujarati to Hindi
     - Hindi to Gujarati

2. **Analysis and Reporting:**
   - Detailed analysis and results are provided in the `Report.pdf` and respective notebooks.

3. **Additional Experiments:**
   - Conducted additional experiments and evaluations as described in the notebooks and report.
