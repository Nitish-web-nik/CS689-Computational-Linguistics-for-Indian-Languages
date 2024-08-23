# CS689A - Computational Linguistics for Indian Languages 🚀

### Name: Nitish Kumar  
### Roll No: 231110033  
### Dept.: M.Tech (C.S.E)

Welcome to the world where code meets language, and not just any language—this is about decoding the magic of Indian languages. This repository contains the code and reports for three assignments that took us on a rollercoaster ride through Unicode correction, tokenization, Named Entity Recognition (NER), and even machine translation with some of the latest and greatest models. Buckle up, because it’s been a wild ride!

---

## Assignment 1 - The Unicode Detective 🕵️‍♀️

### Overview:
Our first mission was all about diving deep into the intricacies of Hindi text. We corrected Unicode errors, tokenized text like pros, and ran frequency analyses on everything from tokens to syllables. Imagine sifting through a treasure trove of data with a magnifying glass—this was it.

### Libraries Used:
- `numpy` (because who doesn't love arrays?)
- `matplotlib.pyplot` (for the graphs that make data look pretty)
- `pandas` (your data's best friend)
- `re` (because regular expressions are the secret sauce)
- `transformers` (bringing AI magic to the table)
- `sentencepiece` (for those who love breaking text into pieces)
- `sklearn` (because we’re all about that machine learning life)

### Steps to Run Assignment:

1. **Unzip the Mystery:**
   Extract the `assignment1.zip` in your local system. Think of it as opening a mystery box—what surprises await inside?

2. **Open the Treasure Map:**
   Open the `231110033.ipynb` file in your favorite environment—Jupyter Notebook, Google Colab, or Visual Studio Code. Make sure to update the data path in the second cell according to your file location. (No one likes a missing file, trust us!)

3. **Follow the Clues:**
   Run the notebook cell by cell, following the questions specified below. It's like solving a puzzle—each piece brings you closer to the big picture.

### Questions:

1. **Unicode Correction:**
   - We built a function that’s like a language spell-checker, correcting Unicode errors in a Hindi corpus. Imagine fixing typos, but in code! Example: The corrected form of the word `त् आ र् ई ख् अ` is `तारीख`. Nailed it!

2. **Tokenization and Frequency Analysis:**
   - Tokenized the text and extracted syllables using our custom methods. Then, we played detective, finding the top-20 frequent uni-gram and bi-gram frequencies of tokens, syllables, and characters. Think of it as finding the most popular words in a secret language.

3. **Word Group Formation:**
   - Grouped words based on semantic units like inflections, verb auxiliaries, and compounds using a tool that felt like sorting your sock drawer—except more fun.

4. **Tokenization Techniques:**
   - Evaluated different tokenizers like Unigram, BPE, mBERT, IndicBERT, and White-space. It was like a tech bake-off—each tokenizer brought something different to the table.

5. **Evaluation of Tokenizers:**
   - Compared the performance of different tokenizers by calculating precision, recall, and F-score for 25 sentences. Because in the world of NLP, stats don’t lie!

6. **Model Comparison:**
   - Summarized the performance of the models. Spoiler: Some did better than others, but that’s part of the fun!

---

## Assignment 2 - The NER Adventure 🌍

### Overview:
Next, we dove into the world of Named Entity Recognition (NER) in Hindi. We manually annotated data (yes, by hand!) and then let IndicBERT and IndicNER models do their thing. The journey was long, but the results? Totally worth it.

### Libraries Used:
- `numpy` (still love arrays)
- `pandas` (because tables are life)
- `transformers` (can’t live without it now)
- `sklearn` (stats for the win)
- `accelerate` (because speed matters)
- `datasets` (to feed the models)
- `seqeval` (for evaluating sequences like a pro)

### Steps to Run Assignment:

1. **Unzip the Adventure:**
   Extract the `assignment2.zip` in your local system. It’s like unwrapping a gift, but instead of socks, you get data files!

2. **Two Roads to Travel:**
   The zip file contains two `.ipynb` files—one for IndicBERT and one for IndicNER. Run each notebook either in Kaggle (our top pick) or Google Colab. It’s like choosing your weapon—both will get the job done.

### Questions:

1. **Named Entity Annotation:**
   - We manually annotated 25 sentences with NER tags in BIO format. It was tedious, but someone had to do it! We used classes like PER (Person), LOC (Location), ORG (Organization), MISC (Miscellaneous), and O (Other). 

2. **Fine-tuning NER Models:**
   - Fine-tuned IndicBERT and IndicNER models on the Naamapadam corpus for Hindi. It’s like training your dog, but instead of “sit” and “stay,” you’re teaching the model to recognize names and places.

3. **ChatGPT NER:**
   - We couldn’t resist seeing how ChatGPT handled NER, so we threw our 25 sentences at it and recorded the results. The verdict? ChatGPT’s good, but even it has its off days.

4. **Model Comparison:**
   - Evaluated the models and recorded macro-F1 scores in the notebooks. Spoiler: We had a winner, but you’ll have to check the notebooks to find out which one!

5. **Report Submission:**
   - Submitted a detailed report in the `report.pdf` file included in the zip. Because what’s an adventure without a story to tell?

---

## Assignment 3 - The Translation Tango 💃

### Overview:
Our final mission took us into the world of machine translation. We evaluated three models—NLLB-200, IndicTrans, and ChatGPT—on translating between Hindi, English, and Gujarati. It was like playing telephone with AI, and the results were fascinating!

### Libraries Used:
- `numpy` (still going strong)
- `random` (because randomness is fun)
- `nltk` (text processing for the win)
- `rouge` (for scoring translations like a judge at a dance-off)
- `torch` (because deep learning is deep)
- `transformers` (our trusty sidekick)

### Steps to Run Assignment:

1. **Unzip the Final Challenge:**
   Extract the `assignment3.zip` in your local system. This folder contains the benchmarks folder, the assignment3 PDF file, 3 `.ipynb` files (one for each model), a `README.md` file, and a `Report.pdf` file.

2. **Three Models, Three Paths:**
   The `.ipynb` files correspond to different models:
   - NLLB-200 with 600M (big brains)
   - IndicTrans (made in India)
   - ChatGPT (the one, the only)

3. **Run with Style:**
   - Run the first two models on Kaggle (for when you need the heavy lifting) and the ChatGPT model on Google Colab (because it’s always online). Follow the sequence in the notebooks and make sure all datasets and files are loaded correctly—no one likes a missing data error!

### Questions:

1. **Machine Translation Evaluation:**
   - Evaluated translations between:
     - English to Hindi
     - Hindi to English
     - Gujarati to Hindi
     - Hindi to Gujarati
   - The results? Let’s just say, some translations were like poetry, others... not so much.

2. **Analysis and Reporting:**
   - Detailed analysis and results are provided in the `Report.pdf` and respective notebooks. If you’re into translation battles, this one’s for you!

3. **Additional Experiments:**
   - We couldn’t stop ourselves from running a few extra experiments. You’ll find them detailed in the notebooks and report—because why settle for just the basics?

---

## Final Thoughts 🧠

And that’s a wrap on our journey through Computational Linguistics for Indian Languages. From fixing Unicode errors to training models that understand Hindi, it’s been a whirlwind of code, caffeine, and late-night debugging. If you’re reading this, we hope our work helps you on your own linguistic adventure. And remember, when in doubt—just hit run and see what happens!

Happy coding! 🎉
