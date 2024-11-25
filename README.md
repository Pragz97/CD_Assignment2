# CD_Assignment2 - Corpus Collection
## Project Description
Data collection and processing with spaCy and pandas for the purpose of lyrical (textual) analysis. <br>
The corpus is a collection of the lyrics of the singles released from Metal band _Ice Nine Kills_'s (INK) horror-media-themed albums _The Silver Scream_ (2018) and _The Silver Scream 2: Welcome to Horrorwood_ (2021). 
<p> The corpus underwent tokenization, lemmatization, and parts-of-speech (POS) tagging, and analysis to identify proper nouns as an example of the type of analysis that can be conducted on the corpus. </p>
<p> This processed corpus can be used by fans of the band, the genre, or horror-media and/or researchers interested in music inspired by other media in some form. </p>

## Features
### Contents
This repository (in addition to this README file) includes:
1. a folder titled **Data** that contains the corpus of fifteen text files, each containing the lyrics of one of the singles released from either _Silver Scream_ album.
2. A Jupyter Notebook file containing the code for the data processing.
3. A CSV file with the corpus metadata compiled by myself.
4. A CSV file titled **INK_silverscream_singles_with_spaCy_tags** combining all the metadata from the previous file, each document's text (lyrics), and the results of the corpus processing and analysis conducted

<p>The above CSV contains the following dataset variables </p>

|Header|Description|DataType|
|---|---|---|
|Filename|Name of the .txt file with the lyrics|Text
|Title|Name of the single (including any featured artists)|Text
|Track listing|Position of the single in the album|Number
|Song Length|Length of the song in mm:ss format|Time Stamp
|Release Date|Date the single was released|Date
|Album|Album the single belongs to|Text
|Horror Reference|The piece of horror media (book, movie, videogame, etc) which inspired the song|Text
|Lyric Source|The source of the lyrics|Text
|Text|The actual lyrics of the single|Text
|Doc|The DOC object resulting from applying spaCy to the text to enrich it for processing|Text
|Tokens|A list of tokens returned after the text's tokenization|Text
|Lemmas|A list of the lemmas returned after the text's lemmatization|Text
|POS|A list of the parts-of-speech tagged within the song's lyrics|Text
|Proper_Nouns|A list of proper nouns identified within the song lyrics (an example of corpus analysis processses that can be applied to this corpus|Text

## Corpus Collection
### Data Collection and Pre-processing
I avoided copying the lyrics directly from their source. Instead, I googled the songs and copy-pasted the lyrics from the "Lyrics" tab, noting the source indicated at the end of the lyrics. This meant that I could skip pre-processing the lyrics (removing verse tags like 'Chorus' and 'Bridge', etc). The lyrics of each of the selected songs were pasted into the Notepad application and saved as .txt files in a folder titled **Data**. 

### Selection Criteria
<p> As a fan of Ice Nine Kills, I think that the way they incorporate references (both direct and implied) to horror media in their music is clever and interesting. Initially, I had decided on collecting the lyrics of all the songs from both Silver Scream albums for the corpus but it would be too big for this project. 

<p> To reduce the corpus to a more manageable size, I decided to select only the singles from the albums. Not only are they the songs the band chose to increase audience engagement with the albums, in INK's case, they are also the songs whose music videos form the movie-esque "plot" of the album's videos. </p>

<p> Some (not all) of the singles from The Silver Scream follow the plot of Spencer Charnas (the band's lead singer) visiting a psychiatrist to talk about the vivid dreams (music videos referencing popular horror movies) that disturb his rest, culminating in the death of the psychiatrist. </p>

The singles from this album are as follows: 
1. Enjoy Your Slay
2. The American Nightmare
3. Thank God It's Friday
4. A Grave Mistake
5. Stabbing in the Dark
6. Merry Axe-mas
7. Savages
8. IT is the End
<p> The music videos for singles 1, 6, and 7 do not follow the album's video narrative </p>

<p>In the following album, Welcome to Horrorwood, the music videos (bar one) end or begin as part of the album's video narrative wherein the music videos themselves are 'found tapes' that are part of the evidence in the court case against Spencer Charnas who has been accused of murdering his fiancee. </p>

The singles from this album are as follows:
1. Hip to be Scared
2. Assault & Batteries
3. Rainy Day
4. Funeral Derangements
5. Take Your Pick
6. The Shower Scene
7. Welcome to Horrorwood

<p> "Take Your Pick" is not part of the over-arching album plot </p>

## Annotations and Tools
<p> As can be noted from the table included above, I used POS tagging as an annotation and used it to extract Proper Nouns from the lyrics that could indicate the horror-media that inspired the single as can be seen in the example in the Jupyter notebook </p>

### Tools Used
1. Notepad application to paste the lyrics and save them as .txt files.
2. Git Bash to add and commit the various files to GitHub
3. Jupyter Notebook to write the code and conduct the text processing.
4. spaCy and pandas packages to enable the data processing.

### _______________________________________________________________________________________ 


