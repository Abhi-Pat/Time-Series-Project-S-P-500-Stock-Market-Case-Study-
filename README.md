# Time-Series-Project-S-P-500-Stock-Market-Case-Study-# Time Series Analysis of S&P 500 Stock Market Data (Case Study)

This repository provides a comprehensive approach to analyzing and visualizing Time Series Data of S&P 500 Stocks (with a focus on major tech companies) using various data processing, analysis, and visualization techniques.

## Steps Performed:

### 1. **Data Preparation**:
   - Imported necessary libraries including `pandas`, `numpy`, `seaborn`, `matplotlib.pyplot`, `plotly.express`, `glob`, and `warnings`.
   - Loaded multiple CSV files containing stock market data, which were then concatenated into a single DataFrame using the `pandas.concat()` method.
   - This DataFrame served as the foundation for all further analysis, providing a unified view of the stock data from various files.

### 2. **Analyzed Stock Price Changes Over Time**:
   - Created a filtered version of the `tech_list` DataFrame from the larger universal DataFrame.
   - Checked for missing values and performed data type corrections to ensure consistency and accuracy.
   - Generated subplots to visualize the price changes for each stock, specifically focusing on the relationship between `date` and `close` (closing price). This helped to visualize the overall trend and fluctuations in stock prices over time.

### 3. **Calculated Moving Averages for Various Stocks**:
   - Implemented rolling windows for calculating the moving averages of stock prices over different time periods (e.g., 10 days, 20 days, 30 days).
   - Created subplots to visualize how each stock’s closing price behaves in relation to its moving average over the specified time windows (`date` vs. moving averages). This analysis is essential for understanding the smoothing of price data and the identification of trends.

### 4. **Apple Stock Price Change Analysis**:
   - Investigated how much profit or loss was made each day by calculating the difference between the opening and closing prices of Apple stock.
   - Multiplied the price change by the number of shares owned to calculate the daily monetary impact.
   - Calculated and plotted the percentage change between consecutive days to understand the stock's daily return.
   - Visualized the daily return in percentage by creating a line plot of `date` vs. "Daily Return (%)", providing insights into the performance of Apple’s stock over time.

### 5. **Resampling Analysis of Closing Prices**:
   - Ensured that the `date` column was set as the row index of the DataFrame to allow resampling of the data.
   - Performed resampling on the closing price data on various time frequencies such as monthly, quarterly, and yearly.
   - Plotted line graphs for each resampled period (monthly, quarterly, and yearly), providing a clearer view of long-term trends and changes in stock prices.

### 6. **Stock Price Correlation Analysis for Tech Companies**:
   - Focused on analyzing whether the closing prices of major tech companies (Apple, Amazon, Google, Microsoft) are correlated.
   - Used a pair plot to visualize the pairwise relationships between the closing prices of these companies. The plots were scatter plots to show the correlation and trends.
   - Created heatmaps to further explore the strength of correlations between the stocks, highlighting areas of high and low correlation.
   - Developed line graphs to visualize the correlation between the closing prices of the selected tech companies, and how these relationships change over time. Additionally, percentage changes in the closing prices were plotted against correlated data to understand the impact of these correlations.

### 7. **Daily Change in Closing Price and Daily Returns Correlation**:
   - Analyzed whether the daily changes in closing prices (or daily returns) of stocks were correlated.
   - Used Seaborn’s `PairGrid` to correlate the percentage changes in daily returns for each company, helping to identify any significant relationships between daily price movements.
   - Generated visualizations such as scatter plots, line plots, and correlation heatmaps to study the interactions and correlations between daily returns across the stocks analyzed.

---

### Features:
- Data preprocessing, cleaning, and transformation for consistent and accurate analysis.
- Use of various statistical and visual techniques (moving averages, correlation analysis, resampling) to explore stock market trends.
- Detailed analysis of price movements, daily returns, and correlations between major tech stocks.
- Interactive and informative visualizations such as pair plots, heatmaps, and line graphs to present the findings in a clear and engaging manner.

### Requirements:
- `pandas`: For data manipulation and analysis.
- `numpy`: For numerical operations.
- `seaborn`: For advanced visualizations.
- `matplotlib`: For creating static, animated, and interactive plots.
- `plotly`: For interactive visualizations (optional but useful).
- `glob`: For managing multiple file loading from directories.
- `warnings`: For handling warnings during analysis.

### How to Use:
1. Clone this repository to your local machine.
2. Install the required libraries using `pip install -r requirements.txt`.
3. Place your stock market CSV data files in the appropriate folder.
4. Run the Python scripts to perform the data analysis and generate visualizations.

This repository aims to provide an efficient and systematic approach to analyzing S&P 500 stock data, offering insightful visualizations and practical techniques for understanding stock market trends and behaviors.
