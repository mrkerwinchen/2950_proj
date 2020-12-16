# Trends in Song Lyrics Over Time (1960's to 2010's)

### Kerwin Chen

[Full analysis here.](https://github.com/mrkerwinchen/2950_proj/blob/master/song_lyrics_trends.ipynb)
Music has changed in the last 50 years, and I was interested in learning about the trends and changes in song lyrics over time, from the 1960's to 2010's. I ran multiple t-tests with an adjusted <img src="https://render.githubusercontent.com/render/math?math=\alpha"> level to control the familywise error rate and found that the difference in length of songs between decades were significant, with an increase in lyric length from the 1960's to 2000's, and a dip in the 2010's. I created a logistic regression model with terms as predictors and decades as output, and determined the characteristic terms, ie terms whos presence indicate a high probability that a song is from a certain decade, as follows:

| Decade | Characteristic Terms                                                                      |
|:------:|:------------------------------------------------------------------------------------------|
| 1960's | darling, loneliness, heartaches, untrue, clown, kissed, arms                              |
| 1970's | behind, lord, woman, sorrow                                                               |
| 1980's | shatter, near, hearts, resist, lasts, clover, jamming, romance, fantasy                   |
| 1990's | pain, step, speak, inside, brothers, yo, loves, confess, silence                          |
| 2000's | wanna, three, thang, wishing, club, butterflies, taken, waking, breathe                   |
| 2010's | i'ma, dark, broke, couch, hate, beautiful, fuckin', shit, missing, wasted, tryna, already |

The characteristic terms for each decade seem to be thematically linked. The 1960's, for example, had 'darling', 'loneliness', and 'heartaches' as characteristic terms, words that have very affectionate and deeply emotional connotations. On the other hand, in the 2010's, we had 'dark', 'broke', 'hate', 'fuckin'', 'shit', and 'wasted' as characteristic terms, which are noticeably darker and more aggressive terms. This may be a reflection of the change in subject matters found within songs, and further sentiment analysis in the future may reveal whether there are true thematic shifts in songs as the decades progress. A model made with the characteristic terms may be useful to lyricists, as they would be able to determine which decade their lyrics most closely resemble, and use this as one of the factors to keep in mind when producing and marketing songs to a specific generation of listeners.