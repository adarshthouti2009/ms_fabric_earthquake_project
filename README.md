# Microsoft Fabric Earthquake Data Engineering Project

## Project Overview
This project is designed to guide you through building a complete data engineering and analytics pipeline using Microsoft Fabric’s capabilities. You will learn how to efficiently ingest, process, transform, and visualize earthquake data sourced from the United States Geological Survey (USGS) API.

By leveraging Microsoft Fabric’s Data Factory, Data Engineering, and Power BI, you will create a structured Bronze-Silver-Gold data processing pipeline. This ensures raw data is transformed into high-quality datasets suitable for analysis, reporting, and business intelligence.

## Key Learning Objectives

  * Understand data lake architecture and how to manage structured and unstructured data efficiently.
  * Utilize Microsoft Fabric’s Data Factory to automate data ingestion from external sources.
  * Implement PySpark and Python in Fabric Data Engineering for large-scale data processing and transformation.
  * Develop incremental data processing strategies to optimize data refresh and avoid redundant computations.
  * Create interactive Power BI dashboards to visualize and analyze earthquake trends globally.

## Technologies & Tools Used

  * Python & PySpark – Data processing, transformation, and analysis.
  * Microsoft Fabric Data Factory – Automating ingestion from the USGS API.
  * Microsoft Fabric Data Engineering (Spark Notebooks) – Processing raw data and transforming it into structured datasets.
  * Microsoft Fabric OneLake (Delta Tables) – Storing structured data for efficient querying.
  * Power BI – Creating analytical dashboards for insights and reporting.

## Project Implementation Details 

### Step 1: Data Ingestion (Bronze Layer Processing)

  * Fetch earthquake event data from the USGS API in near real-time.
  * Store the raw data in the Fabric Data Lakehouse in its original format (JSON/Parquet).
  * Maintain historical records for future reference and replaying transformations.

### Step 2: Data Cleansing & Transformation (Silver Layer Processing)

  * Convert raw JSON data into structured Delta tables for improved querying.
  * Clean, normalize, and standardize key attributes (e.g., timestamps, magnitude types, and location descriptions).
  * Handle missing values and filter out redundant records.
  * Enhance data with calculated fields (e.g., magnitude category classification).

### Step 3: Business-Ready Data (Gold Layer Processing) 

  * Aggregate and refine earthquake event data into meaningful insights.
  * Optimize for query performance and Power BI reporting.
  * Create summary tables for trends, regional analysis, and risk assessments.
  * Implement incremental data updates to improve processing efficiency.

## Data Schema & Attribute Definitions

| Column Name       | Data Type | Description                                              |
| ----------------- | --------- | -------------------------------------------------------- |
| id                | String    | Unique identifier for each earthquake event.             |
| latitude          | Double    | Latitude coordinate of the earthquake event.             |
| longitude         | Double    | Longitude coordinate of the earthquake event.            |
| elevation         | Double    | Elevation at which the event occurred (in meters).       |
| title	String      | String    | Title or descriptive name of the earthquake event.       |
| place_description | String    | Detailed description of the earthquake’s location.       |
| sig               | BigInt    | Significance score of the event (based on USGS scoring). |
| mag               | Double    | Magnitude of the earthquake (Richter scale).             |
| magType           | String    | Type of magnitude scale used (e.g., Mw, ML, Ms).         |
| time              | Timestamp | Exact time when the earthquake occurred.                 |
| updated           | Timestamp | Last update time for the event data.                     |

## Project Outcomes & Insights
  By the end of this project, you will have:
    * A structured data pipeline that ingests, processes, and refines earthquake data in near real-time.
    * A well-organized Fabric Data Lakehouse with efficient data storage and retrieval.
    * A fully functional Power BI dashboard showcasing:
      * Earthquake frequency trends over time.
      * Geographic distribution of earthquake occurrences.
      * Insights into high-risk regions based on historical data.
      * Interactive filtering and drill-down analysis for better decision-making.

## Prerequisites

Before starting this project, ensure you have the following:
  * Microsoft Fabric Account (with necessary permissions).
  * Fabric Administrator access or approval from an admin.
  * Basic understanding of Python, Spark, and data engineering concepts.
  * Familiarity with Power BI for creating reports and visualizations.
		
## Conclusion

This project is ideal for data engineers, analysts, and Power BI developers looking to build an end-to-end data pipeline in Microsoft Fabric while gaining hands-on experience with big data processing, data lakes, and real-time analytics.

		
		
	  
		
		
		
		
		
		


