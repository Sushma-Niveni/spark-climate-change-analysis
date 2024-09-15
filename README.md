
# Spark Climate Change Analysis

This project uses Apache Spark to analyze climate change data. It includes data on average land temperatures and CO2 emissions per capita from various countries. The analysis aims to understand temperature changes over time and the correlation between CO2 emissions and temperature changes.

## Project Structure

- **data/**: Contains raw data files.
  - `temperature_data.csv`: Average land temperature data by country from 1750 to 2015.
  - `co2_data.csv`: CO2 emissions per capita data by country from 1960 to 2014.

- **notebooks/**: Contains Jupyter notebooks for interactive analysis.
  - `climate_change_analysis.ipynb`: A notebook with exploratory analysis and visualization.

- **scripts/**: Contains PySpark scripts for data processing and analysis.
  - `temperature_analysis.py`: PySpark script to analyze temperature and CO2 emissions data.

## Setup

### 1. Install Required Software

- **Python**: Ensure Python 3.x is installed.
- **Java**: Apache Spark requires Java to run. Make sure Java 8 or later is installed.
- **Apache Spark**: Follow [Apache Spark installation instructions](https://spark.apache.org/docs/latest/) for your operating system.

### 2. Install Python Dependencies

You can use the `requirements.txt` file to install necessary Python packages.

1. Install packages using pip:
   ```sh
   pip install -r requirements.txt

### Running the Code
**Google Colab**: Use the Jupyter notebook in the notebooks/ directory for interactive analysis.
**Local PySpark**: Run the PySpark script using the following command:
spark-submit scripts/temperature_analysis.py

### Google Cloud Setup (Optional)
Create a Google Cloud Project: Google Cloud Console
Set Up a Dataproc Cluster: Follow the Dataproc Quickstart guide.
Submit a Spark Job: Use the command 
gcloud dataproc jobs submit pyspark --cluster your-cluster-name --region your-region gs://your-bucket-name/path-to-your-script.py
