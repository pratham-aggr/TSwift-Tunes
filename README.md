# TSwift Tunes: Exploring, Recommending & Searching Through Taylor Swift's Music

Welcome to the **TSwift Tunes** project! This project, completed as part of the DSC 10 course at UC San Diego, explores Taylor Swift’s music through data analysis and machine learning. It includes visualizations, a song recommender system, and a lyrics searcher, all powered by the `tswift` dataset. The project answers key questions about her songs and albums, analyzes audio features, and provides interactive tools for song recommendations and lyric searching.

## Project Overview

This repository contains the following components:

- **Data Exploration and Visualization**: We use the `tswift` DataFrame to explore Taylor Swift's music and answer key questions.
- **Song Recommendation System**: We built a recommender that suggests similar songs based on audio features and user preferences.
- **Lyrics Searcher**: A tool that allows you to search for specific lyrics in Taylor Swift's songs using TF-IDF.
- **Keyword Extraction**: We identify key terms that best summarize each song from Taylor Swift's album *Lover*.

## Data Exploration and Visualization 👀

In this section, we explore Taylor Swift's music through various visualizations, helping us answer the following key questions:

- **How many songs did Taylor Swift release each year?**  
  We analyze Taylor Swift's discography over time and track her song releases year by year.

- **How do different audio features like 'Loudness' and 'Energy' relate to one another?**  
  We create visualizations to explore the correlation between features such as loudness and energy across her songs.

- **Are Taylor Swift's songs generally more positive or more negative?**  
  We perform sentiment analysis to assess whether her songs lean towards a positive or negative emotional tone.

- **Which Taylor Swift album has the most songs in a minor key?**  
  We analyze the keys of her songs to identify which album has the highest number of songs in a minor key.

- **Collaborative vs. Solo Songs**:  
  Taylor Swift has collaborated with artists on songs like *"Snow On The Beach (Ft. Lana Del Rey)"* and *"Fortnight (Ft. Post Malone)"*. This visualization compares the average values of **Explicit**, **Danceability**, and **Acousticness** for collaborative versus solo songs using an overlaid vertical bar chart, highlighting the differences in these key features.

These visualizations provide insights into Taylor Swift's musical style, emotional tone, and the evolution of her discography.

## Song Recommender 🎧

The **Song Recommender** system allows you to find similar songs from Taylor Swift’s catalog based on audio features. This component lets users select a song and receive recommendations for 5 similar songs that match the characteristics of the chosen track.


### How to Use
- **Choose a song**: Select a song from the dropdown list.
- **Recommendations**: Once a song is selected, the system will display the song you chose and play a preview of it. It will also suggest 5 similar Taylor Swift songs based on features like energy, danceability, and popularity.

  ![Alt text](TSwift/data/images/SR2.png)
- **Listen to Previews**: The recommended songs will also have their previews played through Spotify.

## Lyrics Searcher 🔍

The **Lyrics Searcher** allows you to search for specific lyrics in Taylor Swift’s songs using TF-IDF. This tool is inspired by **Shayna Kothari's Online Tool for Taylor Swift Lyrics**, which provides a powerful way to analyze and query Taylor Swift's lyrics.

### Example Usage 
- **Enter a Search Term**: Type in any word or phrase from the lyrics to search for.
- **Retrieve Results**: The system will return the songs that have the highest relevance to the search term 
- **Review Song Excerpts**: See which songs contain the search term and review the lyrics.
- 
![Alt text](TSwift/data/images/LS1.png)

## Keyword Extraction 🔑

In this component, we perform keyword extraction for each song in Taylor Swift's *Lover* album. We use the **TF-IDF** (Term Frequency-Inverse Document Frequency) method to identify the most significant words in the lyrics of each song.

### How it Works:
- **TF-IDF Calculation**: For each song's lyrics, we calculate the frequency of each word (Term Frequency) and how unique the word is across all songs (Inverse Document Frequency).
- **Word Cloud Generation**: After calculating the TF-IDF scores, we visualize the most important words for each song using a word cloud.

### How to Use
- **Select an Album**: Select a song from the dropdown list.
- **Extract Keywords**: The system will calculate the TF-IDF scores for all songs in the album and accordingly extract the top keywords for each song.
- **View Word Clouds**: A word cloud will be generated for each song, displaying the most relevant keywords based on the lyrics.

  ![Alt text](TSwift/data/images/K2.png)



