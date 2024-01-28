# Spotify Data Analysis

by Kristen Beck

A data visualization project focusing on sound feature analysis for the user's Spotify playlists. 
Visualize trends in your own musical preferences and compare your top music with tracks on Spotify’s top playlists.

![app screenshoot](https://github.com/kristenvonbecker/spotify_data_analysis/blob/main/screenshot.png)

This project has two parts, each one found in its on Jupyter notebook. 

## 1. The ETL

This step uses the Spotipy API client to query the user's Spotify playlist data, extracting key audio features which are then cleaned and transformed before being loaded into a CSV file indexed by `track_id` and containing a playlist membership label. Before running this notebook, you will first need to follow [these instructions](https://developer.spotify.com/documentation/web-api/tutorials/getting-started#create-an-app) to set up a Spotify Developer and get your own access tokens (`SPOTIPY_CLIENT_ID` and `SPOTIPY_CLIENT_SECRET`) which should be entered in the API client configuration/authorization step.

## 2. The analysis and visualization

This step uses the Matplotlib and Seaborn libraries to visualize statistical trends of Spotify playlists. Users who were unable to run the ETL notebook and create their own customized dataset should upload the provided sample file `track_df.csv` instead. 
