# CinemaMatch: Personalized Movie Recommender with Sentiment Insights



## Overview
**CinemaMatch** is a recommendation engine that suggests movies similar to those you already enjoy while providing sentiment analysis insights based on user reviews. This tool goes beyond typical recommendations by analyzing real user sentiments for a deeper understanding of each film.

## Key Features
- **Customized Movie Suggestions**: CinemaMatch provides recommendations based on a user’s selected movie preferences, focusing on elements like genre, title, runtime, rating, poster, and more.
- **Sentiment Analysis of Reviews**: By accessing user reviews through IMDb and performing sentiment analysis, CinemaMatch offers nuanced feedback on how viewers feel about each movie.
- **Multi-Source Data Gathering**: Movie information is retrieved through the TMDB API, while review data is web-scraped from IMDb using BeautifulSoup to ensure a comprehensive data set.

## Setting Up the API Key
1. Visit [The Movie Database (TMDB)](https://www.themoviedb.org/) and create a new account.
2. Navigate to the API section within your account settings.
3. Complete the required details to request an API key.
4. Once approved, you’ll find the API key under the API section of your TMDB account settings.

## How to run the project?

1. Install all the libraries mentioned in the "requirements.txt" file.
2. Clone this repository in your local system.
3. Replace YOUR_API_KEY in the `main.py` file.
4. Open the command prompt from your project directory and run the command `python main.py`.
5. Go to your browser and type `http://127.0.0.1:5000/` in the address bar.
6. Hurray! That's it.


## Behind the Recommendation Logic
## Similarity Scoring 
The system uses a similarity scoring method to determine movies closest in character to the user’s preferred movie. By analyzing text features of each movie, CinemaMatch assigns a similarity score based on the cosine similarity between selected movie details.

## Cosine Similarity Explained
Cosine similarity is a metric that calculates the cosine of the angle between two vectors in a multi-dimensional space, representing the similarity between two text documents. It's beneficial here because even if two movies have different amounts of descriptive text, they may still share similar themes or concepts, leading to a high similarity score. A smaller angle implies higher similarity, which allows for more relevant recommendations.

  ![image](https://user-images.githubusercontent.com/36665975/70401457-a7530680-1a55-11ea-9158-97d4e8515ca4.png)

  
## Additional Features to Explore
1. Personalized Dashboards: Integrate a dashboard that tracks past recommended movies and user interactions for continuous improvement.
2. Genre-Specific Filtering: Allow users to select specific genres or exclude certain themes from their recommendations.
3. Sentiment Trend Analysis: Visualize sentiment trends over time, showing how public opinion about a movie has evolved.
