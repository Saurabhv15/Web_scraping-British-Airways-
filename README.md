# Web_scraping-British-Airways-

# British Airways Reviews Sentiment Analysis

This project involves scraping customer reviews for British Airways from [Airline Quality](https://www.airlinequality.com/airline-reviews/british-airways), cleaning and processing the text data, performing sentiment analysis, and visualizing the results.

## Features

1. **Web Scraping**:
   - Uses the `requests` library to fetch data from multiple pages.
   - Scrapes review content using `BeautifulSoup`.

2. **Text Preprocessing**:
   - Removes special characters and noise from reviews.
   - Tokenizes, lemmatizes, and performs part-of-speech tagging for further analysis.

3. **Sentiment Analysis**:
   - Leverages VADER (Valence Aware Dictionary and sEntiment Reasoner) to classify reviews as Positive, Negative, or Neutral.

4. **Visualization**:
   - Generates a pie chart to represent sentiment distribution.
   - Creates a WordCloud to visualize frequently occurring words in the reviews.

5. **Export**:
   - Final processed dataset is exported to a CSV file (`BA_reviews.csv`).

---

## Prerequisites

Ensure you have the following installed in your Python environment:

- Python 3.x
- Libraries:
  - `requests`
  - `BeautifulSoup4`
  - `pandas`
  - `nltk`
  - `matplotlib`
  - `vaderSentiment`
  - `wordcloud`

You can install the required libraries using:

```bash
pip install requests beautifulsoup4 pandas nltk matplotlib vaderSentiment wordcloud
```

---

## How to Run

1. Clone this repository or download the script.
2. Run the script using Python:
   ```bash
   python script_name.py
   ```
3. The script will:
   - Scrape reviews from 10 pages of the British Airways review section on Airline Quality.
   - Perform text preprocessing and sentiment analysis.
   - Save the processed data to a CSV file named `BA_reviews.csv`.
   - Generate and display a pie chart for sentiment analysis and a WordCloud.

---

## Outputs

1. **CSV File**:
   - A file named `BA_reviews.csv` containing:
     - Original reviews.
     - Cleaned reviews.
     - Part-of-Speech tagged tokens.
     - Lemmatized text.
     - Sentiment scores.
     - Sentiment classification (Positive, Neutral, or Negative).

2. **Visualizations**:
   - Pie chart showing the proportion of Positive, Neutral, and Negative reviews.
   - WordCloud highlighting frequently occurring words.

---

## Folder Structure

```
.
├── script_name.py     # Python script for scraping and analysis
├── BA_reviews.csv     # Output file containing processed data
└── README.md          # Documentation file
```

---

## Sample Visualizations

### Sentiment Distribution

- A pie chart displays the percentage of Positive, Neutral, and Negative reviews.

### WordCloud

- A WordCloud highlights common words in the reviews, providing insights into frequent topics.

---

## Notes

- Ensure the website structure has not changed before running the script. If any errors occur during scraping, verify the HTML structure of the webpage.
- Sentiment analysis may not always be 100% accurate, as it depends on the quality of the VADER lexicon.

---
