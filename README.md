# Spotify Data Analysis: Exploring My Listening Habits

## Motivation

I started this project to explore my Spotify listening habits and gain a deeper understanding of my music preferences. By analyzing the data, I hope to uncover patterns in my listening behavior, such as favorite artists, songs, and trends over time. Additionally, I hope to take it a step further by building a predictive model to determine why a track is opened (e.g., via forward button, track done, or play button).Why? Because it is cool! Just kidding, this predictive aspect combines my love for music and technology with the exciting challenge of data science. Through this project, I hope to gain valuable insights while expanding my technical skillset.

---

## Data Source

The data for this project was sourced from Spotify's personal data export feature and my manually curated playlists. The dataset includes:

- **Song listening history**: Timestamps, song names, artists, and more.
- **Playlists**: Information about songs within each playlist.
- **Includes data between 2019 and 2024.**
  
**Note**: The raw data will not be included in the repository to protect privacy.

---

## Data Analysis

This project will follow several stages of analysis:

### 1. Data Cleaning
- Handling missing values, standardizing column names, and ensuring consistency across datasets.

### 2. Exploratory Data Analysis (EDA)
- I will be using Python libraries like Pandas, Matplotlib, and Seaborn to visualize and analyze the data.
- To gain insights into:
  - Top artists and songs by listening hours and play counts.
  - Patterns in music consumption across days, hours, and months.
  - Proportion of unique vs. non-unique songs in playlists.

### 3. Visualization
- **Bar charts**: Top artists and songs.
- **Pie charts**: Unique vs. non-unique songs.
- **Word clouds**: Favorite artists and songs.
- **Time-based trends**: Hourly, daily, and monthly streaming patterns.

### 4. Predictive Modeling
- **Goal**: Building a model in Jupyter Notebook(Easier said then done) to predict the reason a track is opened (`reason_start`) based on contextual, user behavior, and song-related features.
- **Approach**:
  - Implementing machine learning models like Random Forest directly in the notebook(Or other models, if I find more suitable ones).
  - Using scikit-learn for model training and evaluation.
- **Evaluation**:
  - Assessing the model using accuracy, precision, recall, and a confusion matrix.
- **Features**:
  - Song-level: `duration`, `artist`, etc.
  - User-level: `skip_percentage`, historical listening behavior.
  - Context-level: `time_of_day`, `device_type`, `artist`.

---

## Findings

Through this project, I hope to learn the following about my listening habits:

- **Top Artists and Songs**:
  - Identify my top artists and songs by listening time and play counts.
  - Understand how my preferences vary by genre or mood.
- **Streaming Patterns**:
  - Explore which days and times I’m most active.
  - Highlight specific months or seasons when I stream more frequently.
- **Repetition**:
  - Calculate how often I revisit songs and playlists(Answer is a lot).
- **Prediction**:
  - Use the predictive model to identify key factors driving track-opening behavior.

---

## Limitations and Future Work

### Limitations (Expected):
1. **Data Diversity**:
   - The dataset will reflect only my personal listening habits, limiting generalizability.
2. **Class Imbalance**:
   - Some `reason_start` categories (e.g., "trackdone") might dominate, which could affect prediction accuracy for less frequent reasons.
3. **Feature Limitations**:
   - External factors like mood, activity type, or social influences are not included in the dataset(Apple did not send me my data :/).

### Future Work:
1. **Advanced Modeling**:
   - Experiment with deep learning models or ensemble techniques (if allowed) in Jupyter Notebook.
2. **Broader Analysis**:
   - Compare my listening habits with global Spotify trends or data from other users.
3. **Additional Predictions**:
   - Extend the project to predict skip likelihood, playlist preferences, or favorite genres.

---

## How to Run

To explore or replicate the analysis and prediction model:

1. Clone this repository to your local machine.
2. Open the Jupyter Notebook file (`Spotify_Data_Analysis.ipynb`) in your Jupyter environment.
3. Ensure you have Python and the following libraries installed:
   - Pandas
   - Matplotlib
   - Seaborn
   - Scikit-learn
4. Run the notebook cells step by step to:
   - Analyze and visualize the data.
   - Train and evaluate the predictive model.

---

## Acknowledgments

- **Spotify**: For providing the data export feature.
- **Python Libraries**: Matplotlib, Seaborn, Pandas, and Scikit-learn for enabling analysis and modeling.
