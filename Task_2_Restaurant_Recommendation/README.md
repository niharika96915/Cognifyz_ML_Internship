# Task 2: Restaurant Recommendation System

## Overview
This project implements a content-based restaurant recommendation system using the Cognifyz restaurant dataset. It recommends restaurants based on cuisine preferences, price range, and aggregate rating.

## Dataset
- **Records:** 9,551 restaurants
- **Original features:** 21 columns
- **Selected features:** Restaurant Name, Cuisines, Price range, Aggregate rating, City, Has Online delivery, and Has Table booking
- **Preprocessing:** Missing cuisine values were handled, and relevant columns were selected and cleaned.

## Technologies Used
- Python
- Pandas
- Scikit-learn
- TF-IDF Vectorization
- Cosine Similarity
- Google Colab

## Methodology
1. Loaded and explored the restaurant dataset.
2. Selected relevant restaurant attributes.
3. Handled missing values and prepared the data.
4. Converted cuisine descriptions into numerical features using TF-IDF.
5. Calculated cuisine similarity using cosine similarity.
6. Filtered recommendations according to preferred cuisine, maximum price range, and minimum rating.
7. Tested the system with Italian, Indian, and Japanese cuisine preferences.

## Results
The system successfully generated restaurant recommendations for different cuisine preferences.

For the Japanese cuisine test with a maximum price range of 2 and a minimum rating of 4.5, three restaurants were recommended:
- Marukame Udon — Rating: 4.9
- Miyabi 9 — Rating: 4.8
- Kobe Hibachi & Sushi — Rating: 4.6

All three results satisfied the specified price and rating conditions.

## Output
The generated Japanese restaurant recommendations are saved in `outputs/japanese_restaurant_recommendations.csv`.

## Conclusion
This project demonstrates content-based restaurant recommendation using cuisine text similarity, combined with price and rating filters. It can be extended with location preferences, online delivery requirements, table booking preferences, and user feedback.

## Internship
**Organization:** Cognifyz Technologies  
**Project:** Machine Learning Internship — Task 2: Restaurant Recommendation System
