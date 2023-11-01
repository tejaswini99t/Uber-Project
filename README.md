# **Uber Data Analytics Project** 

This project is focused on performing data analytics on Uber data using various tools and technologies, including Google Cloud Platform (GCP), Python, Compute Instance, Mage Data Pipeline Tool, BigQuery, and Looker Studio.

## Dataset:

The project uses the [TLC Trip Record Data](https://www.nyc.gov/site/tlc/about/tlc-trip-record-data.page), which includes yellow and green taxi trip records. Fields captured in the dataset include pick-up and drop-off dates/times, locations, distances, fares, rate types, payment types, and passenger counts.

-   **Dataset Source:**
    -   The dataset used in the project is available [here](https://github.com/darshilparmar/uber-etl-pipeline-data-engineering-project/blob/main/data/uber_data.csv).
-   **Data Dictionary:**
    -   A detailed data dictionary can be found [here](https://www.nyc.gov/assets/tlc/downloads/pdf/data_dictionary_trip_records_yellow.pdf).

## Data Model:

![](images/Image%2011-1-23%20at%202.48%20AM.jpeg)

## Dataflow:

-   Data Upload: Raw data collected from the Uber website is initially uploaded to Google Cloud Storage. This raw data serves as the foundation for the analytics.

-   Data Preprocessing and Coding: Python scripts are used within a Jupyter Notebook to preprocess and code the raw data. This step involves data cleaning, structuring, and ensuring data quality.

-   ETL (Extract, Transform, Load): The heart of the project's data processing happens on a Google VM Compute Engine. Here, the Mage Data Pipeline Tool is deployed to perform the ETL processes, which consist of three main components:

    Extraction (Loader): Data is extracted from Google Cloud Storage using the Loader function.

    Transformation (Transformer):Data is transformed and prepared for analysis using the Transformer function.
    Loading (Exporter): Transformed data is loaded into Google BigQuery using the Exporter function. The code for these functions can be found in the \`Mage_Code\` directory of this repository.

-   Data Storage and Querying:The processed data is stored in Google BigQuery, allowing for efficient data storage and querying capabilities. A SQL query is utilized to generate a structured table for further analytics.

-   Data Analytics and Visualization: Looker Studio is employed to build a dashboard for data analytics. This powerful tool enables you to explore, visualize, and gain insights from the data.

## **Technology Used:**

-   Programming Language: Python
-   Google Cloud Platform (GCP):
    -   Google Storage: For storing data files.
    -   Compute Instance: For running Python scripts and other tasks.
    -   BigQuery: For data storage, querying, and analysis.
    -   Looker Studio: For data visualization and analytics.
    -   Modern Data Pipeline Tool - [Mage Data Pipeline Tool](https://www.mage.ai/): For data ingestion and processing.

## Visualization:

![](images/Untitled%202.png)

## 
