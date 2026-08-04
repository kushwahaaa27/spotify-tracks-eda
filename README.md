Spotify Tracks EDA 🎵

This project explores a dataset of **114,000 Spotify tracks** across **114 genres** and **31,000+ artists**, analyzing audio features like danceability, energy, loudness, and valence to understand what shapes a track's popularity and how genres differ from one another.

Dataset
The dataset contains 20 columns per track, covering:

* **Identifiers** — track_id, artists, album_name, track_name
* **Popularity** — a 0–100 popularity score
* **Audio Features** — danceability, energy, key, loudness, mode, speechiness, acousticness, instrumentalness, liveness, valence, tempo, time_signature
* **Other Metadata** — duration_ms, explicit, track_genre

Each genre contains exactly 1,000 tracks, making this a balanced dataset rather than a real-world popularity distribution.

Tools Used

* Python
* Jupyter Notebook
* Pandas
* Matplotlib
* Seaborn

What I Did
Some of the things I explored in this notebook include:

* Understanding the dataset (shape, data types, summary statistics)
* Handling missing values
* Checking for and removing duplicate rows (450 duplicates found and dropped)
* Popularity score distribution
* Track count by genre
* Explicit vs non-explicit track split
* Distribution of 8 core audio features (danceability, energy, speechiness, acousticness, instrumentalness, liveness, valence, tempo)
* Correlation heatmap across all audio features
* Top genres by average popularity
* Feature relationships via scatter plots — loudness vs energy, acousticness vs energy, valence vs popularity
* Top 10 most popular tracks
* Top 10 artists by track count
* Popularity comparison between explicit and non-explicit tracks
* Song duration distribution
* Musical key and mode (major/minor) distribution, mapped from numeric codes to actual note names
* Top genres by danceability

Some Interesting Findings
Some insights I found while exploring the dataset:

* **Pritam** is the most prolific artist in the dataset, reflecting a strong presence of Bollywood music.
* **The Beatles** and **George Jones** lead track count among Western artists.
* **G Major** is the most commonly used musical key.
* **Major key** songs outnumber Minor key songs, meaning more upbeat tracks than sad ones.
* **Explicit tracks** are slightly more popular on average than non-explicit ones.
* **Energy and Loudness** are strongly positively correlated — louder tracks are almost always more energetic.
* **Acousticness and Energy** are negatively correlated — acoustic tracks tend to be low energy.
* **Valence and Popularity** show no clear relationship — a happy-sounding track isn't guaranteed to be popular.
* Most tracks run **2–4 minutes**, with an average duration of **3.87 minutes**.
* **Latin and dancehall** genres top the danceability charts.

Project Structure

```text
.
├── spotify-eda.ipynb
└── README.md
```

How to Run
Clone the repository:

```bash
git clone https://github.com/kushwahaaa27/spotify-tracks-eda.git
```

Open the notebook and run all the cells.

Why I Made This Project
After working with mostly categorical data in my Netflix EDA project, I wanted to practice EDA on a numeric, feature-heavy dataset instead — working with correlation analysis, scatter relationships, and mapping encoded values (like musical key and mode) back to their real meaning. This project is part of my Machine Learning portfolio, and I plan to keep improving my projects as I learn more.

Feedback
If you have any suggestions or notice something that could be improved, feel free to open an issue or share your feedback.
