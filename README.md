# Top Songs Main Characteristics
Playlists are becoming one of the most renowned ways to listen to music and understanding it can be a intricate part. The following work presents a classification model to identify successful songs by their distinct features based on top chart playlists from 2017 to 2019 from Spotify. In our music survey we perform in depth EDA, feature correlations, detailed distribution analysis and PCA  to hinge on popularity score. We perform numerous algorithms to substantiate our hypothesis like xgb and tSNE methodology and then we  assent it  with spotify's 1921-2020 dataset's popularity matrix. Our assessment reveals the  main components to engender a successful top-song. We consummate by affirming  how  features like "energy", "liveness", "tempo", "valence" and "danceability" can be a benchmark to arbitrate a top song and also be able to collocate  top and not the top-songs.

#### Description of song features
- **duration_ms** - The duration of the track in milliseconds.
- **tempo** - Beats per minute The overall estimated tempo of a track in beats per minute (BPM). In musical terminology, tempo is the speed or pace of a given piece and derives directly from the average beat duration.
- **energy** - Energy is a measure from 0.0 to 1.0 and represents a perceptual measure of intensity and activity. Typically, energetic tracks feel fast, loud, and noisy. For example, death metal has high energy, while a Bach prelude scores low on the scale. Perceptual features contributing to this attribute include dynamic range, perceived loudness, timbre, onset rate, and general entropy.
- **danceability** - Describes how suitable a track is for dancing based on a combination of musical elements including tempo, rhythm stability, beat strength, and overall regularity. A value of 0.0 is least danceable and 1.0 is most danceable.
- **loudness** - The overall loudness of a track in decibels (dB). Loudness values are averaged across the entire track and are useful for comparing relative loudness of tracks. Loudness is the quality of a sound that is the primary psychological correlate of physical strength (amplitude). Values typical range between -60 and 0 db.
- **liveness** - Detects the presence of an audience in the recording. Higher liveness values represent an increased probability that the track was performed live. A value above 0.8 provides strong likelihood that the track is live.
- **acousticness** - A confidence measure from 0.0 to 1.0 of whether the track is acoustic. 1.0 represents high confidence the track is acoustic.
- **speechiness** - Speechiness detects the presence of spoken words in a track. The more exclusively speech-like the recording (e.g. talk show, audio book, poetry), the closer to 1.0 the attribute value. Values above 0.66 describe tracks that are probably made entirely of spoken words. Values between 0.33 and 0.66 describe tracks that may contain both music and speech, either in sections or layered, including such cases as rap music. Values below 0.33 most likely represent music and other non-speech-like tracks.
- **key** - The estimated overall key of the track. Integers map to pitches using standard Pitch Class notation . E.g. 0 = C, 1 = C♯/D♭, 2 = D, and so on. If no key was detected, the value is -1.
- **valense** - A measure from 0.0 to 1.0 describing the musical positiveness conveyed by a track. Tracks with high valence sound more positive (e.g. happy, cheerful, euphoric), while tracks with low valence sound more negative (e.g. sad, depressed, angry).
- **mode** - Mode indicates the modality (major or minor) of a track, the type of scale from which its melodic content is derived. Major is represented by 1 and minor is 0.
- **time signatur** - An estimated overall time signature of a track. The time signature (meter) is a notational convention to specify how many beats are in each bar (or measure).

## **Table of Contents**:
  - **exploration**: This contains jupyter notebooks with Data Analysis
    - Analysis on top songs in the years 2017, 2018, and 2019
    - Comparison top songs from 2017, 2018 and 2019,
    - Analysis of top songs artists.
  - **data**: Csv-files with Spotify playlists (See sources below)
    - Top Spotify Tracks of 2017
    - Top Spotify Tracks of 2018
    - Spotify Dataset 1921-2020, 160k+ Tracks
    - Datasets top50 2017
    - Datasets top50 2018
    - Top 50 Spotify Songs - 2019

## **Installation**:
To run this project there are 2 ways, preferably 1:

1. Go to :https://github.com/fneitzel/DataAnalysisOnMusicPreferences/tree/master/exploration
   and Execute the jupyter files independently 

OR

2. Install the dependencies with

> pip install requirements2.txt

Manual installation:

1) Make sure Python 3.x along with pip is installed
> python --version
#should be Python 3.x
2) Install virtual environment
> pip install virtualenv
3) Create the virtual environment
> virtualenv 'VEnvForSpotifyProject'
4) Activate the virtual environment
> source 'VEnvForSpotifyProject'/bin/activate # Linux/Mac
  
> 'VEnvForSpotifyProject'\Scripts\activate # Windows
5) Install needed dependecies:
> pip install jupyter spotipy pandas seaborn textblob xgboost sklearn plotly
    
For running the data_mining code make sure to install spotipy and use your own SPOTIPY_CLIENT_SECRET and SPOTIPY_CLIENT_ID 


## Sources
- Spotify API. Available under:  https://developer.spotify.com/documentation/web-api/reference/tracks/
- Nadin Tamer. Top Spotify Tracks of 2017. Available under: https://www.kaggle.com/nadintamer/top-tracks-of-2017
- Nadin Tamer. Top Spotify Tracks of 2018. Available under: https://www.kaggle.com/nadintamer/top-spotify-tracks-of-2018
- Leonardo  Henrique.  Top  50  Spotify  Songs  -  2019. Available   under: https://www.kaggle.com/leonardopena/top50spotify2019
- Yama ̧c Eren Ay. Spotify Dataset 1921-2020, 160k+ Tracks. Available under: https://www.kaggle.com/yamaerenay/spotify-dataset-19212020-160k-tracks

## **Experiment**:

![alt text](https://github.com/fneitzel/DataAnalysisOnMusicPreferences/blob/master/Charts/flowchart.png?raw=true "FLOWCHART")

