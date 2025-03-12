# Restaurant Reviews Sentiment Analysis

![Python](https://img.shields.io/badge/Python-3.x-blue.svg)
![NLTK](https://img.shields.io/badge/NLTK-Sentiment-green.svg)
![Transformers](https://img.shields.io/badge/Transformers-BART-orange.svg)

A data science project that analyzes Google Maps restaurant reviews using Natural Language Processing techniques to evaluate sentiment and generate summaries.

## Overview

This project uses Python to analyze restaurant reviews from Google Maps, calculating sentiment scores and creating summaries to identify the best and worst-reviewed restaurants. The analysis combines traditional sentiment analysis (VADER) with modern transformer-based summarization (BART).

## Features

- **Data Loading and Preprocessing**: Imports and filters Google Maps restaurant review data
- **Rating Visualization**: Creates visual charts of restaurant ratings
- **Sentiment Analysis**: Uses NLTK's VADER (Valence Aware Dictionary and sEntiment Reasoner) to analyze review sentiment
- **Review Summarization**: Employs BART (Bidirectional and Auto-Regressive Transformers) to generate concise summaries of reviews
- **Comparison**: Identifies and compares the best and worst-reviewed restaurants

## Requirements

- pandas
- numpy
- matplotlib
- seaborn
- nltk
- transformers
- torch

## Installation

```bash
# Clone the repository
git clone https://github.com/yourusername/restaurant-sentiment-analysis.git
cd restaurant-sentiment-analysis

# Install required packages
pip install pandas numpy matplotlib seaborn nltk transformers torch
```

## Usage

1. Upload your Kaggle API credentials (`kaggle.json`) or modify the data loading section to use your own review data
2. Run the notebook cells sequentially to:
   - Load and preprocess the restaurant review data
   - Generate visualizations of ratings
   - Perform sentiment analysis with VADER
   - Create summaries using BART
   - Compare the best and worst-reviewed restaurants

## Data Source

This project uses the [Google Maps Restaurant Reviews](https://www.kaggle.com/datasets/denizbilginn/google-maps-restaurant-reviews) dataset from Kaggle.

## Project Structure

```
restaurant-sentiment-analysis/
│
├── SentimentAnalysis.ipynb    # Main notebook containing all analysis code
├── README.md                  # Project documentation
└── requirements.txt           # List of dependencies
```

## Methodology

1. **Data Collection**: Restaurant reviews are loaded from a Kaggle dataset
2. **Exploratory Analysis**: Visualization of restaurant ratings using seaborn and matplotlib
3. **Sentiment Analysis**: Each review is analyzed using VADER to calculate polarity scores (positive, negative, neutral, compound)
4. **Aggregation**: Sentiment scores are averaged by restaurant
5. **Summarization**: BART transformer model summarizes collections of reviews for key restaurants

## Results

The analysis identifies:
- The highest-rated restaurants based on both star ratings and sentiment scores
- The lowest-rated restaurants that might need improvement
- Key themes and feedback points from customer reviews through automatic summarization

## Future Enhancements

- Add topic modeling to identify specific aspects of restaurants mentioned in reviews
- Implement word clouds to visualize frequently used terms
- Create an interactive dashboard for exploring the data
- Expand analysis to more restaurants or different types of businesses

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Acknowledgments

- The [NLTK team](https://www.nltk.org/) for the VADER sentiment analysis tool
- [Hugging Face](https://huggingface.co/) for the transformers library and BART model
- [Kaggle](https://www.kaggle.com/) and the dataset creator for providing the restaurant reviews data
