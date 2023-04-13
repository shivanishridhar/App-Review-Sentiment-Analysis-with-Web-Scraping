# App Review Sentiment Analysis with Web Scraping

## Technologies : App review, sentiment analysis, web scraping, NLP, classification, Python, NLTK, scikit-learn, GitHub
In this project, we developed a Python-based system to perform sentiment analysis on 30K+ app reviews scraped from the Google Play Store and Apple App Store combined. The goal of the project was to analyze the sentiment of app reviews, categorizing them as positive or negative based on the text content, and provide insights into user feedback for app developers and marketers.

### Web Scraping 
Google App Scraper is a program or script that automates the process of extracting data from the Google Play Store, which is an online marketplace for Android applications (apps). This type of web scraping tool is designed specifically to collect information related to apps listed on the Google Play Store, such as app name, description, ratings, reviews, download statistics, pricing, and other relevant details
We started by utilizing web scraping techniques to extract app review data from the Google Play Store using Python libraries such as BeautifulSoup and Requests. The scraped data included review text, ratings, and other relevant information.

### Data Preprocessing 
Tokenization and Vectorization were critical steps in preparing the app review data for sentiment analysis.

Tokenization is the process of breaking down the text data into smaller units called tokens, which are typically words or phrases.We used NLTK's built-in functions to tokenize the review text data, which involved splitting the text into individual words or phrases, and removing unnecessary characters, such as punctuation and special characters. This allowed us to convert the unstructured review text into structured data that could be further processed and analyzed.

After tokenization, we performed vectorization using the bag-of-words representation. We used scikit-learn, a popular machine learning library in Python, to create a numerical representation of the tokenized text data. This involved counting the frequency of each word in the tokenized text and creating a sparse matrix representation of the data, where each row represented a review and each column represented a unique word in the dataset. This vectorized representation of the text data served as input for our machine learning algorithms.

We also experimented with word embeddings, which are dense vector representations that capture the semantic meaning of words. We used pre-trained word embedding models, such as Word2Vec or GloVe, to generate dense vector representations of the words in our app review data. These word embeddings were used as input features for our machine learning algorithms, allowing us to capture more nuanced relationships between words in the text data.

### NLP Classification
Afterwards, we applied machine learning techniques for sentiment analysis using scikit-learn. We trained a classification model on a labeled dataset of app reviews, using features extracted from the pre-processed review text, such as bag-of-words representation or word embeddings. We used Naive Bayes Classifier and finally mapped the positive and negative ratings.


