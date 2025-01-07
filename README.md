Spotify Mood Analysis: Investigating the Shift in Music Preferences Post-COVID-19

___________________
OVERVIEW

This project explores whether listeners in the U.S. shifted from upbeat, high-energy music to more mellow genres after the COVID-19 pandemic. Leveraging Spotify and Apple Music APIs, our team analyzed audio features of top-streamed songs from 2019, 2022, and 2023 to identify patterns in music preferences before and after the pandemic.

___________________
RESEARCH QUESTION

Did the COVID-19 pandemic alter music preferences in the U.S., causing a shift from upbeat genres to more mellow ones?

___________________
KEY FINDINGS

No significant change: Statistical tests and classification methods showed no substantial shift in listener preferences. Upbeat music dominated top charts in all years analyzed.
Temporary shifts: While 2022 saw an increase in upbeat music, 2023 showed a return to slightly more acoustic and less positive tracks.

___________________
DATA SOURCES

The datasets were generated using:
1. Spotify API
2. Apple Music API
   
These included the top 100 streamed songs for each year and their detailed audio features:
Danceability
Energy
Valence
Acousticness
Loudness
Mode, among others.

___________________
METHODOLOGY

1. Statistical Hypothesis Testing:
Compared means of audio features (e.g., Energy, Valence) across years.
T-tests and z-tests revealed no statistically significant differences.

2. Simplified Classification:
Songs were categorized as upbeat (+1) or sad (-1) using a scoring system based on 11 audio metrics.
Proportions of upbeat vs. sad songs remained consistent across the years.

___________________
TOOLS AND TECHNOLOGIES

Programming: Python (Pandas, NumPy)
Data Visualization: Matplotlib, Seaborn
Data Collection: Spotify and Apple Music APIs

___________________
LIMITATIONS

Focused on top 100 streamed songs, which may bias results toward popular genres.
Did not analyze lyrical content due to the absence of Natural Language Processing (NLP) tools.
Thresholds for classifying songs as upbeat or sad were subjective.

___________________
FUTURE WORK

Incorporate lyrical analysis using NLP to better understand emotional tone.
Expand analysis to include niche and less mainstream genres.
Explore the role of cultural and environmental factors in shaping music preferences.
Team
Kenjee Koh
Becky Wang
Vy Nguyen
Dennis Wu
Hsiang-Han (Cyan) Huang
