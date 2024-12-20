
# YouTube Analysis on Hadoop Ecosystem

## Project Overview
This project focuses on analyzing YouTube video data using Hadoop's ecosystem tools. The project leverages various components such as HDFS, HBase, Hive, Pig, Apache Spark, and Zookeeper to handle large-scale data processing and analysis. The project is designed to handle complex queries and large datasets effectively, ensuring scalability and efficiency.

## Components Used
- **HDFS & HBase**: Used for distributed storage of the YouTube dataset.
- **Apache Spark**: Handles data cleaning, transformation, and analysis of complex queries stored in HDFS and HBase.
- **Hive & Pig**: Utilized for query analysis.
- **Zookeeper**: Provides distributed coordination across Hadoop components.
- **MongoDB**: Included as a NoSQL alternative to compare query performance and storage efficiency.
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

### Directory Overview
- **data/**: Contains the raw and processed YouTube dataset files.
- **output/**: Contains the results of queries of the year 2007.
- **notebooks/**: Jupyter notebooks used for exploratory data analysis (EDA), data visualization, and interactive analysis.
- **docs/**: Contains project documentation, including **report.pdf** with detailed analysis and descriptions.

### File Overview

- **README.md**: Provides a project overview, setup instructions, and usage guidelines.
- **requirements.txt**: Lists the required Python libraries and dependencies for running scripts and notebooks.
- **data_preparation.ipynb**: Jupyter notebook for cleaning, transforming, and loading the dataset into HDFS and HBase.
- **query_analysis.ipynb**: Jupyter notebook for running predefined analytical queries on Spark, Hive, Pig, HBase, and MongoDB.
- **visualization.ipynb**: Jupyter notebook for creating visualizations of processed data and query results.

## Data Flow Summary

1. **Data Ingestion**: Raw data is ingested into HDFS and HBase.
2. **Data Processing**: Spark handles data cleaning, transformation, and loading into the local machine, HDFS, and HBase.
3. **Query Execution**: Queries are executed through Hive, Pig, HBase, and Spark, with additional comparative analysis in MongoDB.
4. **Performance Analysis**: Execution times and query performance are measured across tools for comparison.
5. **Visualization**: Analysis results are visualized using Jupyter Notebook and libraries like Matplotlib, Seaborn, and Plotly.

## Setup and Usage

### 1. Prerequisites
Ensure that the following components are installed and configured:
- **HDFS**
- **HBase**
- **Apache Spark**
- **Hive**
- **Pig**
- **Zookeeper**
- **MongoDB**

### 2. Running the Project
- **Data Preparation**: • Load the dataset into HDFS, HBase, and MongoDB for comparison.

- **Data Processing**: 
• Use Apache Spark for data cleaning and transformation tasks, optimizing the dataset for efficient querying.
• Additional preprocessing may be conducted in HBase, Hive, and MongoDB for comparative analysis.

- **Analysis**: 
• Perform analytical queries using Hive, Pig, and MongoDB to explore data patterns, aggregations, and comparisons across different storage solutions.
• Use Spark SQL for complex queries and aggregations where required.

- **Visualization**: 
• Current: Visualizations are performed using a combination of PySpark (SparkSession, functions), Matplotlib, Seaborn, Pandas, NumPy, and Dask.
• Future (Planned): We plan to utilize Apache Zeppelin for interactive visualizations, enabling richer data exploration within the Hadoop ecosystem.

## Future Work
In the future, the project will include:
- **Apache Oozie**: To automate the execution of Spark, Hive, and Pig jobs via workflow automation.
- **Apache Zeppelin**: To provide interactive data visualization for easier analysis and insight sharing.

## Contributing
If you'd like to contribute to this project, please fork the repository and submit a pull request.