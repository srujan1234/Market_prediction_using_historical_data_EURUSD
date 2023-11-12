# Market_prediction_using_historical_data_EURUSD(Needs changes, not in order)

**Data Preprocessing for Market Direction Prediction**


This Kaggle notebook focuses on the preprocessing steps required for training a predictive model to forecast market direction (Up or Down) at various time frames using tick data.


1. **Data Loading and Transformation:**
   - Loaded tick data from a CSV file, containing essential columns like 'askPrice,' 'bidPrice,' 'askVolume,' 'bidVolume,' 'time,' 'year,' 'month,' and 'day.'
   - Converted the 'date' or timestamp columns to datetime format for time-based analysis.
   - Created additional features, such as 'year,' 'month,' and 'day,' to facilitate time-based grouping and analysis.

2. **Time Series Features and Labels:**
   - Derived time-related features such as 'year,' 'month,' and 'day' for temporal context.
   - Calculated price changes over different time intervals (3 months, 6 months, 9 months).
   - Generated labels for price direction (Up/Down) based on the calculated price changes.

3. **Volatility and Trend Duration:**
   - Calculated volatility metrics (high and low) for each time interval.
   - Determined trend duration for the given time intervals, aiding in identifying prolonged market trends.

4. **Technical Indicators:**
   - Computed technical indicators like RSI (Relative Strength Index), MACD (Moving Average Convergence Divergence), ADX (Average Directional Index), Stochastic Oscillator, MFI (Money Flow Index), ROC (Rate of Change), ULTOSC (Ultimate Oscillator), CCI (Commodity Channel Index), BOP (Balance of Power), and CMO (Chande Momentum Oscillator).
   - Applied various time intervals (15 minutes, 30 minutes, 60 minutes, 240 minutes, 480 minutes) to capture different aspects of market dynamics.

5. **Data Transformation for Model Training:**
   - Transformed the dataset by incorporating calculated features and labels, creating a comprehensive dataset for model training.
   - Saved the preprocessed dataset with new features and labels to a CSV file.


This notebook prepares the tick data for training a predictive model to forecast market direction in multiple time frames. The inclusion of diverse technical indicators and time-related features enhances the dataset's richness, providing a solid foundation for training robust prediction models.

