# End-to-End Movie Recommendation System on AWS 
 
## Production-Grade AWS Pipeline 
**A complete, cloud-native movie recommendation system implementing real-world data engineering and machine learning practices on AWS.** 
 
## Project Structure 
\`\`\` 
movie-recommendation-system_aws/ 
ÃÄÄ notebooks/ 
³   ÀÄÄ movie_recommendation.ipynb 
ÃÄÄ data/ 
³   ÃÄÄ raw/ 
³   ³   ÃÄÄ movies.csv 
³   ³   ÀÄÄ ratings.csv 
³   ÃÄÄ processed/ 
³   ÀÄÄ models/ 
ÃÄÄ src/ 
ÃÄÄ config/ 
ÃÄÄ requirements.txt 
ÃÄÄ .gitignore 
ÀÄÄ README.md 
\`\`\` 
 
## End-to-End Architecture 
\`\`\` 
1. MovieLens Dataset - S3 Raw Zone 
2. AWS S3 - Glue Crawler 
3. Glue Crawler - Data Catalog 
4. Data Catalog - Glue ETL Job 
5. Glue ETL - S3 Processed Zone 
6. S3 Processed - Notebook 
7. Jupyter - Filtering Model (SVD) 
8. Model - to AWS S3 
\`\`\` 
 
## What You Built (Real Production Pipeline) 
 
- Created \`movie-reco-raw-nishu\` S3 bucket 
- Uploaded \`movies.csv\` and \`ratings.csv\` to Raw zone 
- **Why this matters**: Real data lake architecture 
 
### 2. Metadata Management (AWS Glue Crawler) 
- Automated schema discovery from S3 
- Created \`movie_reco_raw_db\` in Glue Data Catalog 
- Generated tables: \`movies_csv\`, \`ratings_csv\` 
- **Why this matters**: Turns files into queryable datasets 
 
### 3. Data Processing (AWS Glue ETL - Spark) 
- Built Spark ETL job for transformation 
- Performed aggregations: average_rating, rating_count 
- Output to \`movie-reco-processed-nishu/final/\` 
- **Why this matters**: Production ETL pipeline 
 
- Connected Jupyter to S3 using IAM 
- Feature engineering and EDA 
- **Why this matters**: Bridge engineering and science 
 
### 5. Machine Learning (Collaborative Filtering) 
- Implemented SVD algorithm 
- Generated predicted ratings 
- Produced personalized recommendations 
- **Why this matters**: Real ML, not basic sorting 
 
### 6. Production Output 
- Saved recommendations as \`movie_recommendations.csv\` 
- Stored in S3 processed zone 
- **Why this matters**: Ready for production use 
 
## Tech Stack 
 
## Pipeline Flow 
1. Raw Data - bucket 
2. Glue Crawler - Catalog 
3. Glue ETL - processing 
4. S3 Processed -
5. Jupyter - analysis 
6. Model - to S3 
 
## Getting Started 
\`\`\`bash 
git clone https://github.com/SanBigDataProjects/movie-recommendation-system_aws.git 
cd movie-recommendation-system_aws 
pip install -r requirements.txt 
jupyter notebook notebooks/movie_recommendation.ipynb 
\`\`\` 
 
## AWS Configuration 
1. Create IAM user with S3, Glue permissions 
2. Configure AWS CLI 
3. Create S3 buckets 
4. Set up Glue Crawler and ETL jobs 
 
## Skills Demonstrated 
- Data Engineering: S3, Glue, Spark ETL 
- Cloud Architecture: AWS serverless design 
- Data Science: Feature engineering, SVD 
- MLOps: End-to-end pipeline 
- Production Thinking: IAM, scalability 
 
## Results 
- Processed 25M+ ratings 
- Serverless, auto-scaling pipeline 
- Collaborative filtering with SVD 
- Personalized recommendations 
 
## Real-World Applicability 
This mirrors what companies like Netflix and Amazon use for recommendations, implemented on AWS. 
 
## License 
MIT License 
