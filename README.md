
⚡ PJM Hourly Energy Consumption Forecast
This project aims to forecast hourly energy consumption for PJM Interconnection LLC using machine learning and time series modeling techniques. PJM is a regional transmission organization in the U.S. serving various states and the District of Columbia.
📈 Project Objective
The goal is to:
• Analyze hourly energy consumption trends across seasons, hours of the day, weekends, and holidays.
• Build predictive models to forecast demand for the next 30 days.
• Deploy a web app to interactively view and download forecasts.
📂 Project Structure
PJMW_MW_Hourly/
├── PJMW_MW_Hourly.xlsx # Historical hourly power consumption data (in MW)
├── PJMW_MW_Hourly - 7.ipynb # Main notebook for EDA, preprocessing, modeling
├── deployment_final.ipynb # Notebook for deployment using Streamlit
├── random_forest_model.pkl # Trained Random Forest model for forecasting
├── app.py # Final Streamlit app script
├── Requirement documenct.docx # Business and technical requirement overview
🔍 Exploratory Data Analysis (EDA)
• Time-series decomposition and visualization
• Analysis of seasonal trends and autocorrelation
• Holiday and weekend consumption comparisons
• Preprocessing including datetime formatting and sorting
🔧 Model Development
•	Random Forest: Used for the final deployment model
o	Features: hour, day, month, year, weekday, season, weekend/holiday flags
o	Evaluation on train-test split (last 1 year as test set)
•	Other models experimented: Linear Regression, XGBoost (if applicable)
🚀 Web Application (Streamlit)
The app provides:
•	Forecast for up to 30 future days
•	Interactive plots using matplotlib
•	Downloadable forecast as CSV
•	Suggestions for improvements
To run locally:
pip install streamlit pandas joblib matplotlib openpyxl
streamlit run app.py
📊 Sample Forecast
The model uses engineered time-based features to produce short-term energy demand forecasts, useful for planning and operational efficiency.
📌 Future Improvements
• Incorporate weather data for improved accuracy
• Holiday auto-detection using external APIs
• Hour-level forecasting granularity
• Add confidence intervals around predictions
📝 Authors & Acknowledgments
This project was developed as part of a data science internship. The dataset was obtained from PJM's public records. Special thanks to mentors for guidance on modeling and deployment strategies.
📌 How to Use
• Clone this repository to your local system.
• Open and run "PJMW_MW_Hourly - 7.ipynb" to explore the data and understand the model.
• Run "app.py" to launch the Streamlit web app.
• Use "random_forest_model.pkl" to make predictions on new data.
 
Let me know if you'd like this turned into a downloadable .md file once the tools are back online.

