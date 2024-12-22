# Customer Sentiment Analysis for iPhone 15 128GB Model

## Project Overview

The goal of this project is to analyze customer sentiment toward the **iPhone 15 128GB** model based on user reviews.
The analysis will focus on extracting valuable insights from customer feedback, identifying the overall sentiment (positive or negative),
and providing actionable recommendations for improving the product and customer experience.

## Objectives

- **Collect** at least 300 customer reviews for the iPhone 15 128GB model from Flipkart's product page.
- **Clean and preprocess** the data to ensure high-quality information for analysis.
- **Perform sentiment analysis** on the reviews using TextBlob.
- **Analyze** the sentiment distribution, review patterns, and extract key insights.
- **Provide recommendations** for product improvement or marketing strategies based on customer sentiment.

## Tools and Libraries

- **Selenium**: For automating the web scraping process and interacting with the Flipkart website.
- **BeautifulSoup**: For parsing HTML and extracting relevant details from the reviews.
- **Pandas**: For data cleaning, processing, and analysis.
- **TextBlob**: For performing sentiment analysis on the review text.
- **Matplotlib/Seaborn**: For creating visualizations, such as sentiment distributions and word clouds.

## Project Steps

### 1. Data Collection (Web Scraping)

**Tools**: Selenium, BeautifulSoup

- **Task**: Scrape at least 300 customer reviews for the iPhone 15 128GB model.
- **Details Collected**:
  - **Username**: The name of the reviewer.
  - **Rating**: The rating provided by the user (1 to 5 stars).
  - **Review Text**: The content of the customer review.
  
**Steps**:
- Automate browser interactions using Selenium to navigate to Flipkart’s product page for the iPhone 15 128GB.
- Use BeautifulSoup to parse the HTML and extract reviews from multiple pages, handling pagination where necessary.

### 2. Data Cleaning and Preprocessing

**Tools**: Pandas

- **Task**: Clean and preprocess the scraped data.
- **Steps**:
  - **Remove Duplicates**: Eliminate any duplicate reviews to ensure data quality.
  - **Handle Missing Values**: Address missing or incomplete data.
  - **Text Preprocessing**:
    - Convert review text to lowercase.
    - Remove irrelevant characters (special characters, punctuation, extra spaces).
    - Tokenize the text into individual words.
    - Remove stop words (common words that do not add sentiment value).
    - Perform lemmatization to convert words to their base form (e.g., "running" → "run").

### 3. Sentiment Analysis

**Tools**: TextBlob

- **Task**: Perform sentiment analysis on each review.
- **Steps**:
  - Use TextBlob to analyze the sentiment of the review text.
  - TextBlob provides a **polarity score** between -1 (negative) and +1 (positive), and a **subjectivity score**.
  - Define sentiment classification:
    - **Positive**: Polarity score ≥ 0.1
    - **Negative**: Polarity score < 0.1
  - Store sentiment classification in the dataset.

### 4. Data Analysis and Insights

**Tools**: Pandas, Matplotlib/Seaborn

- **Task**: Perform analysis on the sentiment data and visualize the findings.
  
**Steps**:
- **Sentiment Distribution**: Calculate the distribution of positive and negative sentiments.
- **Average Rating vs Sentiment**: Analyze the correlation between numeric ratings and sentiment polarity.
- **Word Cloud**: Create a word cloud to visualize the most frequent terms in positive and negative reviews.
- **Review Length Analysis**: Investigate the relationship between review length and sentiment.

### 5. Reporting

- **Overview**: Summarize the data collection and cleaning processes.
- **Sentiment Analysis Results**: Present the sentiment distribution, average sentiment per rating, and other key findings.
- **Insights**: Identify trends such as common issues with the product or highlights from positive reviews.
- **Recommendations**: Provide recommendations for product improvements or marketing strategies based on customer sentiment.

## Setup Instructions

1. Clone the repository:
   ```bash
   git clone https://github.com/AnchalDayal/Customer-Sentiment-Analysis---Web-Scraping.git
