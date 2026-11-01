# MovieRanker

MovieRanker is a Java application that combines movie ratings from multiple sources to generate a unified ranking of the top 250 movies of all time.

## The Problem

The problem is that the demographics and taste of people who review movies on different websites is different and creates discrepancies in the top rated movie/best movies of all time lists on the these websites. Movie Ranker aims to solve this problem by creating a weighted average of ratings of movies from multiple sources and generating list containing a better representation of the greatest movies of all time based on those ratings.


## How It Works

1. **Retrieve Movie Data From MovieLens:** Download movie information and user ratings from the MovieLens dataset.
2. **Retrieve Movie Data from TMDB:** Use the TMDB API to retrieve additional movie ratings and information.
3. **Match Movies:** Match movies between the two sources using their TMDB or IMDb identifiers.
4. **Calculate Weighted Scores:** Normalize ratings from each source and combine them using a weighted scoring system.
5. **Generate Rankings:** Sort movies by their combined scores and select the top 250.
6. **Export Results:** Save the final rankings to a CSV file.
<img width="592" height="472" alt="SystemDiagram drawio" src="https://github.com/user-attachments/assets/f3c4f068-e602-49b8-8ca7-ff4205c8b0bb" />

## Tech Stack

- **Language:** Java
- **Libraries:** Jackson (JSON parsing), `java.net.http` (HTTP requests), `java.util` (data structures), `java.io` (file input/output), `java.nio.file` (file management), `java.util.zip` (ZIP extraction)
- **External Tools:** TMDB API, MovieLens Latest Small Dataset

## Setup

Work in Progress...

## Roadmap

### MVP (Version 1.0)
- [ ] Collect movie data and ratings from the MovieLens dataset and TMDB API.
- [ ] Match movies between the two sources using IMDb and TMDB identifiers.
- [ ] Calculate a weighted average of each movie's ratings.
- [ ] Sort movies based on their combined ratings.
- [ ] Generate a unified ranking of the top 250 movies.

### Future Improvements (Version 2.0+)
- [ ] Allow users to customize the weights assigned to different rating sources.
- [ ] Integrate additional movie rating sources into the dataset.
- [ ] Develop a GUI to display movie information and posters.

## Author
Alexandr Zhdanov, https://github.com/AlexandrZhda
