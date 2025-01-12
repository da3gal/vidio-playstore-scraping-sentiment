# vidio-playstore-scraping-sentiment
Scraping user reviews for the Vidio app from the Google Playstore (186,433 rows), applying TF-IDF and Word2Vec for feature extraction. Four models (Naive Bayes, SVM, Random Forest, XGBoost, RNN) are used for 3-class sentiment classification (Positive, Neutral, Negative), with hyperparameter tuning, word cloud visualization, and model testing. <br>

The tool used for scraping data is [google-play-scraper](https://github.com/facundoolano/google-play-scraper) by Facundo Olano. The stemming library used for Indonesian words is **Sastrawi**. The slangwords data for text normalization is [Slangwords Dictionary by Rama Prakoso](https://raw.githubusercontent.com/ramaprakoso/analisis-sentimen/refs/heads/master/kamus/kbba.txt). For sentiment labeling, both the [positive lexicon](https://raw.githubusercontent.com/angelmetanosaa/dataset/main/lexicon_positive.csv) and [negative lexicon](https://raw.githubusercontent.com/angelmetanosaa/dataset/main/lexicon_negative.csv) are provided by Angel Metanosa. <br>

To run this project, you will need to install:

```bash
pip install google-play-scraper
pip install Sastrawi
