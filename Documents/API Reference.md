# API Reference: Sentiment Analytics using R and Shiny

This document provides detailed descriptions of the main functions and scripts used in this project.

---

### 1. `get_tweets()`

**Description:**  
Fetches tweets using the Twitter API for a given keyword or hashtag.  

**Parameters:**  
- `search_query` *(string)*: Search term (e.g., `"Delta Airlines"`).  
- `n` *(integer)*: Number of tweets to fetch. Default = 100.  

**Returns:**  
Data frame containing:  
- Tweet text  
- Username  
- Timestamp  
- Retweet/favorite counts  

**Example Usage:**
    ```R
    tweets <- get_tweets("Delta Airlines", n = 500)

---

### 2. `analyze_sentiment()`

**Description:**
  Classifies text into sentiment categories.

**Parameters:**
	•	text (string): Input tweet text.

**Returns:**
  Sentiment label: "positive", "negative", or "neutral".

**Example Usage:**
    ```R
    sentiment <- analyze_sentiment("Delta service was amazing!")
    # Output: "positive"

---

### 3. `plot_sentiment_distribution()`

**Description:**
Creates a pie/bar chart showing the percentage of positive, negative, and neutral tweets.

**Parameters:**
	•	sentiment_data (data frame): Data frame with sentiment labels.

**Returns:**
A ggplot object for visualization.

**Example Usage:**
    ```R
    plot_sentiment_distribution(sentiment_data)

---

### 4. `plot_sentiment_trends()`

**Description:**
  Plots sentiment frequency over time.

**Parameters:**
	•	sentiment_data (data frame): Data frame with timestamps and sentiment labels.

**Returns:**
  A ggplot line chart of sentiment trends.

**Example Usage:**
    ```R
    plot_sentiment_trends(sentiment_data)

---

### 5. `create_wordcloud()`

**Description:**
Generates a word cloud of frequently used terms in the dataset.

**Parameters:**
	•	text_data (vector of strings): Cleaned tweet text.

**Returns:**
A word cloud visualization.

**Example Usage:**
    ```R
    create_wordcloud(tweets$text)

---    

### Notes
	•	All functions assume that authentication via rtweet::create_token() has been completed.
	•	Functions can be reused with any keyword/hashtag, not just airline data.

