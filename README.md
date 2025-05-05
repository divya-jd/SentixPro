# SentixPro

Sentiment analysis plays an essential role in understanding user opinions, emotions, and perceptions embedded within textual data. While sentence-level sentiment analysis provides an overall judgment about whether a sentence or review is positive or negative, it often fails to capture the fine-grained opinions related to specific product or service aspects. On the other hand, aspect-based sentimentanalysis (ABSA) focuses on extracting and evaluating sentiments toward particular components or attributes mentioned in the text, offering a more detailed and actionable understanding.

The core problem addressed in this project is to systematically compare the performance and
capabilities of two prominent sentiment analysis approaches:

(1) Sentence-level sentiment analysis using both LSTM with GloVe embeddings and the
transformer-based DistilBERT model, and
(2) Unsupervised aspect-based sentiment analysis using graph-based extraction techniques paired
with a pre-trained DistilBERT sentiment classifier.

This comparison seeks to uncover the strengths, weaknesses, and practical applicability of each
method across different evaluation scenarios, including general sentiment classification and
fine-grained aspect-level evaluation. By addressing these questions, the project aims to provide
insights that can guide the selection and application of sentiment analysis techniques in diverse use cases.

##Dataset

a. Source
The datasets used for training and testing the models come from public review datasets available on platforms such as Amazon Polarity. These datasets include both positive and negative reviews from a range of product categories, which were used for training both DistilBERT and LSTM + GloVe
models for sentiment analysis.

b. Size
The datasets used for the experiments consist of:
●Sentence based: 10000 samples of training and 1000 testing
●Unsupervised Aspect-Based Dataset: 5,000 test samples for aspect-based sentiment
analysis.

c. Preprocessing Steps
The following preprocessing steps were performed to prepare the text data for the models:
1. Text Lower-casing:All text was converted to lowercase to standardize the input and minimize
variations.
2. Special Character Removal:Non-alphanumeric characters (such as punctuation and special
symbols) were removed to ensure that only relevant words remain for analysis.
3. Tokenization:The text was split into individual words, a process known as tokenization, which
is essential for transforming text into a format suitable for machine learning models.
4. Stopword Removal:Common words (e.g.,"the","is,"and") that don't contribute significantly
to sentiment analysis were removed.
5. Lemmatization:Lemmatization was applied to reduce words to their root form. For example,
words like "running" were converted to "run",making the text more uniform.
6. Text Reconstruction:After processing, the individual words were rejoined into a single string
to prepare the text for input into the sentiment analysis models.

For more information and files related to the project, you can connect with me on LinkedIn: https://www.linkedin.com/in/velankani-joise-divya/