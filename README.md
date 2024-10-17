# Airline Share Price Analysis

This project is part of a coursework assignment aimed at analyzing the historical share price performance of four airline companies: **British Airways (IAG)**, **EasyJet (EZJ)**, **Jet2 (JET2)**, and **Lufthansa (0H4A)**. The goal is to combine, clean, and visualize the data in a reusable and scalable way.

## Project Overview

This project is divided into several tasks, which are completed using **Python** and the **pandas** library to handle data manipulation, and **matplotlib** for data visualization. The goal is to create a reusable codebase that can handle similar datasets with minimal modifications.

### Task Breakdown

1. **Import and Combine Data**:
   - All four airline datasets are imported, and the share price data is combined into a single **pandas DataFrame**.
   - The combined dataset includes three columns: the company identifier, date, and price.
   - This step ensures that the combined dataset is clean and standardized for further analysis.

2. **Time Series Plot of Raw Data**:
   - A time series plot is generated to visualize the raw share price data for each airline company over the available time period.
   - A separate line is used for each airline to facilitate comparison.

3. **Handle Missing Data**:
   - Upon examining the raw data, some gaps are observed in the data for one of the airlines.
   - The dataset is filtered to include only the periods where data for all airlines is available, ensuring a consistent time series comparison.
   - A new time series plot is created using this cleaned dataset.

4. **Proportional Change Visualization**:
   - To compare the **relative performance** of each airline’s share price over time, we normalize the share prices. This is done by setting the price at the start of the period to **100%** and calculating the relative price changes thereafter.
   - This visualization allows for an intuitive comparison of how each airline's stock has risen or fallen relative to its starting point, regardless of their initial share prices.

## Code Highlights

- **Modularity**: The code is designed to be reusable. It can handle similar datasets by simply changing the file paths or filenames, without needing extensive modifications.
- **Data Cleaning**: Missing data is handled efficiently by ensuring all datasets are aligned to the same time frame for comparative analysis.
- **Visualization**: Multiple time series plots are generated to compare the raw and normalized data, making it easy to spot trends and performance differences.

## Technologies Used

- **Python**: The entire project is implemented in Python.
- **pandas**: For data manipulation, cleaning, and merging of datasets.
- **matplotlib**: For creating visualizations such as time series plots.
- **Jupyter Notebook**: Used for developing and testing the code interactively.

## How to Run the Project

1. Install the required libraries if you haven't already:
   ```bash
   pip install pandas matplotlib
   ```

2. Open the Jupyter Notebook file (`shares_hgwc71.ipynb`) and execute the cells step by step to import the data, combine it, clean it, and create the visualizations.

3. You can also modify the file paths or replace the airline datasets with other company stock data to reuse the analysis pipeline for different data.

## Future Improvements

- Implement **interactive visualizations** using libraries like `plotly` to allow users to zoom in and out of specific periods.
- Add **automated reporting** to generate summaries of the share price trends and key statistics (e.g., mean, median, volatility).
- Explore **advanced data imputation techniques** to fill missing data points, rather than discarding incomplete time periods.

## Acknowledgments

This project was completed as part of the Introduction to Business Analytics course, and the datasets were provided for educational purposes.
