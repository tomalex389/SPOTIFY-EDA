

[**SPOTIFY**](http://www.prezentr.com/?utm_source=templates&utm_medium=presentation&utm_campaign=free_downloads_2020)[** ](http://www.prezentr.com/?utm_source=templates&utm_medium=presentation&utm_campaign=free_downloads_2020)[PLAYLIST**](http://www.prezentr.com/?utm_source=templates&utm_medium=presentation&utm_campaign=free_downloads_2020)

[**AUDIO**](http://www.prezentr.com/?utm_source=templates&utm_medium=presentation&utm_campaign=free_downloads_2020)[** ](http://www.prezentr.com/?utm_source=templates&utm_medium=presentation&utm_campaign=free_downloads_2020)[FEATURES**](http://www.prezentr.com/?utm_source=templates&utm_medium=presentation&utm_campaign=free_downloads_2020)

[**EDA**](http://www.prezentr.com/?utm_source=templates&utm_medium=presentation&utm_campaign=free_downloads_2020)

[TO](http://www.prezentr.com/?utm_source=templates&utm_medium=presentation&utm_campaign=free_downloads_2020)[ ](http://www.prezentr.com/?utm_source=templates&utm_medium=presentation&utm_campaign=free_downloads_2020)[M](http://www.prezentr.com/?utm_source=templates&utm_medium=presentation&utm_campaign=free_downloads_2020)[ ](http://www.prezentr.com/?utm_source=templates&utm_medium=presentation&utm_campaign=free_downloads_2020)[ALEX](http://www.prezentr.com/?utm_source=templates&utm_medium=presentation&utm_campaign=free_downloads_2020)

[DHRUV](http://www.prezentr.com/?utm_source=templates&utm_medium=presentation&utm_campaign=free_downloads_2020)[ ](http://www.prezentr.com/?utm_source=templates&utm_medium=presentation&utm_campaign=free_downloads_2020)[PATEL](http://www.prezentr.com/?utm_source=templates&utm_medium=presentation&utm_campaign=free_downloads_2020)

[SANDEEP](http://www.prezentr.com/?utm_source=templates&utm_medium=presentation&utm_campaign=free_downloads_2020)[ ](http://www.prezentr.com/?utm_source=templates&utm_medium=presentation&utm_campaign=free_downloads_2020)[UNNIKRISHNAN](http://www.prezentr.com/?utm_source=templates&utm_medium=presentation&utm_campaign=free_downloads_2020)





**Problem / Hypothesis**

What features make a desirable track for Tom?

What features make an undesirable track for Tom?

If we use Spotify’s API to retrieve track attributes along with

visualization libraries to process the data, we will find that Tom

likes tracks that are fast-paced and loud.





**D ATA COLLECTION - SPOTIFY API**

Two playlists totalling 700+ songs

\- liked tracks “YES PLAYLIST”

\- disliked tracks “NO PLAYLIST”

Retrieve playlist IDs

Retrieve Authorization Token

Enter Playlist IDs and Authorization

Token

Retrieve Track IDs in playlists





**D ATA COLLECTION - SPOTIFY API**

**(cont.)**

Retrieve track ids from generated

data





**D ATA COLLECTION - SPOTIFY API**

**(cont.)**

Enter string of trackIDs

separated by commas

for each playlist

Enter Authorization

Token

Save output as .json





**D ATA COLLECTION - SPOTIFY API**

**(cont.)**

We manipulate the data from

these .json files:

\- good.json

\- dislike.json





**Spotify API Documentation**

**Acousticness : A confidence measure from 0.0 to 1.0 of whether the track is acoustic. 1.0 represents high confidence the track is acoustic.**

**Danceability : Danceability describes how suitable a track is for dancing based on a combination of musical elements including tempo, rhythm stability, beat**

**strength, and overall regularity. A value of 0.0 is least danceable and 1.0 is most danceable.**

**Duration\_ms : The duration of the track in milliseconds.**

**Energy : Energy is a measure from 0.0 to 1.0 and represents a perceptual measure of intensity and activity. Typically, energetic tracks feel fast, loud, and noisy.**

**For example, death metal has high energy, while a Bach prelude scores low on the scale. Perceptual features contributing to this attribute include dynamic**

**range, perceived loudness, timbre, onset rate, and general entropy.**

**Instrumentalness : Predicts whether a track contains no vocals. “Ooh” and “aah” sounds are treated as instrumental in this context. Rap or spoken word**

**tracks are clearly “vocal”. The closer the instrumentalness value is to 1.0, the greater likelihood the track contains no vocal content. Values above 0.5 are**

**intended to represent instrumental tracks, but confidence is higher as the value approaches 1.0.**

**Key : The key the track is in. Integers map to pitches using standard Pitch Class notation . E.g. 0 = C, 1 = C♯/D♭, 2 = D, and so on.**

**Liveness : Detects the presence of an audience in the recording. Higher liveness values represent an increased probability that the track was performed live. A**

**value above 0.8 provides strong likelihood that the track is live.**

**Loudness : The overall loudness of a track in decibels (dB). Loudness values are averaged across the entire track and are useful for comparing relative**

**loudness of tracks. Loudness is the quality of a sound that is the primary psychological correlate of physical strength (amplitude). Values typical range**

**between -60 and 0 db.**

**Mode : Mode indicates the modality (major or minor) of a track, the type of scale from which its melodic content is derived. Major is represented by 1 and minor**

**is 0.**

**Speechiness : Speechiness detects the presence of spoken words in a track. The more exclusively speech-like the recording (e.g. talk show, audio book,**

**poetry), the closer to 1.0 the attribute value. Values above 0.66 describe tracks that are probably made entirely of spoken words. Values between 0.33 and 0.66**

**describe tracks that may contain both music and speech, either in sections or layered, including such cases as rap music. Values below 0.33 most likely**

**represent music and other non-speech-like tracks.**

**Tempo : The overall estimated tempo of a track in beats per minute (BPM). In musical terminology, tempo is the speed or pace of a given piece and derives**

**directly from the average beat duration.**

**Time\_signature : An estimated overall time signature of a track. The time signature (meter) is a notational convention to specify how many beats are in each**

**bar (or measure).**

**Valence : A measure from 0.0 to 1.0 describing the musical positiveness conveyed by a track. Tracks with high valence sound more positive (e.g. happy,**

**cheerful, euphoric), while tracks with low valence sound more negative (e.g. sad, depressed, angry).**





Data Cleaning / Data Prep

Imported Libraries:

Open/Load JSON files

Did the same for

dislike.json





Data Cleaning (cont.)

Did the same

for dislike

Convert DF to CSV

Unique

Values





Data Cleaning / Data Prep (cont.)

Drop Columns

Merge DFs

Find Missing Cells

Did the

same

for

dislike





**Data Cleaning (cont.)**

Find Null and

Duplicated

Values

Checking For Outliers





**Outliers**

● **No outliers were removed as it**

**defines the extreme**

**forwardness of the song**

**towards that audio feature**





**Sav ing Data to MySQL**





**Heat Map**

**Correlated**

**Highly-Correlated**





**Scatter Plots**

**duration\_ms x energy**

**duration\_ms x tempo**

**right\_g = ['acousticness', 'energy', 'valence',**

**'tempo', 'loudness', 'danceability']**

**for x in right\_g:**

**scatterprint(data, 'duration\_ms', x)**

**duration\_ms x energy**

● To m favors high energy (high intensity and activity) and typically shorter duration

tracks

**duration\_ms x tempo**

● To m favors high BPM tracks with varying levels of duration





**Scatter Plots (cont.)**

**duration\_ms x loudness duration\_ms x danceability**

**duration\_ms x loudness**

● To m favors very loud tracks over anything else

**duration\_ms x danceability**

● To m favors tracks with over 0.4 in danceability and typically

shorter duration tracks





**Scatter Plots (cont.)**

**loudness x acousticness**

**loudness x energy**

**right\_g = ['acousticness', 'energy', 'valence', 'tempo',**

**'instrumentalness', 'acousticness', 'danceability']**

**for x in right\_g:**

**loudness x acousticness**

● To m favors loudness over acousticness

**scatterprint(data, 'loudness', x)**

**loudness x energy**

● To m favors songs with high energy and loudness





**Scatter Plots (cont.)**

**loudness x valence**

**loudness x tempo**

**loudness x danceability**

**loudness x valence**

● To m favors loud songs irregardless of valence (musical positiveness)

**loudness x tempo**

● To m favors loud songs irregardless of tempo (bpm)

**loudness x danceability**

● To m favors tracks that are danceable and loud





**Scatter Plots (cont.)**

**danceability x acousticness**

**danceability x energy**

**danceability x acousticness**

● To m favors danceability over acousticness

**danceability x energy**

● To m favors songs with high energy and danceability





**ie Chart**

**labels = ["4 beats per Bar","3 beats per Bar","5 beats per Bar","1 beats per Bar"]**

**explode = [0.1, 0.1, 0.1, 0.1]**

**plt.pie(data\_pie ,labels= labels , explode = explode , autopct="%1.2f%%", shadow=**

**True, colors= ['#ebf707','#c0c90a','#929908','#686e05'])**

**plt.legend()**

**plt.show()**





**Pie Chart**

**Beats Per Bar**

DislIked Tracks

LIked Tracks





**Histograms**

**- every liked track ranks at**

**least 0.5 in danceability**

**- although a track may have**

**high danceability, it is not**

**necessarily liked**

**- disliked tracks has a bimodal**

**shape in danceability**

**- liked tracks are negatively**

**skewed(skewed left) in**

**danceability**

**plt.figure(figsize=(10,5))**

**plt.suptitle('Histograms of danceability', fontsize = 20)**

**ax1 = sns.histplot(x = data['danceability'],color= 'teal', hue= data['liking'], bins= 15, kde= True, palette= 'YlOrRd')**

**ax1.set(xlabel= 'danceability', ylabel= 'Frequency')**

**plt.tight\_layout()**

**plt.show()**





**Histograms (cont.)**

**- every liked track ranks at**

**least -15db in loudness**

**- although a track may be loud**

**it is not necessarily liked**

**- liked and disliked tracks are**

**negatively skewed(skewed**

**left) in loudness**

**plt.figure(figsize=(10,5))**

**plt.suptitle('Histograms of loudness', fontsize = 20)**

**ax1 = sns.histplot(x = data['loudness'],color= 'teal', hue= data['liking'], bins= 15, kde= True, palette= 'Greens')**

**ax1.set(xlabel= 'loudness', ylabel= 'Frequency')**

**plt.tight\_layout()**

**plt.show()**





**Histograms (cont.)**

**- liked tracks vary in**

**speechiness, but are generally**

**higher in speechiness**

**compared to disliked tracks**

**- disliked tracks are typically**

**low in speechiness**

**- disliked tracks are more**

**positively skewed(skewed**

**right) than liked tracks**

**plt.figure(figsize=(10,5))**

**plt.suptitle('Histograms of speechiness', fontsize = 20)**

**ax1 = sns.histplot(x = data['speechiness'],color= 'teal', hue= data['liking'], bins= 15, kde= True, palette= 'BuPu')**

**ax1.set(xlabel= 'speechiness', ylabel= 'Frequency')**

**plt.tight\_layout()**

**plt.show()**





**Histograms (cont.)**

**- liked tracks are generally**

**high in tempo, around 150**

**bpm**

**- disliked tracks are**

**generally lower than liked**

**tracks in tempo around, 110**

**bpm**

**- disliked tracks are slightly**

**positively skewed(skewed**

**right) while liked tracks, are**

**slighly negatively skewed**

**plt.figure(figsize=(10,5))**

**plt.suptitle('Histograms of tempo', fontsize = 20)**

**ax1 = sns.histplot(x = data['tempo'],color= 'yellow', hue= data['liking'], bins= 15, kde= True, palette= 'rocket')**

**ax1.set(xlabel= 'tempo', ylabel= 'Frequency')**

**plt.tight\_layout()**

**plt.show()**





**Histograms (cont.)**

**- liked tracks (<3.5 min) are**

**generally low in duration**

**compared to disliked tracks**

**(<4 min)**

**- disliked and liked tracks are**

**positively skewed (skewed**

**right)**

**plt.figure(figsize=(10,5))**

**plt.suptitle('Histograms of Duration of the song', fontsize = 20)**

**ax1 = sns.histplot(x = data['duration\_ms'],color= 'yellow', hue= data['liking'], bins= 15, kde= True, palette= 'twilight')**

**ax1.set(xlabel= 'Duration', ylabel= 'Frequency')**

**plt.tight\_layout()**

**plt.show()**





**Histograms (cont.)**

**- liked tracks are generally**

**higher in valence compared to**

**disliked tracks**

**- disliked tracks vary in**

**valence from low to high and**

**cannot be generalized**

**- disliked tracks have a**

**bimodal distribution (two**

**peaks) while liked tracks, are**

**slighly negatively skewed**

**(skewed left)**

**plt.figure(figsize=(10,5))**

**plt.suptitle('Histograms of Valence', fontsize = 20)**

**ax1 = sns.histplot(x = data['valence'],color= 'yellow', hue= data['liking'], bins= 15, kde= True, palette= 'RdBu')**

**ax1.set(xlabel= 'Valence', ylabel= 'Frequency')**

**plt.tight\_layout()**

**plt.show()**





**Pairplots**

Liked Tracks

Disliked Tracks





**Bar Graphs**





**Bar Graphs**





**Summary - Conclusions**

Based on the EDA, we can say that the features posing high importance for Tom are:

● Highly danceable

● highly energetic

● loudness

● high in tempo

● lower than 300,000 ms or 5 min in duration

● mood of the song, generally happier ones(valence)

Link to the greatest playlist ;)

<https://open.spotify.com/playlist/70CQj2Fu063UNJBQCI5IIW?si=28f208b89f634018>

