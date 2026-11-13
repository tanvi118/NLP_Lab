# Computational Linguistics and Natural Language Processing Experiments

This repository contains practical NLP experiments for the **Computational Linguistics and Natural Language Processing** course. The experiments introduce text processing, corpus analysis, linguistic annotation, information extraction, and statistical language modeling.

## Course Objectives

- Understand Natural Language Processing and Natural Language Understanding.
- Process and analyze real-world text data.
- Apply tokenization, preprocessing, tagging, parsing, and named entity recognition.
- Build statistical language models and understand smoothing.
- Develop practical programming skills using common NLP tools and corpora.

## Experiments

| Experiment | Topic | Main Concepts | Dataset/Corpus |
|---|---|---|---|
| 2 | Text Retrieval and Text Processing | Tweet retrieval, sentence tokenization, word tokenization, cleaning, frequency analysis | Kaggle Twitter/X tweets dataset |
| 3 | Processing Data and Morphological Analysis | HTML removal, lowercasing, stop-word removal, stemming, lemmatization, prefixes and suffixes | IMDb Dataset of 50K Movie Reviews |
| 4 | Text Mining and Named Entity Recognition | Word counts, frequent words, bar charts, word clouds, corpus access, NER | Sample text and NLTK Brown Corpus |
| 5 | POS Tagging, Chunking and Parsing | Twitter tokenization, POS tagging, chunking, shallow parsing, dependency parsing | Kaggle Twitter/X tweets dataset |
| 6 | N-Gram Language Model and Smoothing | Unigrams, bigrams, trigrams, MLE, Laplace smoothing, sentence probability, perplexity | English News Sentence Corpus |

## Technologies Used

- Python 3
- Jupyter Notebook or Google Colab
- NLTK
- spaCy
- pandas
- NumPy
- Matplotlib
- WordCloud
- KaggleHub or manually downloaded Kaggle datasets

## Installation

```bash
pip install nltk spacy pandas numpy matplotlib wordcloud kagglehub
python -m spacy download en_core_web_sm
```

The notebooks may also download required NLTK resources such as tokenizers, stop words, POS taggers, corpora, and WordNet data. If required, run:

```python
import nltk

nltk.download('punkt')
nltk.download('punkt_tab')
nltk.download('stopwords')
nltk.download('wordnet')
nltk.download('omw-1.4')
nltk.download('averaged_perceptron_tagger')
nltk.download('averaged_perceptron_tagger_eng')
nltk.download('brown')
```

## Dataset Requirements

### Twitter/X Dataset

Experiments 2 and 5 use a Kaggle Twitter/X dataset. Download the CSV file and upload it when prompted, or place it in the notebook's working directory. The notebooks automatically identify the tweet/text column where possible.

### IMDb Dataset

Experiment 3 uses `IMDB Dataset.csv`, containing:

- `review`: movie-review text
- `sentiment`: positive or negative label

### English News Sentence Corpus

Experiment 6 uses `all_news_sentences.txt`. The corpus is used to build unigram, bigram, and trigram models.

## How to Run

1. Clone or download this repository.
2. Install the required dependencies.
3. Open the required notebook in Jupyter or Google Colab.
4. Download or upload the dataset requested by the notebook.
5. Run the cells from top to bottom.
6. Review the generated tables, plots, word clouds, parsed trees, and language-model results.

## Learning Outcomes

After completing these experiments, students should be able to:

- Retrieve and tokenize text data.
- Clean raw social-media and review text.
- Apply stemming and lemmatization.
- Analyze word frequency and text corpora.
- Perform POS tagging, chunking, and dependency parsing.
- Extract named entities using spaCy.
- Construct N-gram language models.
- Explain the zero-frequency problem and apply Laplace smoothing.
- Calculate sentence probability and perplexity.

## Repository Structure

```text
.
├── Experiment_2_Text_Retrieval_Twitter_Tokenization.ipynb
├── Experiment_3_Processing_Data_IMDb.ipynb
├── Experiment_4_Text_Mining_and_NER.ipynb
├── Experiment_5_POS_Tagging_Chunking_Twitter.ipynb
├── Experiment_6_NGram_Language_Model_Smoothing.ipynb
└── README.md
```

## Notes

- Dataset filenames and column names may differ depending on the Kaggle download.
- Exact POS-tagging output can vary with the installed NLTK model version.
- Perplexity values should be compared only when the evaluation data and preprocessing are the same.
- Kaggle downloads may require authentication or manual dataset upload.

## License

This repository is intended for educational use. Dataset licenses and terms of use belong to their respective dataset providers.
