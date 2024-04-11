
# Myntra Product Catalog Search Application (elastic-search-and-BERT-vector-embedding)

## Project Overview
This project implements a search application for the Myntra products catalog. It utilizes Elasticsearch to index product data from a CSV file and provides a Python Flask application for querying this data.

### Components
- `indexData.ipynb`: Jupyter Notebook for processing and loading data into Elasticsearch.
- `indexMapping.py`: Python script to define Elasticsearch index settings and mappings.
- `myntra_products_catalog.csv`: The dataset containing Myntra product details.
- `searchApp.py`: Python Flask application for querying the indexed data.

## Prerequisites
- Python 3.8 or higher
- Elasticsearch 7.x or higher
- Flask
- Jupyter Notebook or JupyterLab
- Python libraries: `pandas`, `elasticsearch`, `flask`

## Installation Guide

### Step 1: Install Elasticsearch
1. Download Elasticsearch from the [Elasticsearch official website](https://www.elastic.co/downloads/elasticsearch).
2. Follow the platform-specific installation instructions.

### Step 2: Install Python and Dependencies
1. Ensure Python 3.8 or higher is installed on your machine.
2. Install required Python libraries:
   ```bash
   pip install pandas elasticsearch flask jupyter
### Step 4: Load Data into Elasticsearch
1. Open indexData.ipynb in Jupyter Notebook or JupyterLab.
2. Execute the notebook cells to process and load data from myntra_products_catalog.csv into the Elasticsearch index. This involves:
- Reading the CSV file into a pandas DataFrame.
- Cleaning and preprocessing the data (if necessary).
- Using the Elasticsearch Python client to index data.
- Ensure that your Elasticsearch service is running during this process, as the notebook 
  interacts directly with your Elasticsearch instance.
### Step 5: Start the Flask Application
- Run searchApp.py to start the Flask web application. This script sets up a web server that hosts your search interface:
  ```bash
  python searchApp.py
- Ensure all previous steps have been successfully completed and that your Elasticsearch index contains the data.

### Step 6: Access the Web Application
  - Open a web browser and navigate to http://localhost:5000 to use the search interface.
  - Start searching through the Myntra product catalog using the provided search bar.

### Usage
After setting up the application and starting the Flask server, use the web interface to query the product catalog. The search functionality lets you query products by keywords, categories, or other indexed attributes.
