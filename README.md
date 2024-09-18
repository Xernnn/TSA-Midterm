# Predict HPG and MWG Stock Prices using ARIMA, LSTM, and GRU model
**Time Series Data and Analysis Course Final Project**

For a detailed analysis and complete data, please refer to the [final report](Report.pdf).

---

**Lecturer:** Prof. Trinh Tuan Phong

### Group 5 Members:
- BI12-389 Nguyen Son
- BI12-447 An Minh Tri
- BI12-375 Nguyen Cong Quoc
- BI12-357 Nguyen Duc Phuong
- BI12-390 Vu Hung Son

**ICT Department - Academic Year 3 - University of Science and Technology of Hanoi**

---

## Overview
This project focuses on predicting the stock prices of two companies: HPG (Hoa Phat Group) and MWG (Mobile World Investment Corporation) over a period from January 2, 2018, to March 31, 2023. We employ three different models—ARIMA, LSTM, and GRU—to analyze and forecast stock prices, comparing their performance based on metrics such as R-squared, MAPE, and RMSE.

## Objectives
- Build predictive models using ARIMA, LSTM, and GRU.
- Compare the performance of these models for stock price forecasting.
- Analyze and visualize stock price trends and volatility.

## Methodology
1. **Data Collection**: Stock price data for HPG and MWG was collected and analyzed.
2. **Descriptive Statistics**: Basic statistics were computed to summarize the data.
3. **Data Visualization**: Time series plots and percentage changes were visualized to observe trends.
4. **Model Implementation**:
   - **ARIMA**: Used for traditional time series forecasting.
   - **LSTM**: Implemented to capture temporal dependencies in complex data.
   - **GRU**: Similar to LSTM but with fewer parameters, providing efficient computation.

## Results
- **ARIMA**: Struggled to capture trends, resulting in flat predictions with poor metrics.
- **LSTM**: Showed significant improvement in capturing trends and volatility, yielding better predictive accuracy.
- **GRU**: Performed comparably to LSTM, effectively handling the complexities of stock price data.

### Performance Comparison
| Model      | Dataset | R-squared       | MAPE    | RMSE       |
|------------|---------|-----------------|---------|------------|
| ARIMA      | HPG     | -4.82           | 76.84%  | 15,308.11  |
| ARIMA (Test)| HPG   | 0.99            | 2.13%   | 594.48     |
| LSTM       | HPG     | 0.99            | 2.88%   | 769.52     |
| GRU        | HPG     | 0.98            | 3.22%   | 858.24     |
| ARIMA      | MWG     | -0.53           | 27.87%  | 16,399.79  |
| ARIMA (Test)| MWG   | 0.99            | 1.94%   | 1,584.73   |
| LSTM       | MWG     | 0.90            | 5.97%   | 4,201.82   |
| GRU        | MWG     | 0.99            | 1.98%   | 1,596.51   |

## Conclusion
The LSTM model outperformed both ARIMA and GRU in predicting stock prices for HPG and MWG. It effectively captured the temporal patterns and volatility inherent in the stock price data, making it a robust choice for stock price forecasting.
