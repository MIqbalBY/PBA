---
title: "AI dan AR dalam Gamifikasi SIAR Halal apps: Katalisasi Pertumbuhan Sosial Ekonomi dalam Kerangka Digital Halal"
author: "irhafidz, nurainir, hadziq, Siska Arifiani"
date: "13/03/2025"
output: raw_data (moneyspent_cleaned.csv) cleaned_data (out.csv), sentiment_siarhalal.ipynb
---

## Repository Structure

```
📂 Sentiment-Analysis-SIARHalal-MSMEs
 ├── data/                # Raw and processed datasets
 │   ├── moneyspent_cleaned.csv      # Original dataset
 │   ├── out.csv    # Processed dataset with sentiment scores
 │
 ├── notebooks/           # Jupyter Notebooks for analysis
 │   ├── sentimentsiarhalal.ipynb  # Main notebook
 │
 ├── README.md            # Project introduction (this file)
 ├── LICENSE              # License information
```

## Introduction

This repository is part of the research project **"AI dan AR dalam Gamifikasi SIAR Halal apps: Katalisasi Pertumbuhan Sosial Ekonomi dalam Kerangka Digital Halal"**, which is a recipient of **RGBI 2024 (Research Grant Bank Indonesia)** under **TIM ID 2516 – TOPIK 1: Pemanfaatan AI untuk meningkatkan Inklusi Ekonomi & Keuangan Konvensional dan Syariah**.

### **Research Theme:**
- **Sub-tema 3:** Pemanfaatan AI untuk Mendorong Inklusi Ekonomi khususnya kepada pelaku ekonomi kecil dan menengah

This project focuses on **leveraging AI and AR technologies** to enhance the gamification experience in **SIAR Halal apps**, aiming to **boost digital halal economy growth** and improve economic inclusion, particularly for **small and medium enterprises (MSMEs)**.

Key features of this project include:
- **Preprocessing user reviews** (cleaning, stopword removal, tokenization)
- **Sentiment analysis using TextBlob** (polarity and subjectivity scoring)
- **Data aggregation and visualization** (analyzing sentiment trends per food stall)

The primary goal is to identify trends in **customer feedback**, highlight areas for business improvement, and understand **how sentiment correlates with ratings and customer visits**.

## Dataset

The dataset consists of user-generated reviews for multiple food stalls, including:
- `msme`: Name of the food stall
- `Number_of_Visits`: Total visits recorded
- `Number_of_Feedbacks`: Number of customer reviews
- `Average_Rating`: Average rating score
- `Average_Spend`: Average spending per customer
- `Sentiment`: Sentiment polarity score (-1 = Negative, 0 = Neutral, 1 = Positive)

## Methodology

The sentiment analysis pipeline follows these steps:
1. **Data Preprocessing:**
   - Tokenization
   - Stopword removal using `Sastrawi`
   - Normalization (removing special characters, lowercasing, stemming, lemmatization)
2. **Sentiment Analysis:**
   - `TextBlob` to compute **polarity** and **subjectivity** scores
   - Aggregation of sentiment scores per food stall
3. **Exploratory Data Analysis (EDA):**
   - Word cloud visualization
   - Sentiment distribution charts
   - Correlation analysis between sentiment, ratings, and visits
