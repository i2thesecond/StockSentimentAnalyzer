# StockSentimentAnalyzer
The Stock Sentiment Analyzer performs Natural Language Processing(NLP) on Twitter data and correlates the current mood sentiment of public posts on the Twitter platform to stock market trends.

The application is based on research from J. Bollen and H. Mao's paper "Twitter mood as a stock market predictor" from the IEEE Compiuter Journal 44(10):91-94, in addition to related research.

Users indicate key words to capture public posts; such as stock tickers ($MSFT) and other related keyterms (such as "Microsoft"). Twitter's streaming API is used to store public posts that contain the indicated keyterms. The tweets are periodically processed through NLP algorithms that derive the columative emotional sentiment amongst captured posts. Live stock prices are captured using the Yahoo Finance API. Sentiment is correlated with stock market prices to predict stock market trends (Bullish, Bearish, or Nuetral). Users can view the market prediction by stock ticker.

Tweepy library to connect to Twitter's Streaming API

Yahoo Finance API to connect to Yahoo's stock price data.
 
NLTK library performs NLP processing on Twitter data. 

Django Framework used as database storage. Provide web-based user interface. 

The application is to help the Omaha Amatuer Investing Group that meets at Hardy Coffee on Benson every Wednesday at 4:30 PM.

## Installation
```bash
docker-build .
docker-compose run django bash
python manage.py migrate
python manage.py createsuperuser
```

## Getting Started
To run my awesome app simply,
```bash
docker-compose up
```
See in-app menus for help with using specific features.


## Research
J. Bollen and H. Mao "Twitter mood as a stock market predictor"
Venkata Pagolu, Kamal Challa, Ganapati Panda "Sentiment Anaylysis of Twitter Data for Predicgting Stock Market Movements"
Anshul Mittal, Arpit Goel "Stock Prediction Using Twitter Sentiment Analysis"

# License
The MIT License (MIT)

Copyright (c) Gavin R. Crowl

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in
all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
THE SOFTWARE.
