# Spotify Data Analysis: Insights into My Listening Habits

## Introduction
This project delves into my personal Spotify listening habits by analyzing data from playlists and songs I listened to. Through this project, I aim to gain insights into my favorite artists, songs, and listening patterns over time. This analysis combines data visualization and exploration to uncover meaningful trends in my music preferences. Beyond analyzing patterns and trends, this project aims to include a predictive model to determine why a track is opened (e.g., via forward button, track done, or play button) based on contextual, user behavior, and song-related features.

## Motivation
I wanted to explore my Spotify data to better understand my music taste, identify listening patterns, find trends across playlists and time. Also, I think predicting track-opening behaviour provides nice insights into my listening habits by understanding my track selection. Also it is very cool. Analyzing personal data like this provides a fun and informative way to combine music and data science.


## Data Source
- The data for this project comes from Spotify's personal data export feature and my manually curated playlists.
- Includes:
  - Song listening history (timestamps, song names, artists...).
  - Playlists with song details.
- **Note**: The raw data is not included in this repository for privacy reasons.

## Key Features
- Analysis of top artists and songs by listening hours and play counts.
- Time-based patterns in music consumption (hourly, daily, monthly).
- Unique vs. non-unique songs in playlists.
- Visual representation of insights using:
  - Bar charts for top artists and songs.
  - Pie charts for unique vs. non-unique songs.
  - Word clouds for favorite songs and artists.
  
**Predictive Model**: A machine learning model to predict why a track was opened based on contextual, behavioral, and song-related features.

## Machine Learning Approach
- **Goal**: Predict the reason for track opening (`reason_start`) based on:
  - Song attributes (e.g., duration, artist?(I hate Beiber)).
  - Contextual features (e.g., time of day, artist?).
  - User behavior (e.g., skip history, session activity).
- **Model**: Implementing a Random Forest classifier (or other more suitable models).
- **Evaluation**: Assess using accuracy, precision, recall, and confusion matrix.
- **Features**:
  - Song-level: `duration`, etc.
  - User-level: `skip_percentage`, etc.
  - Context-level: `time_of_day`, `device_type`.


## **Techniques Used**
- Exploratory Data Analysis (EDA): To clean and understand the data.
- Visualization: Using Python libraries like Matplotlib and Seaborn to create graphs.
- Time Series Analysis: To explore trends over hours, days, and months.

  **Below are examples of the insights gained through visualizations:**
  - Top Artists and Songs: By listening hours and play counts.
  - Unique vs. Non-Unique Songs: Pie chart representation.
  - Day-wise and Hourly Streaming Patterns: Time-based analysis.
  - Word Clouds: Highlighting favorite songs and artists.



##  **Results**
**Key findings from the analysis include:**

- My top 10 favorite artists based on listening time and play counts.
- Streaming is most active on Sundays and during late afternoon/evening hours.
- I listen to unique songs about 16.6% of the time, while the remaining 83.4% includes repeated songs(How original!).
- March stands out as the month with the highest streaming activity.
















