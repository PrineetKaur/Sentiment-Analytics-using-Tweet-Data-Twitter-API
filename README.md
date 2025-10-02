# Sentiment Analytics using Tweet Data (Twitter API)

## (Project from my Big Data Analytics Master's 2022 batch)

## Table of Contents
1. [Project Overview](#Project_Overview)
2. [Features](#features)
3. [Technologies Used](#technologies_used)
4. [Project Structure](#Project_Structure)
5. [Getting Started](#Getting-Started)
6. [Documentation](#documentation)
7. [Project Usage](#project-usage)
8. [License](#license)
9. [Acknowledgments](#acknowledgments)

## 📌 Project Overview
Customer opinions expressed on social media can have a significant impact on a brand's reputation.
This project collects real-time tweets about Delta Airlines to gauge customer sentiment (positive, negative, neutral). Utilizing R, Shiny, and Markdown, it fetches real-time data via the Twitter API, performs sentiment analysis, and presents the findings through interactive dashboards.

## ✨ Features
- Fetch tweets in real-time via **Twitter API**
- Perform **sentiment classification** on text data
- Generate **distribution graphs** of sentiment
- Display **trends over time**
- Visualize frequent terms using a **word cloud**
- Interactive **Shiny dashboard** for exploration

## 🖥️ Technologies Used
- **R**: Programming language for statistical computing.
- **Shiny**: Web application framework for R.
- **rtweet**: R package for accessing Twitter's REST and stream APIs.
- **tidyverse**: Collection of R packages for data science.
- **ggplot2**: Data visualization package for R.

## 📂 Project Structure
Sentiment-Analytics-using-Tweet-Data-Twitter-API/
│
├── SMA Project - Group 4_Code.ipynb   		# Core notebook with R/Shiny code
├── docs/
│   ├── how_to_guide.md                		# Step-by-step Setup Guide
│   ├── api_reference.md               		# Functions and API documentation
├── LICENSE.md                        		# MIT License
└── README.md                         		# Project Overview

## 🚀 Getting Started 

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
	```R
	shiny::runApp("SMA Project - Group 4_Code.ipynb")

### Obtain Twitter API credentials
Create a Twitter Developer account and set up an application to get the *API_KEY, API_SECRET, ACCESS_TOKEN, and ACCESS_SECRET*.

## 📖 Documentation
- [How-to Guide](documentaion/how-to-guide.md) – Setup & usage instructions
- [API Reference](documentation/APIreference.md) – Functions and parameters

## 🔄 Project Usage
	•	Upon launching the Shiny app, input relevant keywords or hashtags related to Delta Airlines.
	•	The dashboard will display real-time sentiment analysis, including:
	•	Sentiment distribution (positive, negative, neutral)
	•	Time-series sentiment trends
	•	Word clouds of frequently used terms

## 🖼 Screenshots

(Work in Progress :))

## 📜 License

This project is licensed under the MIT License - see the *LICENSE.md* file for details.

## 🙌 Acknowledgments
	•	rtweet for Twitter API integration.
	•	Shiny for interactive web applications.
	•	tidyverse for data manipulation and visualization.
