I built this project to see how Taylor Swift’s lyrics evolve emotionally across her career using NLP. The dataset comes from Kaggle(https://www.kaggle.com/datasets/ishikajohari/taylor-swift-all-lyrics-30-albums), which includes her albums, songs, and metadata in a clean, structured format.

For sentiment analysis, I didn’t want to rely on just one method. TextBlob gives a quick sense of polarity and subjectivity, but it can miss the nuance of short, emotional lines. VADER is great for that since it’s tuned for social media-style text (a good fit for lyrics). On top of that, I added machine learning models (Logistic Regression, Naive Bayes) with TF-IDF features to capture patterns beyond dictionary-based scores.

Before analysis, the lyrics go through NLTK preprocessing—things like tokenization, stopword removal, and lemmatization—to clean up the text and strip out non-lyrical markers. That way, the results actually reflect meaning instead of noise.

The tool generates album comparisons, sentiment timelines, and distribution plots, plus it exports the results which you can checkout in the sentiment_results.csv file. In short, it’s both a fan project and a data science exercise—meant to explore Taylor’s artistic evolution while also showing how different sentiment methods stack up.
