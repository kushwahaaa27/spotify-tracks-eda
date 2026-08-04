# Spotify Tracks EDA 🎵

This project explores a dataset of **114,000 Spotify tracks** across **114 genres** and **31,000+ artists**. Using Exploratory Data Analysis (EDA), I analyzed various audio features to understand how tracks differ across genres and what factors are related to their popularity.

## Dataset

The dataset contains information about Spotify tracks, including:

- **Identifiers** — Track ID, Artist(s), Album Name, Track Name
- **Popularity** — Spotify popularity score (0–100)
- **Audio Features** — Danceability, Energy, Key, Loudness, Mode, Speechiness, Acousticness, Instrumentalness, Liveness, Valence, Tempo, and Time Signature
- **Other Metadata** — Duration, Explicit Flag, and Genre

> **Note:** Each genre contains exactly **1,000 tracks**, making this a balanced dataset created for analysis rather than a true representation of Spotify's complete music catalog.

## Tools Used

- Python
- Jupyter Notebook
- Pandas
- Matplotlib
- Seaborn

## What I Did

Some of the analyses performed in this notebook include:

- Understanding the dataset (shape, data types, summary statistics)
- Handling missing values
- Checking for and removing duplicate rows (450 duplicates found and removed)
- Popularity score distribution
- Track count by genre
- Explicit vs Non-explicit track distribution
- Distribution of core audio features such as Danceability, Energy, Speechiness, Acousticness, Instrumentalness, Liveness, Valence, and Tempo
- Correlation analysis between numerical features
- Top genres by average popularity
- Scatter plot analysis (Energy vs Loudness, Acousticness vs Energy, Valence vs Popularity)
- Top 10 most popular tracks
- Top 10 artists by number of tracks
- Popularity comparison between Explicit and Non-explicit tracks
- Song duration analysis
- Musical key and mode (Major/Minor) analysis by mapping encoded values to actual note names
- Top genres by Danceability

## Some Interesting Findings

Some interesting insights from the analysis:

- **Pritam** is the most represented artist in the dataset, highlighting the strong presence of Bollywood music.
- **The Beatles** and **George Jones** have some of the highest track counts among Western artists.
- **G Major** is the most frequently occurring musical key.
- Songs in **Major mode** appear more often than songs in Minor mode.
- Explicit tracks are slightly more popular on average than Non-explicit tracks.
- **Energy** and **Loudness** are strongly positively correlated.
- **Acousticness** and **Energy** show a strong negative correlation.
- **Valence** has little relationship with popularity.
- Most tracks have a duration between **2 and 4 minutes**, with an average length of approximately **3.87 minutes**.
- **Latin** and **Dancehall** are among the most danceable genres in the dataset.

## Project Structure

```text
spotify-tracks-eda/
│
├── data/
│   └── spotify-tracks-dataset-detailed.csv
│
├── notebooks/
│   └── spotify-eda.ipynb
│
├── .gitignore
└── README.md
```

## How to Run

Clone the repository:

```bash
git clone https://github.com/kushwahaaa27/spotify-tracks-eda.git
```

Open the notebook and run all the cells.

## Why I Made This Project

After working with a dataset that mainly contained categorical features in my Netflix EDA project, I wanted to challenge myself with a more feature-rich dataset containing many numerical variables.

This project helped me practice correlation analysis, explore relationships between different audio features, and work with encoded values such as musical keys and modes. It is another step in building my Machine Learning portfolio as I continue learning.

## What I Learned

Working on this project helped me:

- Improve my Exploratory Data Analysis (EDA) skills.
- Better understand relationships between numerical features using correlation analysis.
- Gain more confidence creating meaningful visualizations with Matplotlib and Seaborn.
- Practice working with large real-world datasets containing both categorical and numerical data.
- Improve my ability to communicate insights through data.

## Feedback

If you have any suggestions or notice something that could be improved, feel free to open an issue or share your feedback.
