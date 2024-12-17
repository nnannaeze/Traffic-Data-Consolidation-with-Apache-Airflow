# Traffic-Data-Consolidation-with-Apache-Airflow


      /traffic-data-consolidation-airflow/
      │
      ├── /data/                    # Raw data files (CSV, TSV, fixed-width)
      │   ├── toll_data.csv
      │   ├── toll_data.tsv
      │   └── toll_data.txt
      │
      ├── /dags/                     # Airflow DAGs
      │   └── traffic_data_dag.py
      │
      ├── /logs/                     # Airflow logs
      │
      ├── /staging/                  # Staging area for processed data
      │   └── consolidated_data.csv
      │
      ├── /scripts/                  # Helper scripts (curl commands, data cleaning, etc.)
      │   └── download_data.sh
      │
      ├── README.md                  # Project overview and setup instructions
      ├── requirements.txt           # List of dependencies (Airflow, etc.)
      └── .gitignore                 # Ignore unnecessary files like logs, data, etc.


## Project Introduction

### Scenario Overview

As a data engineer at a data analytics consulting company, you have been assigned a project aimed at decongesting the national highways by analyzing road traffic data from various toll plazas. Each toll plaza is operated by a different toll operator, and each operator has a distinct IT setup, using different file formats (CSV, TSV, and fixed-width) to store the traffic data. The challenge is to collect this data from the various toll operators, consolidate it into a single, unified file, and prepare it for further analysis.

### Project Objectives

The objective of this project is to develop an Apache Airflow DAG that will:
- **Extract** road traffic data from different file formats (CSV, TSV, and fixed-width).
- **Transform** the data to ensure consistency, applying necessary data cleaning and formatting.
- **Load** the transformed data into a staging area, where it can be analyzed for traffic patterns and used to support decisions related to highway decongestion.

This project showcases the ability to handle data from multiple sources, automate ETL processes using Airflow, and ensure that the data is ready for analysis by consolidating it into a single, consistent format.

## Tools and Technologies  

This section highlights the tools and technologies I used, explaining my hands-on actions for clarity and showcasing my proficiency.  

### Apache Kafka  
- I downloaded and installed Kafka in my WSL Ubuntu environment.  
- I configured Kafka to run in KRaft mode (without Zookeeper).  
- I started the Kafka broker and tested its setup to ensure functionality.  
- I used Python scripts with the `kafka-python` library to produce and consume messages.  

### Python  
- I wrote Python scripts for data extraction, transformation, and loading (ETL) processes.  
- I integrated Python with tools like Kafka for real-time data streaming.  
- I used libraries such as `pandas` for data manipulation and `matplotlib` for visualization.  

### WSL (Windows Subsystem for Linux)  
- I set up WSL to create a seamless Linux environment on my Windows system.  
- I used WSL for running Bash scripts, Kafka, and other Linux-based tools.  
- I navigated and managed file systems within WSL for better compatibility with my tools.  

### Bash Scripting  
- I wrote Bash scripts to automate repetitive tasks like starting Kafka services and managing logs.  
- I used Bash to monitor system performance and manage Linux configurations.  

### Directed Acyclic Graphs (DAGs)  
- I utilized DAGs to design and visualize ETL workflows.  
- I implemented DAGs using tools like Apache Airflow to orchestrate tasks efficiently.

- 

