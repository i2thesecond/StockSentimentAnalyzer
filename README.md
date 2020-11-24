# StockSentimentAnalyzer
The Stock Sentiment Analyzer predicts stock market trends (Bearish, Bullish, or Neutral) by performing emotional sentiment analysis on public Twitter data and correlating the data with stock market prices.

### How It Works
The application captures public tweets containing stock tickers (such as "$MSFT"). Under each stock ticker, the user can include related key terms (such as "Microsoft" or "Redmond") that will also be captured. A periodical process performs sentiment analysis using Natural Language Processing(NLP) techniques to derive the stock ticker's cumulative emotional sentiment. The emotional sentiment is correlated with stock market prices to predict stock market trends (Bullish, Bearish, or Neutral). Users can view the application's market prediction by stock ticker.

### Project Objective
The project's objective is to explore OSSINT-based stock prediction analysis's potential and provide a useful tool for the Omaha Amateur Investing group. 

Research from J. Bollen and H. Mao's paper "Twitter mood as a stock market predictor" from the IEEE Computer Journal 44(10):91-94, in addition to subsequent research on the subject, inspires the project.

### Dependencies
The project makes use of multiple open-source libraries. These libraries are as follows:

* Tweepy library is used to connect to Twitter's Streaming API. 
* yfinance is used to connect to Yahoo Finance API to gather stock prices. 
* NLTK library is used to perform NLP processing on collected tweets to derive sentiment. 
* Django Framework provides the web framework used for the application UI and database storage through Django's object-relational mapper (ORM).

The application uses docker and docker-compose to deploy.

## Installation
```bash
docker-build .
docker-compose run django bash
python manage.py migrate
python manage.py createsuperuser
```

## Getting Started
To run Stock Sentiment Analyzer simply,
```bash
docker-compose up
```

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
