**Background**

Soundtracks are an important piece in the composition of any T.V show and movie. 
Artfully placed pieces bring life and add an extra dimension to the content and enable a certain 
rhythm to each scene and segment. Music gives a higher chance of success because of how it entraps 
and guides the audience to the story as it unfolds.

This analysis looks at whether there is a difference in the musical composition of two 
popular T.V Shows, Madmen and Whitelines, that contrast significantly in terms of genre and theme.
- **Madmen** is an American period-drama set in the 1960s about a New York advertising agency,
focusing on their personal lives of the people and families who work there during the 
tumultuous and divisive decade. 
- **Whitelines** is a British-Spannish mystery thriller 
set between ‘90s Manchester and club-laden Ibiza about a woman investigating the suspicious and
long-abandoned dissaparence of her free-spirited brother twenty years ago.

This findings... 

**Method**

For this project, I scraped data from Spotify, which is a popular music streaming service. 
I used Spotipy, "a lightweight Python library for the Spotify Web API", to access the data 
for the two playlists. I extracted data on pre-defined audio features for all the songs 
within the Madmen and Whitelies soundtrack. These are defined below: 

- **Acousticness**: A confidence measure from 0.0 to 1.0 of whether the track is acoustic. 
1.0 represents high confidence the track is acoustic. 
- **Danceability**: Danceability describes how suitable a track is for dancing based on a
combination of musical elements including tempo, rhythm stability, beat strength, and 
overall regularity. A value of 0.0 is least danceable and 1.0 is most danceable. 
- **Energy**: Energy is a measure from 0.0 to 1.0 and represents a perceptual measure of 
intensity and activity. Typically, energetic tracks feel fast, loud, and noisy. 
Perceptual features contributing to this attribute include dynamic range, perceived loudness,
timbre, onset rate, and general entropy.
- **Instrumentalness**: Predicts whether a track contains no vocals. The closer the 
instrumentalness value is to 1.0, the greater likelihood the track contains no vocal content. Values above 0.5 are intended to represent instrumental tracks, but confidence is higher as the value approaches 1.0. 
- **Liveness**: Detects the presence of an audience in the recording. Higher liveness values
represent an increased probability that the track was performed live. A value above 0.8 
provides strong likelihood that the track is live. 
- **Loudness**: The overall loudness of a track in decibels (dB). Loudness values are 
averaged across the entire track and are useful for comparing relative loudness of tracks.
Loudness is the quality of a sound that is the primary psychological correlate of physical
strength (amplitude).
- **Speechiness**:	Speechiness detects the presence of spoken words in a track. The more
exclusively speech-like the recording (e.g. talk show, audio book, poetry), the closer to
1.0 the attribute value. Values above 0.66 describe tracks that are probably made entirely 
of spoken words. Values between 0.33 and 0.66 describe tracks that may contain both music 
and speech, either in sections or layered, including such cases as rap music. Values below
0.33 most likely represent music and other non-speech-like tracks. 
- **Tempo**: The overall estimated tempo of a track in beats per minute (BPM). 


