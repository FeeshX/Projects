## **Scraping the Spotify API using Python to Compare the Audio Features of Soundtracks in Two Popular T.V Shows**

![MadMen and Whitelines](https://github.com/mishaisran/Projects/blob/master/Spotify%20API/Images/Header%20Project.png)

**Overview**
---
Soundtracks are an important piece in the composition of any T.V show and movie. 
Artfully placed pieces bring life and add an extra dimension of a moment. Music gives a higher chance of success because of how it entraps and guides the audience to the story as it unfolds. My analysis looks at whether there is a variation in the musical composition of two popular T.V Shows that vary significantly in genre and theme. I extracted data on pre-defined audio features that reflect the characteristics of a song from Spotipy, a Python library for the Spotify Web API

- **Madmen** *is an American period-drama set in the 1960s about a New York advertising agency, focusing on their personal lives of the people and families who work there during the tumultuous and divisive decade.*
- **Whitelines** *is a British-Spannish mystery thriller 
set between ‘90s Manchester and club-laden Ibiza about a woman investigating the suspicious and long-abandoned dissaparence of her free-spirited brother twenty years ago.*

**Spotify Audio Features**
---
The features retrieved from the API are defined below (*further details available in Spotify's documentation [here](https://developer.spotify.com/documentation/web-api/reference/tracks/get-audio-features/)*): 

| Feature      | Value Description                                                    | 
| :---         | :---              | 
| **Acousticness**   | *A confidence measure from 0.0 to 1.0 of whether the track is acoustic. 1.0 represents high confidence the track is acoustic.*        | 
| **Danceability**     | Danceability describes how suitable a track is for dancing based on a combination of musical elements including tempo, rhythm stability, beat strength, and overall regularity. A value of 0.0 is least danceable and 1.0 is most danceable.*          |
| **Energy**     | *Energy is a measure from 0.0 to 1.0 and represents a perceptual measure of intensity and activity. Typically, energetic tracks feel fast, loud, and noisy. Perceptual features contributing to this attribute include dynamic range, perceived loudness, timbre, onset rate, and general entropy.*          | 
| **Instrumentalness**     | *Predicts whether a track contains no vocals. The closer the  instrumentalness value is to 1.0, the greater likelihood the track contains no vocal content. Values above 0.5 are intended to represent instrumental tracks, but confidence is higher as the value approaches 1.0.*          | 
| **Liveness**    | *Detects the presence of an audience in the recording. Higher liveness values represent an increased probability that the track was performed live. A value above 0.8 provides strong likelihood that the track is live.*          | 
| **Loudness**     | *The overall loudness of a track in decibels (dB). Loudness values are averaged across the entire track and are useful for comparing relative loudness of tracks. Loudness is the quality of a sound that is the primary psychological correlate of physical strength (amplitude).*          | 
| **Speechiness**     | *Speechiness detects the presence of spoken words in a track. The more exclusively speech-like the recording (e.g. talk show, audio book, poetry), the closer to 1.0 the attribute value. Values above 0.66 describe tracks that are probably made entirely  of spoken words. Values between 0.33 and 0.66 describe tracks that may contain both music and speech, either in sections or layered, including such cases as rap music. Values below 0.33 most likely represent music and other non-speech-like tracks.*| 
| **Tempo**    | *The overall estimated tempo of a track in beats per minute (BPM).*          | 


**Analysis of the Data**
---
The diagram below shows the mean values of audio features. 

[diagram here]

According to the visual, Madmen has music that is high in acousticness, energy and danceability. This is typical of what one would expect in a 60s melodrama that is packed with instrumentals, funk-soul, pop-rock and classics. Whitelines in contrast, does lower in acousticness but high in energy and danceability as most of its soundtrack comprises of up-beat, electric, modern tunes. I next looked at how varied each playlist is. A very varied playlist encompasses songs from multiple genres. The opposite of this, a low varied playlist, is one where songs mostly fall under the same genre. For this the standard deviation of the audio features were calculated. Madmen has a greater variety in its song selection than Whitelines by a marginal amount.

**Next Steps**
---
When selecting tracks for upcoming productions, music directors can shortlist those that fit with ones that possess a similar audio feature profile (defined below) as the ones used in existing, successful T.V shows. This would provide a data-driven way to pair a show with a song based on past data rather than scanning thousands of tracks and spending hours finding the right tune. 

**Project Info**
---
<pre>
Contributor  : <a href=https://github.com/Al-Cap>Misha Isran</a>
</pre>

<pre>
Languages    : Python
Tools/IDE    : Anaconda
Libraries    : Spotipy, pandas, matplotlib, numpy
</pre>
  </tbody>
</table>
