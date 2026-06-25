# Spotify Streaming & Audio Trends Dashboard 🎧📊

A comprehensive Power BI data analytics solution designed to clean, model, and visualize streaming metrics and acoustic features from thousands of tracks. This project transforms raw music data into actionable business intelligence using a sleek, brand-aligned custom theme.

## 📥 Data Source
* **Source:** The underlying dataset used for this analysis was sourced from **Kaggle**. 

## 🚀 Key Visualizations & Insights
* **Sum of Popularity by Artists:** Clear identification of top-performing global artists across the catalog.
* **Acoustic Feature Mapping:** Dynamic tracking of physical music attributes (Danceability vs. Energy levels) across varying music genres.
* **Content Proportions:** A segmented breakdown of explicit vs. non-explicit track distributions.
* **High-Level KPIs:** Instant tracking of metrics across total tracks, average global popularity, and average track energy.

## 🛠️ Backend Architecture & Engineering
The underlying infrastructure of this dashboard relies on careful data modeling and engineering principles:

### 1. Data Cleaning & ETL (Power Query)
* **Data Cleansing:** Handled data type normalization, structured data schemas, and eliminated blank records from the source file.
* **Feature Typing:** Scaled numeric features (Danceability, Energy, and Popularity) into explicit numerical values for responsive cross-filtering.

### 2. Data Model
* **Schema Layout:** Built using a flat, high-performance schema structure optimized for instant data row retrieval and filtering.

### 3. DAX Measures & Logic
The core metrics on the dashboard are driven by dynamic Data Analysis Expressions (DAX), including:

* **Total Track Footprint:** 
  `Total Tracks = COUNTROWS('cleaned_spotify_data')`
* **Baseline Popularity:** 
  `Average Popularity = AVERAGE('cleaned_spotify_data'[popularity])`
* **Energy Aggregation:** 
  `Average Energy = AVERAGE('cleaned_spotify_data'[energy])`

## 🎨 UI/UX Design & Branding
* **Theme Customization:** Shifted away from standard templates to engineer a custom "Spotify Dark Mode" aesthetic, providing high-contrast visual clarity.
* **Scannability:** Strategic positioning of key analytical metrics at the baseline layer, ensuring a clean visual hierarchy.

## 📁 Repository Structure
* `/Dashboard`: Contains the finalized `.pbix` Power BI workspace file.
* `/Data`: Houses the raw/cleaned data assets.
* `/Image`: Stores UI mockups and dashboard screenshots.
* `/Notebook`: Contains tracking scratchpads and initial exploration files.
