# README: Spark SQL Data Analysis

## Project Overview

In this project, I used **Apache Spark SQL** to analyze home sales data. The goal was to read the data, perform SQL queries, and extract useful insights about the homes, such as their average prices based on different features (e.g., number of bedrooms, view rating). I also explored performance optimization techniques like **caching** to speed up queries.

## Key Concepts

- **Apache Spark**: An open-source framework for processing large datasets quickly. It is designed for distributed computing and can handle massive amounts of data.
- **SQL**: A programming language used for managing and querying data in relational databases. Here, SQL is used to analyze the data stored in Spark.
- **DataFrame**: A distributed collection of data organized into named columns, similar to a table in a database. Spark DataFrames are used to store and process data.
- **Parquet**: A columnar file format optimized for storing large amounts of data. It's efficient for reading and writing large datasets in Spark.
- **Caching**: Storing data in memory to make queries faster. By caching the data, Spark doesn’t need to read it from disk multiple times, improving performance for repeated queries.

## Key Insights

The project focused on several SQL queries that calculated the **average price of homes** based on specific criteria such as:

- Average home price by the number of bedrooms.
- Average home price by "view" rating, filtering for homes with an average price of at least $350,000.
- Average home price for homes built in specific years.

I also compared query performance by running the same queries once on uncached data and once on cached data. Caching the data in memory allowed Spark to run the queries much faster by reducing the need to repeatedly access data stored on disk.

## Results & Performance

- **Caching** significantly improved the performance of the queries. After caching the data, subsequent queries ran faster, as the data was stored in memory.
- I observed a noticeable difference in execution time between uncached and cached queries, which highlights the power of caching in optimizing data processing tasks in Spark.

## Conclusion

This project demonstrated how Spark SQL can be used to analyze large datasets efficiently using SQL queries. I learned how to load data, create temporary tables, perform complex queries, and optimize query performance with caching. This workflow is essential for working with large-scale data and making data analysis faster and more efficient.

