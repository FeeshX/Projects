## **Music Analysis of T.V Show Soundtracks using the Spotify API and Python**

![MadMen and Whitelines](https://github.com/mishaisran/Projects/blob/master/Spotify%20API/Images/Header%20Project.png)

**Overview**
---
Soundtracks are an important piece in the composition of any T.V show and movie. 
Artfully placed pieces bring life and add an extra dimension of a moment. Music gives a higher chance of success because of how it entraps and guides the audience to the story as it unfolds. In this analysis, I look at whether there is a variation in the musical composition of two popular T.V Shows that vary significantly in genre and theme. 

- **Madmen** *is an American period-drama set in the 1960s about a New York advertising agency, focusing on their personal lives of the people and families who work there during the tumultuous and divisive decade.*

- **Whitelines** *is a British-Spannish mystery thriller 
set between ‘90s Manchester and present-day club-laden Ibiza about a woman investigating the suspicious and long-abandoned dissaparence of her free-spirited brother twenty years ago.*

**Spotify Audio Features**
---
To access Spotify's API, I created a developer account. Once the account was created, I was provided a 'client id' and 'client secret' as authorization credentials to use within my code. I extracted data on pre-defined audio features that reflect the characteristics of a song from Spotipy, a Python library for the Spotify Web API. The resulting dataset is 98 rows and 15 columns for the Whitelines soundtrack and 100 rows and 15 columns for the Madmen soundtrack. Each row reflects a track on the playlist. To extract data on audio features for each track, I pulled the username of the playlist (found in the Profile link URL) of the person who created the playlist, and the the playlist URI.

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

![Mean Values](https://github.com/mishaisran/Projects/blob/master/Spotify%20API/Images/Mean%20values.PNG)

According to the visual, Madmen has music that is high in acousticness, energy and danceability. This is typical of what one would expect in a 60s melodrama that is packed with instrumentals, funk-soul, pop-rock and classics. Whitelines in contrast, does lower in acousticness but high in energy and danceability as most of its soundtrack comprises of up-beat, electric, modern tunes. 

![Radar Chart](https://github.com/mishaisran/Projects/blob/master/Spotify%20API/Images/Mean%20values%20Radar%20Chart.PNG)

I next looked at how varied each playlist is. A very varied playlist encompasses songs from multiple genres. The opposite of this, a low varied playlist, is one where songs mostly fall under the same genre. For this the standard deviation of the audio features were calculated. Madmen has a mean S.D of 0.195 and a greater variety in its song selection than Whitelines with a mean S.D of 0.146 by a marginal amount. Madmen has the greatest variety in songs within the instrumentalness characteristic whereas Whitelines has the greatest variety in acousticness.

![Variety](https://github.com/mishaisran/Projects/blob/master/Spotify%20API/Images/Variety.PNG)

![MadMen and Whitelines](https://github.com/mishaisran/Projects/blob/master/Spotify%20API/Images/SD%20of%20shows.PNG)

The last comparative variable I analysed was song release year. As shown in the diagram below, Whitelines comprises mostly of new, modern tracks that were produced from 2016 and ahead, whereas Madmen has a versatile playlist with songs spanning decades from the 1950's all the way to 2020. Note that the show concluded in 2015. The songs identified in the chart following this year represent instrumental music such as relaxing piano music, rain drops etc. that have been since then reproduced. This is one limitation of the data as the selected playlists on Spotify are curated by individuals and not music composers/producers/supervisors of the show. 
 
 ![Soundtracks by Release Year](https://github.com/mishaisran/Projects/blob/master/Spotify%20API/Images/Soundtracks%20by%20Release%20Year.PNG)

**Next Steps**
---
The analysis shows that there is a slight difference between the soundtracks of the Madmen and Whitelines in areas such as energy, danceability, liveness and tempo but a significant difference in other audio features such as acousticness and release year. When selecting tracks for upcoming productions, music directors can shortlist those that fit with ones that possess a similar audio feature profile (defined below) as the ones used in existing, successful T.V shows. This would provide a data-driven way to pair a show with a song based on past data rather than scanning thousands of tracks and spending hours finding the right tune. The code serves as a template to compare the difference in musical composition of two soundtracks based on Spotify's pre-defined audio variables.

**Project Info**
---
<pre>
Contributor  : <a href=https://github.com/Al-Cap>Misha Isran</a>
</pre>

<pre>
Languages    : Python
Tools/IDE    : Anaconda
Libraries    : Spotipy, pandas, matplotlib, numpy, time
</pre>
  </tbody>
</table>
