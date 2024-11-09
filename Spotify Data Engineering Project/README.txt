Project Overview

This project, "Spotify Data Engineering Pipeline," showcases a structured approach to data ingestion, transformation, cataloging, querying, and visualization, all powered by AWS. With the Spotify 2023 dataset, I’ve built a robust ETL pipeline that takes raw data through a series of stages to derive valuable insights that can support decision-making.

Solution Architecture

Here’s the architecture I designed for the project:
Staging Layer: Raw data files are stored in Amazon S3.
ETL Pipeline: I used AWS Glue to build a pipeline that extracts, transforms, and loads (ETL) the data from the staging layer to a structured data warehouse.
Data Cataloging: AWS Glue Crawler scans and catalogs the data, creating tables within a database.
Querying and Analysis: Amazon Athena enables querying of cataloged data.
Data Visualization: AWS QuickSight visualizations help uncover insights from the dataset.

Dataset Description

The project uses Spotify’s 2023 dataset, consisting of five CSV files, which I preprocessed into three main files:
Spotify Albums: Includes details like album name, artist names, and release dates.
Spotify Artists: Information on artists, including names, genres, and follower counts.
Spotify Tracks: Track-level information such as track ID, popularity score, and streaming metrics.
Each file captures different aspects of Spotify’s extensive music catalog, providing data on audio features, track popularity, and more.

AWS Services Used

This project utilizes several AWS services to build a scalable pipeline:
Amazon S3: Storing both raw and processed data.
AWS Glue: ETL service to transform and load data into a structured format.
AWS Glue Crawler: Scans data, creating tables for easy querying.
Amazon Athena: Provides SQL querying capabilities over the cataloged data.
Amazon QuickSight: Used for data visualization and creating insightful reports.

Project Workflow
Data Ingestion: Raw data files are ingested into the staging layer on Amazon S3.
ETL Processing: AWS Glue transforms and loads data into the data warehouse.
Data Cataloging: AWS Glue Crawler catalogs data, creating a database and tables.
Data Querying: Amazon Athena queries the cataloged tables for analysis.
Visualization: AWS QuickSight visualizations display insights on artist popularity, album performance, and feature trends.
