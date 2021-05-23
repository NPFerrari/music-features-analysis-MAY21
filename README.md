# music-features-analysis-MAY21
In this project, I have analysed how popular songs features have changed over time, starting from 2018 to 2021.

**Introduction:**
For this project, I decided to work on analysing different patterns of the most popular songs over time. In order to do this, I first worked on web scraping the Billboard top100 songs titles and artists by week starting from June 2018 until May 2021. Furthermore, I used the Spotify API wrapper to extract audio features for each of the song and finally analyse the dataset. 

**Analysis:**
The final dataset was constructed by 15k hit songs and their respective audio features. The audio features are the following and I also provided a short description for each of them: 
- Instrumentalness: This value represents the amount of vocals in the song. The closer it is to 1.0, the more instrumental the song is.
- Acousticness: This value describes how acoustic a song is. A score of 1.0 means the song is most likely to be an acoustic one.
- Liveness: This value describes the probability that the song was recorded with a live audience. According to the official documentation “a value above 0.8 provides strong likelihood that the track is live”.
- Speechiness: “Speechiness detects the presence of spoken words in a track”. If the speechiness of a song is above 0.66, it is probably made of spoken words, a score between 0.33 and 0.66 is a song that may contain both music and words, and a score below 0.33 means the song does not have any speech.
- Energy: “(energy) represents a perceptual measure of intensity and activity. Typically, energetic tracks feel fast, loud, and noisy”.
- Danceability: “Danceability describes how suitable a track is for dancing based on a combination of musical elements including tempo, rhythm stability, beat strength, and overall regularity. A value of 0.0 is least danceable and 1.0 is most danceable”.
- Valence: “A measure from 0.0 to 1.0 describing the musical positiveness conveyed by a track. Tracks with high valence sound more positive (e.g. happy, cheerful, euphoric), while tracks with low valence sound more negative (e.g. sad, depressed, angry)”.
