# How-to Guide: For Performing Sentiment Analysis on Tweets Using R and Shiny

This guide walks you through the process of setting up, running, and exploring the sentiment analysis application that analyzes tweets about Delta Airlines (or any other topic).

---

## 1. Introduction
Sentiment analysis is a natural language processing technique that determines whether text expresses a positive, negative, or neutral sentiment.  
This project collects tweets in real-time via the Twitter API, processes them in R, and presents results through an interactive **Shiny dashboard**.

---

## 2. Prerequisites
- **R** (v4.0 or higher) installed on your system.  
- **RStudio** (recommended for running and debugging).  
- A **Twitter Developer Account** to obtain API keys.  
- Internet connection.

---

## 3. Installation

### Step 1: Clone the Repository
    ```bash
    git clone https://github.com/PrineetKaur/Sentiment-Analytics-using-Tweet-Data-Twitter-API.git
    cd Sentiment-Analytics-using-Tweet-Data-Twitter-API

### Step 2: Install Required R Packages
    Open R or RStudio and run:
    ```R
    install.packages(c("shiny", "rtweet", "tidyverse", "ggplot2", "lubridate"))

---

## 4. Setting up Twitter API Credentials
	1.	Go to Twitter Developer Portal.
	2.	Create a new app and generate the following credentials:
	•	API_KEY
	•	API_SECRET
	•	ACCESS_TOKEN
	•	ACCESS_SECRET
	3.	In R, authenticate using:
    ```R
    library(rtweet)
    token <- create_token(
    app = "your_app_name",
    consumer_key = "API_KEY",
    consumer_secret = "API_SECRET",
    access_token = "ACCESS_TOKEN",
    access_secret = "ACCESS_SECRET"
    )

---

## 5. Running the Application
	1.	Launch the app from RStudio:
  ```R
  shiny::runApp("SMA Project - Group 4_Code.ipynb")

	2.	Open the Shiny dashboard in your browser.
	3.	Enter a search term (e.g., “Delta Airlines”) and wait for tweets to load.


---

## 6. Exploring the Dashboard
	•	Sentiment Distribution: Pie chart showing percentages of positive, negative, and neutral tweets.
	•	Trends Over Time: Line chart displaying sentiment changes by day/hour.
	•	Word Cloud: Visual representation of frequent terms in tweets.

⸻

## 7. Troubleshooting
	•	No tweets retrieved?
	•	Ensure API credentials are correct and have sufficient access.
	•	Error loading Shiny app?
	•	Check if the required R packages are installed.
	•	Graphs not rendering?
	•	Verify dataset is not empty (try broader search terms).

⸻

## 8. Conclusion

By following this guide, you can fetch tweets in real-time, analyze sentiment, and visualize insights interactively. This project demonstrates how social media analytics can help businesses understand customer perception.

