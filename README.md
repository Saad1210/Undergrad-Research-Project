# Undergrad-Research-Project

**Project Overview**

The objective of this project is to develop a robust framework that can identify conflicting ship trajectories using AIS data. The framework processes extensive real-world maritime data, identifies peak traffic locations and times, and applies advanced metrics to detect potential encounters, ultimately reducing computational costs and enhancing detection accuracy.

## Framework Overview
The framework developed in this project is inspired by the work of Po-Ruey Lei on mining maritime traffic conflict trajectories from massive AIS data. It involves three main steps:

1. Window-Based Encounter Identification: Grouping ship trajectories that might intersect within a specific time window.
2. Conflict Ascertainment: Detecting potential conflicts from the identified encounters.
3. Conflict Trajectory (CT) Generation: Collecting and organizing all identified conflicts chronologically to form conflict trajectories.

## Key Features
- Data Preprocessing:
    - Processed over 15 million data points from AIS data collected over 6 months, involving 4000+ ships.
    - Normalized time into 1-minute intervals and discretized space into 1x1km grids, reducing computational cost by 67%.

- Exploratory Data Analysis (EDA):
    - Conducted EDA using Geopy, Plotly, and Matplotlib to gain insights into maritime traffic patterns.
    - Identified peak traffic hours and locations, providing valuable information for maritime traffic management.

- Conflict Detection:
    - Developed an encounter detection mechanism using TCPA (Time to Closest Point of Approach) and DCPA (Distance to Closest Point of Approach) metrics.
    - Implemented detection at specific timestamps to identify potential conflicts between ship trajectories.
