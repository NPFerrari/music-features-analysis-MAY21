# music-features-analysis-MAY21
In this project, I have analysed how popular songs features have changed over time, starting from 2018 to 2021.


**Introduction:**

For this project, I decided to work on analysing different patterns of the most popular songs over time. In order to do this, I first worked on web scraping the Billboard top100 songs titles and artists by week starting from June 2018 until May 2021. Furthermore, I used the Spotify API wrapper to extract audio features for each of the song and finally analyse the dataset. 


**The dataset:**

The final dataset was constructed by 15k hit songs and their respective audio features. The dataset also presents a variable called "week_popularity" showing in which week the song was popular based on the top100 Billboard website. The audio features are the following and I also provided a short description for each of them: 
- _Instrumentalness_: This value represents the amount of vocals in the song. The closer it is to 1.0, the more instrumental the song is.
- _Acousticness_: This value describes how acoustic a song is. A score of 1.0 means the song is most likely to be an acoustic one.
- _Liveness_: This value describes the probability that the song was recorded with a live audience. According to the official documentation “a value above 0.8 provides strong likelihood that the track is live”.
- _Speechiness_: “Speechiness detects the presence of spoken words in a track”. If the speechiness of a song is above 0.66, it is probably made of spoken words, a score between 0.33 and 0.66 is a song that may contain both music and words, and a score below 0.33 means the song does not have any speech.
- _Energy_: “(energy) represents a perceptual measure of intensity and activity. Typically, energetic tracks feel fast, loud, and noisy”.
- _Danceability_: “Danceability describes how suitable a track is for dancing based on a combination of musical elements including tempo, rhythm stability, beat strength, and overall regularity. A value of 0.0 is least danceable and 1.0 is most danceable”.
- _Valence_: “A measure from 0.0 to 1.0 describing the musical positiveness conveyed by a track. Tracks with high valence sound more positive (e.g. happy, cheerful, euphoric), while tracks with low valence sound more negative (e.g. sad, depressed, angry)”.


**Analysis of audio feaatures over time**:

The analysis in a nutshell was constructed starting from creating a set of clusters in the first top 100 song (week 1, June 2018) using an unsupervised machine learning model (K_means). From this model, we obtained three clusters. Afterwards, with a cascading procedure, I run several KNearestNeighbours models, which would assign one of the three clusters created in week 1 on the following week, by looking at the cluster of the previous week. 
Week 1
  Week 2
    Week 3
      Week 4
        Week 5
          ......
            Week 148
              Week 149
                Week 150


**Key Takeaways**:

The aim for using this procedure was to see if it would have been possible to spot certain trends of music overtime by studying their audio features. Here's what I found out: 
- MUSIC AS A SOCIAL CONSTRUCT
  Relationship between music and culture:
  Musical sounds and practices in a given collectivity are relative to the respective social
  functions music carries out in any particular cultural setting.
- PRODUCERS ADAPT TO TRENDS / SPOTIFY
  No significant changes in the clusters:
  --> labels fit trends and barely move from 'what works', even if genres of songs differs
- AUDIO FEATURES SONGS:
  Stay in the range of what works
  Acoustic songs --> popular in Winter (Dec, Xmas time)
  Danceable/Valence (happier) songs --> popular in Summer time (Jun)
      
      

**For an in-depth view on the project, this repository contains also a pdf presentation and the python codes. Have fun and let me know if you like my work!**
