# Optimizing-Walmart-Sales-Strategy-with-Predictive-Analytics


# Optimizing Walmart's Sales Strategy with Predictive Analytics

## Problem
Walmart faces challenges due to significant seasonal variations in sales. If the company fails to anticipate these variations, it could experience substantial financial losses. Predicting future sales is crucial for enabling the company to:
- Arrange stocks effectively
- Calculate revenue projections accurately
- Decide on new investments
- Influence stock prices and investor perceptions positively

Conversely, failing to meet projected sales targets could damage stock prices and investor confidence, posing a critical challenge, especially for a large-scale company like Walmart.

## Aim
The aim of this project is to build a model that predicts sales for Walmart stores. This predictive model will enable Walmart to:
- Arrange stocks effectively
- Calculate revenue projections
- Make informed investment decisions
- Respond proactively to seasonal sales variations

## Solution
An accurate prediction model will enable Walmart to:
1. Determine seasonal demands and take timely actions
2. Avoid financial losses by meeting sales targets, positively impacting stock prices and investor perceptions
3. Forecast revenue easily and accurately
4. Manage inventory efficiently
5. Plan and execute more effective marketing campaigns

## Plan
1. **Understanding, Cleaning, and Exploring Data**:
   - Analyze the seasonal effects on sales and categorize sales data by weeks of the year and holiday periods.

2. **Preparing Data for Modeling**:
   - Encode boolean and string features.
   - Prepare data by encoding all columns for modeling.

3. **Modeling Approaches**:
   - **Random Forest Regressor**: Perform feature selection based on feature importance to achieve a Weighted Mean Absolute Error (WMAE) of 1801.
   - **ARIMA/Exponential Smoothing/ARCH Models**: Handle non-stationary data using techniques like differencing, log transformations, and shifts. Exponential Smoothing yielded the best result with a WMAE of 821.

## Metric
The metric for this project is **Weighted Mean Absolute Error (WMAE)**. Errors during holiday periods are weighted differently to reflect their importance.

## Findings
1. **Departmental and Seasonal Effects**:
   - While some departments have higher sales during certain seasons, other departments may outperform overall averages.
   - Seasonal sales trends vary significantly by department (e.g., Thanksgiving impacts some departments more).

2. **Store-Level Insights**:
   - Sales trends vary significantly based on store size categories (A, B, C). Larger stores (type A) have higher sales volumes.
   - Seasonal sales spikes are prominent in certain areas.

3. **Holiday Sales**:
   - Average holiday sales exceed non-holiday sales.
   - Top 4 sales periods are Christmas, Thanksgiving, Black Friday, and the 22nd week (late May, when schools close).
   - Christmas shopping peaks during the 51st week of the year, not the final week.

4. **Monthly Trends**:
   - January sales are significantly lower due to high sales during November and December.

5. **External Factors**:
   - CPI, temperature, unemployment rate, and fuel price show no clear pattern with weekly sales.

## More Detailed Findings
Detailed exploration and findings are available in the notebooks included in this repository.

## Future Improvements
1. Apply advanced techniques to make data more stationary.
2. Perform more detailed feature engineering and selection.
3. Incorporate additional data to analyze holiday effects and include holidays like Easter, Halloween, and Back-to-School periods.
4. Enhance markdown modeling by department.
5. Develop specialized models for specific stores or departments.
6. Conduct market basket analysis to identify high-demand items by department.

## Repository Structure
- **Data/**: Contains datasets used for analysis.
- **Walmart_Sales_Forecasting.ipynb**: Jupyter Notebook with data cleaning, exploration, and predictive modeling.
- **README.md**: Detailed documentation of the project.

## How to Run the Project
1. Clone the repository:
   ```bash
   git clone https://github.com/SuryaVegesna27/Optimizing-Walmart-Sales-Strategy-with-Predictive-Analytics.git
   ```
2. Navigate to the project folder:
   ```bash
   cd Optimizing-Walmart-Sales-Strategy-with-Predictive-Analytics
   ```
3. Install the required libraries:
   ```bash
   pip install -r requirements.txt
   ```
4. Open the Jupyter Notebook:
   ```bash
   jupyter notebook Walmart_Sales_Forecasting.ipynb
   ```

## Contributing
Contributions are welcome! Please feel free to submit issues or pull requests for improvements.

## License
This project is licensed under the MIT License. See the LICENSE file for details.
