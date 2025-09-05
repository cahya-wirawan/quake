# Earthquake Data Exploration

This repository contains tools and notebooks for collecting, processing, and analyzing real-time earthquake data from the USGS (United States Geological Survey) API.

## Contents

### spark.ipynb

A comprehensive Jupyter notebook that demonstrates earthquake data collection and analysis using Apache Spark and the USGS API. This notebook provides:

**Data Collection:**
- Fetches real-time earthquake data from the USGS GeoJSON API
- Retrieves daily earthquake data (approximately 250 entries) from around the world
- Handles data from the official USGS earthquake feed

**Data Processing with Apache Spark:**
- Initializes Spark sessions for distributed data processing
- Defines robust schemas for handling nested GeoJSON earthquake data structure
- Creates Spark DataFrames for efficient large-scale data analysis
- Performs data transformations and analysis to identify strongest earthquakes
- Supports filtering by magnitude, location, and other earthquake properties

**Data Storage and Export:**
- Saves processed earthquake data in multiple formats:
  - Parquet files for efficient columnar storage
  - CSV files for easy data sharing
  - JSON files for web applications
- Creates managed Spark tables for SQL querying

**Interactive Visualization:**
- Generates interactive world maps using Folium
- Plots earthquake locations with magnitude-based markers
- Provides detailed popup information for each earthquake event
- Supports filtering and visualization of specific earthquake subsets

**Advanced Analytics:**
- Demonstrates Spark SQL queries for complex data analysis
- Filters earthquakes by magnitude thresholds (e.g., > 5.0, > 3.0)
- Searches earthquakes by geographic location keywords
- Shows time-based analysis of earthquake events

**AI-Powered Querying:**
- Integrates with Google's Gemini API for natural language processing
- Converts plain English questions into Spark SQL queries
- Enables non-technical users to explore earthquake data using natural language
- Example: "Show all earthquakes with magnitude greater than 3.0 in Indonesia"

**Key Features:**
- Real-time data from authoritative USGS sources
- Scalable processing using Apache Spark
- Interactive mapping and visualization
- Multiple export formats for data sharing
- AI-powered natural language query interface
- Comprehensive error handling and data validation

This notebook serves as both a learning resource for Spark-based data processing and a practical tool for earthquake data analysis and monitoring.
