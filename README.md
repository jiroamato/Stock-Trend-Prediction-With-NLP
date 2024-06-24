# **Stock Trend Prediction with NLP**
How much does news affect the trend of stock prices and why is it important?

With better tools to assess market sentiment, both individual and institutional investors are equipped to make swift and strategic investment decisions and potentially resulting in higher returns. A key important benefit is wealth preservation, firms that manage retirement funds for example can position themselves from capital loss using sentiment data.


## **Overview**
In this project, the goal is to garner insights on the relationship between sentiment in the financial markets and its impact in stock price movements. I will attempt to do so with Machine Learninng first incorporating NLP. In this preliminary version. I will be doing some EDA on a data set for use in training sentiment analysis on financial news.

The importance of sentiment analysis shows itself in the following:
- Informed decision making:
  - Sentiment analysis adds another dimension of information for investor to act on in order to make better market moves.
- Risk management:
  - Gauging sentiment allows investors to potentially identify risk factors in the market early enough to protect their portfolios.
 
To give you a perspective of how the market is, the Canadian Pension Plan's assets under management is around $590.8 billion. With better market intel, we can reduce the risk of our nesteggs.

Here is a flowchart of the proposed model:<br>
![image](/docs/figures/flowchart.jpg)


## **Table Of Contents**
1. Data Cleaning
2. Exploratory Data Analysis (EDA)
3. Data Pre-processing
4. Vectorization
5. Next Steps     


## **Data**
The initial training dataset has **4,840 rows** and **2 columns**

### Data Dictionary

**Column Name:**   

- `Headline:` The headline of the news article
- `Sentiment:` Classifications by positive, neutral or negative. These classifications were agreed upon by 16 professionals in the Finance domain.

**Other datasets of the project (will investigate further):**

The second dataset of the project contains daily news gather from 2009-2020 which has the following:

### Data Dictionary (2nd Dataset)
Contains **843,062** unique articles.

**Column Name:**   

- `headline:` The headline of the news article
- `url:` Link to the article
- `publisher:` Name of the publisher
- `date:` Date the article was released
- `stock:` The stock that the article refers to

Lastly, the third dataset contains the daily historical price of the S&P 500 index from 2000-2024 which has the following:

### Data Dictionary (3rd Dataset)

**Column Name:**   
Contains **6,038** observations.

- `Date:` Date of when the price was recorded
- `Open:` Price level during the market opening
- `High:` Highest that price went to during trading hours
- `Low:` Lowest that price went to during trading hours
- `Adj Close:` The closing price (adjusted to include any corporate decision made before the next trading day)
- `Volume:` The total amount that the index was traded expressed in $


## **Model**
As far as vectorization models of text-data, **Bag of Words** is used as an initial benchmark in this first-pass. **TF-IDF** was also explored in this dataset. There will be two models that will be required to model sentiment analysis and stock trends.

**Sentiment Analysis Modelling**:
- Base Models:
	- Logistic Regression
	- Decision Tree
	- K-Nearest Neighbor
	- Naïve Bayes

**Time Series Modelling**:
- Base Models:
	- AR
	- ARIMA

## **Developer**
Jiro Amato

## **License**
This project is licensed under the [License](https://opensource.org/license/mit)