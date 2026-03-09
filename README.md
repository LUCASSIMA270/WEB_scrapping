# Web-scrapping-Python

🌐 FC_LEA: Election Web Scraping Project
Extraction, Cleaning, and Analysis of Political Polls (Denmark & Czech Republic)

This repository contains the complete Web Scraping pipeline developed to collect, process, and standardize opinion poll data from Wikipedia. The project focuses on the electoral cycles of Denmark (2015, 2019, 2022) and the Czech Republic, transforming raw HTML data into structured datasets for statistical analysis.
🧐 Project Objective

The goal is to build a robust database that allows for comparing voting intentions (polls) with official election results. The script automates the retrieval of complex tables from Wikipedia, manages formatting variations across countries and years, and classifies parties according to their political orientation.
🛠️ Toolkit (Technical Stack)

The project is entirely developed in Python within a Jupyter Notebook environment, utilizing the following libraries:

    Extraction: requests and BeautifulSoup (bs4) for HTML parsing.

    Data Processing: pandas for DataFrame manipulation and re (Regex) for standardizing dates and party names.

    Visualization: matplotlib for plotting electoral trends.

    Output: openpyxl for generating standardized multi-sheet Excel files.

📂 Repository Contents

    FC_LEA_FINAL.ipynb: The main notebook containing the source code, from the initial HTTP request to the final export.

    PROJECT GUIDELINES.pdf: Academic directives and technical specifications for the project.

    election_data/: (Generated folder) Contains the produced Excel files (e.g., Denmark_2022_general.xlsx), categorized by country and year.

📈 Methodology & Technical Challenges

The script follows a rigorous workflow to ensure data quality:

    Dynamic Parsing: Automatic identification of relevant columns (polling_firm, sample_size, date) despite changing table structures.

    Time Standardization: Conversion of heterogeneous date formats (e.g., "2-5 May") into ISO format (YYYY-MM-DD).

    Political Mapping: Automatic assignment of orientation (Left, Right, Center) to each party via a mapping dictionary.

    Outlier Handling: Cleaning special characters and converting text strings into floating-point numerical values.

🚀 Results & Outputs

The project generates Excel files ready for econometric analysis, including:

    Polling firm name and sample size.

    Predicted score for each party vs. its actual final result.

    Political orientation to facilitate group analysis by blocs.
