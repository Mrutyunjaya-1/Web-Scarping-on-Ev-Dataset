🚗 Electric Vehicle (EV) Market Analysis: A Data Pipeline Project

Project Overview

This project implements a full data science pipeline, starting with Web Scraping to consolidate fragmented data from the global Electric Vehicle (EV) market. The primary goal was to create a single, clean, and structured dataset for deep Exploratory Data Analysis (EDA), allowing for robust insights into core market trends, performance trade-offs, and competitive positioning among manufacturers.

Data Source: EV database websites (Simulated data collected via Python)
Outcome: A clean dataset used for data-driven insights, suitable for consumer and industry research.

🛠️ Technical Stack and Methodology

This project showcases expertise across the entire data pipeline:

1. Data Extraction (Web Scraping)

Libraries: Requests (for fetching HTML content) and BeautifulSoup (for parsing).

Technique: Implemented a recursive scraping mechanism to iterate over multiple pages, ensuring comprehensive data collection.

Key Skill: Extensive use of Regular Expressions (Regex) to reliably extract numeric values (Price, Range, Battery size) from text fields containing units and symbols (e.g., converting "450 km" to 450).

2. Data Cleaning & Preparation

Libraries: Pandas and NumPy.

Processes:

Data Standardization: Removed unit suffixes ('km', 'kWh', 'kg') and converted feature columns to appropriate numeric data types.

Imputation & Validation: Handled all missing values using mode imputation or strategic data inference.

Integrity Check: Confirmed zero missing values and zero duplicate rows after cleaning.

3. Exploratory Data Analysis (EDA)

Libraries: Seaborn and Matplotlib.

Visualization Focus: Correlation heatmaps, distribution histograms, and targeted scatter plots to reveal complex engineering trade-offs.

🔑 Key Analytical Insights

The analysis of the cleaned EV dataset provided clear answers to critical market questions:

Core Performance Correlation (r > 0.89): A highly positive correlation was established between Battery Capacity and Real-World Range, confirming battery size as the single greatest factor in vehicle range.

Market Trade-offs: The analysis revealed the strong negative correlation between Vehicle Weight and Energy Efficiency, highlighting the primary engineering challenge in EV design.

Competitive Advantage: Identified efficiency leaders (e.g., Tesla, BMW, BYD) who achieve superior range compared to competitors at equivalent vehicle weights.

Market Standard: Determined that the current industry standard centers around a 60-80 kWh battery and a 300-500 km range for most mainstream models.

⚙️ Repository and Setup

The repository is structured to reflect the project's flow:

├── 01_scraping_code/         # Contains the core Python scraping script
├── 02_notebooks/             # Contains the Jupyter Notebook for all Cleaning and EDA
├── data/                     # Contains the final cleaned dataset (`clean_ev_dataset.csv`)
├── visualizations/           # Contains all presentation-ready charts and plots
└── README.md                 # This file


Execution Instructions

Clone the repository.

Install Dependencies: pip install pandas numpy matplotlib seaborn beautifulsoup4 requests

Run Analysis: Execute the steps within the 02_notebooks/EV_Data_Analysis_and_Cleaning.ipynb file to replicate all cleaning, analysis, and visualization results.

👤 Contributor

[Mrutyunjaya Debata] - Data Extraction, Cleaning, and Visualization
