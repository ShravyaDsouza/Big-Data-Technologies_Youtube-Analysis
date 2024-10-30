
# YouTube Analysis on Hadoop Ecosystem

## Project Overview
This project focuses on analyzing YouTube video data using Hadoop's ecosystem tools. The project leverages various components such as HDFS, HBase, Hive, Pig, Apache Spark, and Zookeeper to handle large-scale data processing and analysis. The project is designed to handle complex queries and large datasets effectively, ensuring scalability and efficiency.

## Components Used
- **HDFS & HBase**: Used for distributed storage of the YouTube dataset.
- **Apache Spark**: Handles data cleaning, transformation, and analysis of complex queries stored in HDFS and HBase.
- **Hive & Pig**: Utilized for query analysis.
- **Zookeeper**: Provides distributed coordination across Hadoop components.
- **Zeppelin** (Planned): For data visualization.
- **Oozie** (Planned): For workflow automation.

## Dataset

The dataset used in this project can be found at [this link](https://netsg.cs.sfu.ca/youtubedata/).

### Dataset Attributes:
- **video ID**: An 11-digit string, which is unique.
- **uploader**: A string of the video uploader's username.
- **age**: An integer number representing the days between the date when the video was uploaded and February 15, 2007 (YouTube's establishment date).
- **category**: A string of the video category chosen by the uploader.
- **length**: An integer representing the video length (in seconds).
- **views**: An integer representing the number of views.
- **rate**: A float representing the video rating.
- **ratings**: An integer representing the number of ratings.
- **comments**: An integer representing the number of comments.
- **related IDs**: Up to 20 strings of related video IDs.

### Queries Included
1. Top 10 Most Viewed Videos
2. Average Rating by Category
3. Videos with Ratings Greater Than 4.5
4. Average Views per Category
5. Top 5 Uploaders by Number of Videos
6. Top 5 Longest Videos
7. Total Comments Count by Category
8. Total Number of Videos by Each Uploader
9. Average Video Length by Category
10. Videos with High Views but Low Ratings
11. Relationship Between Video Length and Views

## Project Structure


## Setup and Usage

### 1. Prerequisites
Ensure that the following Hadoop components are installed and configured:
- **HDFS**
- **HBase**
- **Apache Spark**
- **Hive**
- **Pig**
- **Zookeeper**

## Future Work
In the future, the project will include:
- **Apache Oozie**: To automate the execution of Spark, Hive, and Pig jobs via workflow automation.
- **Apache Zeppelin**: To provide interactive data visualization for easier analysis and insight sharing.

## Contributing
If you'd like to contribute to this project, please fork the repository and submit a pull request.

