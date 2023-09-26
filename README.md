# Unsupervised Machine Learning
## Goal
To evaluate whether Machine Learning can be used to automatise playlist creation.

## Overview 
Moosic is a small startup that creates playlists curated manually by music experts. Their listeners love the personal touch, which they achieve by capturing the "mood" or "vibe".  

  _Board_: Believes that they need at least a **degree of automatisation**, as music experts are not able to keep up with the demand. **Currently** the whole creation process is **done manually**.
  
  _Music Experts_: Are **skeptical** that audio features on their own are not enough to capture the "mood" which is very subjective that **only a human can judge**.

## Context
Moosic wants the data science team to use a dataset that has been collected from the Spotify API and contains the audio features (tempo, energy, danceability…) for a few thousand songs.  After useing a basic **clustering algorithm** such as K-Means to divide the dataset into a few clusters the data team shall answer the following two questions: 

1. *Are Spotify’s audio features able to identify “similar songs”, as defined by humanly detectable criteria?*
2. *Is K-Means a good method to create playlists?* 

### Task: 
* Import list of 5000 songs collected from Spotify API
* Use basic clustering ex.: K-Means to divide dataset into clusters
* Validate clusters, export clusters (playlists) to Spotify and listen to some of the songs

#### Challenges:
* Difficult to evaluate the results without listening to each playlist
* No tangible way to measure accuracy
* Unevenly large clusters
* Subjective - what is a good playlist?

#### Solutions:
* Must be visualized, so we can see the overlaps and the outliers
* Limit the number of features to 3 (or multiples of 3) so it can be visualized in 3D scatterplot
* Find a balance between K-score and the business objectives
* Instead of replacing music experts, ML does the "heavy lifting" and they fine-tune the results

## Approach
1. Evaluate the database; basic cleaning, ex.: missing, corrupted values, correct data types
2. Exploration of audio features
3. Decide which features to drop, and which features to use
4. K-Means clustering
5. Evaluation of clusters
6. Sub-clustering
7. Evaluation of final clusters

## Deliverables
5 minute **PowerPoint presentation** found [here](https://drive.google.com/file/d/1vUTZUToQtD97X_53d7Ht7nSnJrvjJ5G_/view?usp=sharing) to the Board of Directors, that summarizes the findings and suggests a course of action.
**Python code** is found [here](4_0_5000_songs_FINAL_NOTEBOOK.ipynb).

## Skills & Tools
1. Data Cleaning & Quality Assurance
2. Data Preprocessing: Scaling
3. K-Means Clustering
4. Elbow Method and Silhouette Score
5. Data Visualization (3D Scatterplot)
