# Sentiment Analytics using Tweet Data (Twitter API)

## (Project from my Big Data Analytics Master's 2022 batch)

## Table of Contents
1. [Project Overview](#project-overview)
2. [Features](#features)
3. [Technologies Used](#technologies-used)
4. [Setup Instructions](#setup-instructions)
5. [Usage](#project-usage)
6. [How-to Guide](docs/how-to-guide.md)
7. [API Reference](docs/api-reference.md)
8. [License](#license)
9. [Acknowledgments](#acknowledgments)

## Project Overview
This project analyzes public tweets about Delta Airlines to gauge customer sentiment. Utilizing R, Shiny, and Markdown, it fetches real-time data via the Twitter API, performs sentiment analysis, and presents the findings through interactive dashboards.

## Features
- **Real-time Data Collection**: Fetches tweets using the Twitter API.
- **Sentiment Analysis**: Classifies tweets into positive, negative, or neutral sentiments.
- **Interactive Dashboards**: Visualizes sentiment trends and patterns using Shiny.

## Technologies Used
- **R**: Programming language for statistical computing.
- **Shiny**: Web application framework for R.
- **rtweet**: R package for accessing Twitter's REST and stream APIs.
- **tidyverse**: Collection of R packages for data science.
- **ggplot2**: Data visualization package for R.

## Setup Instructions
1. Clone the repository:
   ```bash
   git clone https://github.com/PrineetKaur/Sentiment-Analytics-using-Tweet-Data-Twitter-API.git
   cd Sentiment-Analytics-using-Tweet-Data-Twitter-API

2.	Install necessary R packages: 
    ```R
  	install.packages(c("shiny", "rtweet", "tidyverse", "ggplot2"))

3.	Obtain Twitter API credentials by creating a Twitter Developer account and setting up an application to get the *API_KEY, API_SECRET, ACCESS_TOKEN, and ACCESS_SECRET*.

## Project Usage
	•	Upon launching the Shiny app, input relevant keywords or hashtags related to Delta Airlines.
	•	The dashboard will display real-time sentiment analysis, including:
	•	Sentiment distribution (positive, negative, neutral)
	•	Time-series sentiment trends
	•	Word clouds of frequently used terms

## How-to Guide

Following are the basic steps to set up and run the sentiment analysis application. If you feel stuck somewhere and need a detailed "How-To", you can refer to the *How-to Guide.md* file.

### Step 1: Install R and RStudio
	•	Download and install R from https://cran.r-project.org/.
	•	Download and install RStudio from https://posit.co/download/rstudio-desktop/.

### Step 2: Install Required R Packages
Open RStudio and run the following command to install the necessary packages:
     ```R
    install.packages(c("shiny", "rtweet", "tidyverse", "ggplot2"))

### Step 3: Obtain Twitter API Credentials
	•	Visit Twitter Developer and create a new application.
	•	Note down the API_KEY, API_SECRET, ACCESS_TOKEN, and ACCESS_SECRET.

### Step 4: Run the Shiny Application

In RStudio, run the following command to start the application:
    ```R
    shiny::runApp("SMA Project - Group 4_Code.ipynb")

### Step 5: Interact with the Dashboard
	•	Enter keywords or hashtags related to Delta Airlines in the input field.
	•	Explore the visualizations to understand the sentiment trends.

## API Reference

### get_tweets()
	•	Description: Fetches recent tweets based on a search query.
	•	Parameters:
	•	search_query: Character string specifying the search term.
	•	n: Integer specifying the number of tweets to fetch.
	•	Returns: A data frame containing tweet text, user information, and metadata.

### analyze_sentiment()
	•	Description: Analyzes the sentiment of a given text.
	•	Parameters:
	•	text: Character string containing the text to analyze.
	•	Returns: A character string indicating the sentiment ("positive", "negative", "neutral").

### plot_sentiment_trends()
	•	Description: Plots the sentiment trends over time.
	•	Parameters:
	•	sentiment_data: Data frame containing sentiment data with timestamps.
	•	Returns: A ggplot object displaying the sentiment trends.

## License

This project is licensed under the MIT License - see the *LICENSE.md* file for details.

## Acknowledgments
	•	rtweet for Twitter API integration.
	•	Shiny for interactive web applications.
	•	tidyverse for data manipulation and visualization.
