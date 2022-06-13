# Fraudit
The following repo utilizes a companies data to determine if it's investment request is fraudulent or not.
Please note, the data itself is from a large bank in Canada and cannot be shared (even though it's been censored to not reveal the identity of the companies). 

## Data
There are two datasets: 
- Candian Companies Dataset - About 30k rows of canadian companies asking for Loans / Investments over the span of 3 years. 
- General Companies Dataset - About 28k rows of companies (outside of Canada) asking for loans / investments over the span of last 3 years. 

Due to confidentiality reasons, the raw data is not shared here. 

## Reports 

You can see some reports on the Canadian Companies Dataset and General Companies dataset here: 
- https://htmlpreview.github.io/?https://github.com/Tahir001/Fraudit/blob/main/Automatic_Analysis/Canadian_Companies_Analysis.html
- https://htmlpreview.github.io/?https://github.com/Tahir001/Fraudit/blob/main/Automatic_Analysis/General_Companies_Analysis.html

Note that the above is only a preview, if you'd like an interactive report, feel free to download the .html files inside of the Automatic Analysis folder and play around with it. 

## Repository Structure
In this repo, we breakdown our End to End modelling pipeline and use a seperate Notebook for each process.

Fraudit
├── Automatic_Analysis
│   ├── Canadian_Companies_Analysis.html
│   └── General_Companies_Analysis.html
├── Data
│   └── Top 100 Features.xlsx
├── LICENSE
├── Pictures
│   ├── Linked_lists.png
│   ├── Ratios_Used_1.png
│   └── Ratios_Used_2.png
├── README.md
└── Scripts
    ├── Archived
    ├── Data Pre-Processing & Class Imbalance Issue.ipynb
    ├── Defining Base Models & Model Metrics.ipynb
    ├── Exploratory Data Analysis & Data Cleaning.ipynb
    ├── Feature Engineering.ipynb
    ├── Feature Selection.ipynb
    ├── Hyperparameter Optimization & Final Model.ipynb
    ├── IMI CASE COMPETITION [Master Sheet].ipynb
    └── Training Machine Learning Models.ipynb

5 directories, 16 files


The Pictures Folder contains all of the screenshots we used in our presentation, and some of our visualization output.

The Automatic_Analysis folder contains the result from Pandas Profiling (Automatic EDA library)

The Code Folder contains our process which is entailed as follows: 
1. Exploratory Data Analysis
2. Data Cleaning and Pre-Processing 
3. Solving the class imbalance issue
4. Feature Engineering and Feature Selection
5. Modelling & Hyperparameter Optimization
6. Model Explaination
7. Results & Final Submission
