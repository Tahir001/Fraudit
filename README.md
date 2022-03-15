# Fraudit
The following repo utilizes a companies data to determine if it's investment request is fraudulent or not.
Please note, the data itself is from a large bank in Canada and cannot be shared (even though it's been censored to not reveal the identity of the companies). 

## Data
There are two datasets: 
- Candian Companies Dataset - About 30k rows of canadian companies asking for Loans / Investments over the span of 3 years. 
- General Companies Dataset - About 28k rows of companies (outside of Canada) asking for loans / investments over the span of last 3 years. 

## Repository Structure
In this repo, we breakdown our End to End modelling pipeline and use a seperate Notebook for each process.
The Code Folder contains our process which is entailed as follows: 
1. Exploratory Data Analysis
2. Data Cleaning and Pre-Processing 
3. Solving the class imbalance issue
4. Feature Engineering and Feature Selection
5. Modelling & Hyperparameter Optimization
6. Model Explaination
7. Results

The Pictures Folder contains all of the screenshots we used in our presentation, and some of our visualization output.

The Automatic_Analysis folder contains the result from Pandas Profiling (Automatic EDA library)

## Presentation Slides
A Rough Draft of the presentation slides can be found here: https://docs.google.com/presentation/d/1TSxYwJy-8RPQgrMXTs8Cb-ag7hUpsb4q29BoZ7dX5Z4/edit?usp=sharing
