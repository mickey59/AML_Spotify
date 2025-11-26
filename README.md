# AML_Spotify

Spotify Analysis
We are a skunkworks team within Spotify tasked with exploring ways by which the company can get better insight about the artists, albums, and user preferences for music. We’ve been given access to data from the “Top 200” playlists published globally by Spotify from 01/01/2017 to 31/05/2023 comprising of nearly 0.5M songs composed of different regional charts! This data has canonical information such as track titles, artist info, url, and so on.

# Cleaning the data:

In order to clean the data we have from Spotify we run the jupyter notebook 'repoClean.ipynb', we remove certain rank, date, and points columns from the data and we add a scaled loudness column. 
In the Archive Notebooks folder we have notebooks that clean the dataset and add new features such as song lyrics, language detected, featuring artists. These notebooks do not need to be run anymore.


# First Task- Genre Prediction:

In the 'genre_classification.ipynb', we normalise the data, split the dataset into training, validation and test sets. We then implement a Logistic Regression model, a Decision Tree Classifier, a Random Forest Classifer. Finally, we classify songs into seperate genre labels.
In the 'gpNN.ipynb' we also implement a Neural Network Model.


# Second Task- Song Recommendation:

In the 'song-prediction.ipynb' file we create semantic embeddings for the song lyric data, and we implement four models and compare their performances based on five metrics; ‘silhouette score’ to measure cluster quality, ‘mean pairwise distance’
to measure how diverse songs are in the dataset, and ‘embedding efficiency’ given by (silhouette/variance) to determine if the model is dominated by noise, and finally two coherence scores. 