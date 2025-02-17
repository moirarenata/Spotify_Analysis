# Spotify Wrapped (Moira's Version) 

We can all agree that the 2024 Spotify Wrapped was a bit of a letdown. Everyone was waiting to hear about their music aura location based on their listening activity for the past year. 
Instead, we got AI-generated music evolutions like Pink Pilates Princess and Vampire Rock April—seriously, what does that even mean? 
So, I took matters into my own hands and explored my Spotify listening activity using Spotify’s API to uncover some interesting stats! 
This repository contains the code and data needed to perform and reproduce the analysis. (Client ID and Client Secret have been removed.)

# Overview 

This project explores my Spotify listening history, retrieves song lyrics, and applies sentiment analysis to understand trends in the music I listen to. By integrating Spotify API, Genius API, and BERT-based NLP, I examine both listening patterns and lyrical sentiment trends to generate a customized Spotify Wrapped experience.


**Repository structure:**

```
Spotify_Analysis/
├── data/                           
│   ├── Lyrics_Noah_Kahan.csv        # Raw lyrics dataset
│   ├── Lyrics_Noah_Kahan_bert.csv   # Lyrics with BERT sentiment scores
│   ├── Lyrics_Noah_Kahan_Sentiment_BERT.csv  # Processed sentiment data
│   ├── Lyrics_NoahKahan.json        # Raw lyrics in JSON format
│   ├── StreamingHistory_music_0.json  # Spotify streaming history (multiple files)
│   ├── StreamingHistory_music_1.json
│   ├── StreamingHistory_music_2.json
│   ├── StreamingHistory_music_3.json
│
├── data_viz/                        # Cleaned data used for visualization
│
├── src/                             # Jupyter Notebooks for analysis
│   ├── clean_lyrics_nk.ipynb        # Preprocesses and cleans song lyrics
│   ├── scrape_lyrics_genius.ipynb   # Extracts lyrics using the Genius API
│   ├── senti_analysis_ot.ipynb      # Applies sentiment analysis to lyrics
│   ├── spotify_analysis.ipynb       # Analyzes Spotify listening history and trends
│
└── README.md                        # Project documentation
```
