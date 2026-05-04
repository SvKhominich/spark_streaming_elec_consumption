# Streaming ETL for Energy Consumption and Household Segmentation in Zurich

## Project overview
In this notebook, I build a **Structured Streaming pipeline in PySpark** using the **HEAPO dataset**.  
I combine:
- **smart-meter time-series data**
- **household metadata**
- **weather data**

and write the enriched result to parquet for later SQL analysis.

## About the HEAPO dataset
The HEAPO dataset is a residential energy dataset that connects **household electricity measurements** with **building and resident characteristics** and **weather context**.  
It is well suited for questions such as:
- how energy usage changes with household size,
- how weather conditions influence consumption,
- and how building characteristics help explain demand patterns.

## What I do in this notebook
I use Spark to:
1. load the HEAPO parquet files,
2. prepare smart-meter and weather inputs,
3. enrich the smart-meter stream with static metadata,
4. join the stream with weather observations,
5. write the final output to parquet,
6. and answer a few analytical SQL questions on top of the result.


