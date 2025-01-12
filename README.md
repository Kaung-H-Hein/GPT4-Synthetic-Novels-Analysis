# GPT4-Synthetic-Novels-Analysis
This repository presents a comprehensive project that applies natural language processing (NLP) techniques to a dataset of 700 synthetic short stories generated by OpenAI’s GPT-4 model. Each story is annotated with metadata, which includes information that can be used to train and evaluate models. The project, part of my MSc in AI studies, is divided into three sections:

**Section 1: Text Processing and Linguistic Insights**
- 1.1 Zipf’s Law
- 1.2 Writing Style and Dependency Parsing

**Section 2: Text Classification**
- 2.1 Text Classification with Word2Vec
- 2.2 Text Classification with BERT

**Section 3: Sentiment and Emotion**
- 3.1 Sentiment Analysis with BERT
- 3.2 Emotional Content of Stories

## Section 1: Text Processing and Linguistic Insights

This section investigates key aspects of the linguistic properties of synthetic text generated by OpenAI's GPT-4 model, focusing on Zipf’s law and writing style. 
The following tasks were performed for analysis:

### 1.1 Zipf’s Law
Zipf’s law is an empirical observation stating that in a given corpus, the frequency of a word is inversely proportional to its rank in the frequency table. 
This law holds true for most natural languages, where the most common word occurs roughly twice as often as the second most common word, three times as often as the third most common, and so on.

**Aim**:  
The objective is to determine if Zipf’s law holds for synthetic text generated by GPT-4. The text is treated as a single corpus, and the analysis checks whether Zipf’s law holds by calculating token frequencies, ranking the tokens, and visualising the results.

**Overview**:  
The steps followed in this analysis include:
1. **Data exploration and preparation**:
   - Collecting story data and concatenating the text contents into a single corpus.
   - Applying the `en_core_web_sm` English tokenizer, tagger, and parser from `spaCy`.
   - Using regular expressions to remove punctuation.
   - Processing the text with the `spaCy` NLP pipeline, extracting tokens.
2. **Analysis**:
   - Calculating token frequencies and rankings.
   - Visualising the frequency distribution.
   - Evaluating whether Zipf’s law holds for the synthetic text.

### 1.2 Writing Style and Dependency Parsing
The text for each story was generated in the style of one of five authors: Samuel Beckett, Stephen King, Lewis Carroll, Charles Dickens, and Enid Blyton. 
The author used for each story is provided in the “writer” metadata field.

**Aim**:  
The goal is to explore whether there are differences in the linguistic structure of stories generated by different authors. Specifically, the syntactic complexity of sentences is investigated by examining the longest dependency span in each sentence. This measure (`max_dep`) serves as an indicator of syntactic complexity, and `max_dep` is compared across the five authors.

**Overview**:  
The steps followed in this analysis include:
1. **Data exploration**:
   - Retrieving the writer metadata.
   - Selecting stories based on the author metadata.
2. **Analysis**:
   - Calculating the longest dependency span for each sentence.
   - Calculating the average and maximum dependency spans for each story.
   - Visualising the results, using raincloud plots to compare the syntactic complexity across authors.

### Key Libraries and Tools Used:
- **spaCy** for tokenization and dependency parsing.
- **Matplotlib** for data visualisation.
- **ptitprince** for raincloud plots.
- **NumPy** and **collections.Counter** for data manipulation.

--

## Section 2: Text Classification

### 2.1 Text Classification with Word2Vec

### 2.2 Text Classification with BERT

### Key Libraries and Tools Used:

## Section 3: Sentiment and Emotion

### 3.1 Sentiment Analysis with BERT

### Emotional Content of Stories

### Key Libraries and Tools Used:
