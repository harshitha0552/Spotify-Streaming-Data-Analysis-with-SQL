# Spotify-Streaming-Data-Analysis-with-SQL
Project Category: Advanced
[Click Here to get Dataset](https://www.kaggle.com/datasets/sanjanchaudhari/spotify-dataset)

## Overview
This project showcases exploratory data analysis (EDA) and advanced SQL querying using a real-world-style Spotify dataset. The goal is to derive meaningful insights related to tracks, artists, albums, and user engagement using standard queries of varying complexity (easy, medium, and advanced).

```sql
-- create table
CREATE TABLE spotify (
    artist VARCHAR(255),
    track VARCHAR(255),
    album VARCHAR(255),
    album_type VARCHAR(50),
    danceability FLOAT,
    energy FLOAT,
    loudness FLOAT,
    speechiness FLOAT,
    acousticness FLOAT,
    instrumentalness FLOAT,
    liveness FLOAT,
    valence FLOAT,
    tempo FLOAT,
    duration_min FLOAT,
    title VARCHAR(255),
    channel VARCHAR(255),
    views FLOAT,
    likes BIGINT,
    comments BIGINT,
    licensed BOOLEAN,
    official_video BOOLEAN,
    stream BIGINT,
    energy_liveness FLOAT,
    most_played_on VARCHAR(50)
);
```
## Project Steps

### 1. Data Exploration
Before diving into SQL, it’s important to understand the dataset thoroughly. The dataset contains attributes such as:
- `Artist`: The performer of the track.
- `Track`: The name of the song.
- `Album`: The album to which the track belongs.
- `Album_type`: The type of album (e.g., single or album).
- Various metrics such as `danceability`, `energy`, `loudness`, `tempo`, and more.
  
### 2. Data Cleaning and Normalization
 Ensure consistent data types and handle missing values appropriately.
 
### 3. Creating the Table
Used `CREATE TABLE` with relevant datatypes and constraints as shown above.
   
### 4. Querying the Data
Queries were categorized into Easy, Medium, and Advanced based on complexity.
 
### 4. Querying the Data
After the data is inserted, various SQL queries can be written to explore and analyze the data.

#### Easy Queries
- Simple data retrieval, filtering, and basic aggregations.
  
#### Medium Queries
- More complex queries involving grouping, aggregation functions, and joins.
  
#### Advanced Queries
- Nested subqueries, window functions, CTEs, and performance optimization.
  
---

## 15 Practice Questions

### Easy Level
1. Retrieve the names of all tracks that have more than 1 billion streams.
2. List all albums along with their respective artists.
3. Get the total number of comments for tracks where `licensed = TRUE`.
4. Find all tracks that belong to the album type `single`.
5. Count the total number of tracks by each artist.

### Medium Level
1. Calculate the average danceability of tracks in each album.
2. Find the top 5 tracks with the highest energy values.
3. List all tracks along with their views and likes where `official_video = TRUE`.
4. For each album, calculate the total views of all associated tracks.
5. Retrieve the track names that have been streamed on Spotify more than YouTube.

### Advanced Level
1. Find the top 3 most-viewed tracks for each artist using window functions.
2. Write a query to find tracks where the liveness score is above the average.
3. Use a `WITH` clause to calculate the difference between the highest and lowest energy values for tracks in each album.
4. Find tracks where the energy-to-liveness ratio is greater than 1.2.
5. Calculate the cumulative sum of likes for tracks ordered by the number of views, using window functions.
```sql

## Technology Stack
- **Database**: PostgreSQL
- **SQL Queries**: DDL, DML, Aggregations, Joins, Subqueries, Window Functions
- **Tools**: pgAdmin 4 (or any SQL editor), PostgreSQL (via Homebrew, Docker, or direct installation)

## How to Run the Project
1. Install PostgreSQL and pgAdmin (if not already installed).
2. Set up the database schema and tables using the provided normalization structure.
3. Insert the sample data into the respective tables.
4. Execute SQL queries to solve the listed problems.
5. Explore query optimization techniques for large datasets.

## ✅ Next Steps  
- **Build Dashboards**: Visualize insights using tools like **Power BI**, **Tableau**, or **Metabase** to enhance storytelling from the SQL queries.  
- **Enhance Dataset**: Expand the dataset with additional fields (e.g., genres, listener locations) or larger volume to simulate real-world scaling.  
- **Performance Tuning**: Experiment with indexing strategies, query refactoring, and execution plans for better performance on complex queries.  
- **Data Modeling**: Normalize or restructure the schema to practice relational design principles and improve maintainability.

---

## 🤝 Contributing  
Have ideas to improve this project or want to add your own queries?  
You're welcome to **fork the repo**, open **pull requests**, or raise **issues** for discussions and collaboration.
