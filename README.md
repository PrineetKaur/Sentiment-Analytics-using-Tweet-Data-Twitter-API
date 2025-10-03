# Sentiment Analytics using Tweet Data (Twitter API)

## (Project from my Big Data Analytics Master's 2022 batch)

## Table of Contents
1. [Project Overview](#Project-Overview)
2. [Features](#Features)
3. [Technologies Used](#Technologies-Used)
4. [Project Structure](#Project-Structure)
5. [Getting Started](#Getting-Started)
6. [Documentation](#Documentation)
7. [Project Usage](#Project-Usage)
8. [Project Conclusion](#Project-Conclusion)
9. [License](#License)
10. [Acknowledgments](#Acknowledgments)


## Project Overview
Customer opinions expressed on social media can have a significant impact on a brand's reputation.
This project collects real-time tweets about Delta Airlines to gauge customer sentiment (positive, negative, neutral). Utilizing R, Shiny, and Markdown, it fetches real-time data via the Twitter API, performs sentiment analysis, and presents the findings through interactive dashboards.

## Features
- Fetch tweets in real-time via **Twitter API**
- Perform **sentiment classification** on text data
- Generate **distribution graphs** of sentiment
- Display **trends over time**
- Visualize frequent terms using a **word cloud**
- Interactive **Shiny dashboard** for exploration

## Technologies Used
- **R**: Programming language for statistical computing.
- **Shiny**: Web application framework for R.
- **rtweet**: R package for accessing Twitter's REST and stream APIs.
- **tidyverse**: Collection of R packages for data science.
- **ggplot2**: Data visualization package for R.

## Project Structure

	Sentiment-Analytics-using-Tweet-Data-Twitter-API/
	│
	├── SMA Project - Group 4_Code.ipynb   		# Core notebook with R/Shiny code
	├── docs/
	│   ├── how_to_guide.md                		# Step-by-step Setup Guide
	│   ├── api_reference.md               		# Functions and API documentation
	├── LICENSE.md                        		# MIT License
	└── README.md                         		# Project Overview

## Getting Started 

### Prerequisites
	•	R (v4.0+)
	•	RStudio (recommended)
	•	Twitter Developer Account for API keys

### Installation
1. Clone the repository:
  	```bash
  	git clone https://github.com/PrineetKaur/Sentiment-Analytics-using-Tweet-Data-Twitter-API.git
   	cd Sentiment-Analytics-using-Tweet-Data-Twitter-API

2.	Install necessary R packages: 
   	```R
  	install.packages(c("shiny", "rtweet", "tidyverse", "ggplot2"))

### Run the Shiny App
	
	shiny::runApp("SMA Project - Group 4_Code.ipynb")

### Obtain Twitter API credentials
Create a Twitter Developer account and set up an application to get the *API_KEY, API_SECRET, ACCESS_TOKEN, and ACCESS_SECRET*.

## Documentation
- [How to Guide](Docs/how-to-guide.md) – Setup & usage instructions
- [API Reference](Docs/api-reference.md) – Functions and parameters

## Project Usage
	•	Upon launching the Shiny app, input relevant keywords or hashtags related to Delta Airlines.
	•	The dashboard will display real-time sentiment analysis, including:
	•	Sentiment distribution (positive, negative, neutral)
	•	Time-series sentiment trends
	•	Word clouds of frequently used terms

## Project Conclusion
The tweets data helped to summarize the overall user tweet trend for Delta Airlines, which included:

- ***Follower Profile Summary*** - (Provides a world map to see the overall distribution of the Tweets users across the globe and their top locations
  
 - ***User Trend*** *(user-specific data like the most liked post, most popular hashtags among users, most shared links, etc)*

- ***Tweeter Status Frequency*** *(helped understand the most likable days of the month when users post about Delta Airlines, and in return, the tendency of Delta Airlines to post replies to the user tweets)*

- ***User Profile*** – *(Included top users making maximum tweets about Delta Airlines, their most preferred platforms, and the top languages they spoke)*

- ***Sentiment Analysis*** – *(Concluded based on the Emotions scores of the Tweets along with their engagement & response activity w.r.t those sentiments (positive/negative))*

- ***Detailed Topic Analysis using Bigrams***

## Screenshots
Some screenshots for reference from the final [Analysis Markdown Report](https://rpubs.com/delta_twitter/721486)

##### World Map showing Global Distribution of Users Tweeting about Delta Airlines
<img align="left" alt="world map" width="100px" src="https://i.ibb.co/jP7gcCZM/Screenshot-2025-10-03-at-11-28-23.png" />

##### Topic Analysis of Tweets from Top 6 Competitors
<img align="left" alt="Competition" width="100px" src="https://i.ibb.co/Mx702Mmb/Screenshot-2025-10-03-at-11-27-01.png" />


<br />
<br />
<br />
<br />


## License

This project is licensed under the MIT License - see the *LICENSE.md* file for details.

## Acknowledgments
	•	rtweet for Twitter API integration.
	•	Shiny for interactive web applications.
	•	tidyverse for data manipulation and visualization.

