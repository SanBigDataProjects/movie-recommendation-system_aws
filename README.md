# Movie Recommendation System with AWS

## Project Overview
End-to-end movie recommendation system using AWS S3, Glue, and Spark with collaborative filtering algorithms.

## Project Structure
- **data/**
  - raw/
    - movies.csv
    - ratings.csv
  - processed/
- **notebooks/**
  - movie_recommendation.ipynb
- LICENSE
- requirements.txt
- .gitignore
- README.md

## What You Built
1. **AWS S3 Data Lake** - Raw and processed data storage
2. **AWS Glue ETL** - Data processing pipeline
3. **Collaborative Filtering** - SVD algorithm for recommendations
4. **Production Pipeline** - End-to-end AWS workflow

## Tech Stack
- **AWS**: S3, Glue, IAM
- **Python**: Pandas, Scikit-surprise
- **ML**: Collaborative Filtering (SVD)

## Getting Started
```bash
git clone https://github.com/SanBigDataProjects/movie-recommendation-system_aws.git
cd movie-recommendation-system_aws
pip install -r requirements.txt
jupyter notebook notebooks/movie_recommendation.ipynb
