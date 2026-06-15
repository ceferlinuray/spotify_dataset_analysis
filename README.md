# spotify_dataset_analysis
This project analyzes a Spotify tracks dataset to uncover patterns in song popularity, genre characteristics, artist performance, and audio features.
The analysis combines exploratory data analysis (EDA), business-oriented insights, and machine learning techniques to understand what makes songs successful on Spotify.

Dataset

The dataset contains Spotify tracks along with:

Track information (name, artist, album)
Popularity score (0–100)
Genre classification
Audio features such as:
  Danceability
  Energy
  Speechiness
  Acousticness
  Instrumentalness
  Liveness
  Valence
  Tempo
  Duration


Data Preparation
Missing Values
Checked for missing values.
Removed rows containing null values.
Duplicate Tracks

Many tracks appeared multiple times because a single song could belong to multiple genres.

To support different analytical goals, two datasets were created:

Song-Level Dataset (df_song)
  One record per unique track.
  Duplicates removed using track_id.
  Used for popularity, artist, audio feature, and machine learning analyses.
  
Genre-Level Dataset (df_genre)
Original dataset retained.
Used for genre-specific analyses.

Exploratory Data Analysis
Popularity Anaysis
What are the top 10 most popular songs?
What are the top 10 most popular artists?
Which artists are consistently popular rather than relying on a single viral hit?

Genre Analysis
Which genres contain the most tracks?
Which genres are the most popular?
Which genres are the least popular?
Which genres have the highest danceability?
Which genres have the highest energy?


Audio Feature Analysis
Average danceability, energy, and valence
Correlation between audio features and popularity
Genre-level audio feature profiles
Which songs have excellent audio characteristics but low popularity?
Do collaborations perform better?
Are collaborations more likely to become hit songs?


Duration Analysis
Average song length
Genres with the longest songs
Genres with the shortest songs

Song Analysis
What are the characteristics of top 10% songs?
What emotional profile listeners prefer

Machine Learning
Predicting Song Popularity
A supervised machine learning approach was used to estimate song popularity from audio features.


Technologies Used
Python
Pandas
NumPy
Matplotlib
Seaborn
Scikit-learn


