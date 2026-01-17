# Movie Recommendation System with AWS

## Project Overview
This project implements a **production-grade movie recommendation system** on AWS, demonstrating full-stack data engineering and machine learning skills. The pipeline processes **25M+ movie ratings** to deliver personalized recommendations using:

1. **AWS S3** as a data lake (raw/processed zones)
2. **AWS Glue** for serverless ETL and metadata management
3. **Apache Spark** for distributed data processing
4. **Collaborative Filtering** (SVD) for recommendation algorithms
5. **End-to-end automation** from data ingestion to model deployment

**Business Impact**: This architecture mirrors what companies like Netflix and Amazon use for personalized recommendations, scaled down to demonstrate core concepts while maintaining production-ready practices.

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
