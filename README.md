# Project Title

A brief description of what this project does and who it's for.

## Table of Contents

- [Installation](#installation)
- [Data Setup](#data)
- [Data Ingestion](#ingestion)
- [Analysis](#analysis)
- [Visualization](#visualization)
- [License](#license)
- [Acknowledgments](#acknowledgments)

## Installation

Instructions on how to install and set up the project.

```bash
# Clone the repository
git clone https://github.com/svukomanovic/Amazon-Sentiment-Analysis.git

# Navigate to the project directory
cd Amazon-Sentiment-Analysis

## Data Setup

#To download data navigate to 
From the link: https://amazon-reviews-2023.github.io/
Download a [review] data set and [meta] dataset, to replicate our research datasets download:
1. Appliances
2. Amazon Fashion
3. Pet Supplies
4. Toys and Games

## Data Ingestion (data-ingestion.ipynb)

1. With Jupyter notebooks opne the data-ingestion.ipynb notebook

2. If you are on a Windows machine, run the first stage it will open a GUI prompt to load the data.  
   - Review Data Input: 
   -- Appliances.jsonl 
   -- Toys_and_Games.jsonl
   -- Pet_Supplies.jsonl
   -- Amazon_Fashion.jsonl
   
3. If you are on a Mac machine, skip the first step for windows, and run the second step for Mac and just hardcode the file name that you want to input

4. Repeat the same with Step 2 Windows and Mac but instead of the review data, import the metadata files
   - Metadata Data Input:
   -- meta_Appliances.jsonl
   -- meta_Pat_Supplies.jsonl
   -- meta_Toys_and_Games.jsonl
   -- meta_Amazon_Fashion.jsonl
   
5. Last stage of the data-ingestion.ipynb generates a csv file, with Windows you can select the file name, with Mac.  For ease of use we suggest using the following name examples:
 -- appliances_2022.csv
 -- pet_supplies_2022.csv
 -- toys_and_games_year_2022.csv
 -- amazon_fashion_2022.csv

## Sentiment Analysis (Amazon-analysis.ipynb)
1. If you changed the name of the csv file, then update the Amazon-analysis.ipynb for MAC version
2. Run the first stage with Windows and select the appliances_2022.csv file
3. For Mac just skip the first step with windows, and load the appliances_2022.csv
4. Run the rest of the stages to create the dataset, and generate a violin chart to compare the accuracy of the data
5. You can update the file name now to another CSV if you want to validate the data for any other data set.

## Visualization Month by Month analysis (month-by-month-analysis.ipynb)
1. Start with windows and or the MAC stage and load the appliances_2022.csv
2. you can run the other stages that will process the data and then generate the visualization for the year.
3. You can run the other stages if you labeled the files the same way as the data ingestion steps 2,4, and 5 that will generate the visualization for the other files.  Note this can take some time (3-4hrs)