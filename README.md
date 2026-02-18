Airline Passenger Traffic Forecasting
📌 Project Objective
The goal of this project is to analyze and predict monthly international airline passenger numbers. This is a classic Time Series Analysis problem where the goal is to understand historical patterns (Trend and Seasonality) to forecast future demand.

📊 Dataset
Name: Air Passengers Dataset (1949 - 1960).

Features: Monthly timestamp and total passenger count.

Characteristics: The data exhibits a clear upward Trend and strong Yearly Seasonality.

🛠️ Methodology
I implemented two distinct approaches to compare performance:

Machine Learning (Random Forest): A baseline model that uses lagged observations (the previous 12 months) as features.

Deep Learning (LSTM): A Recurrent Neural Network (RNN) that uses "memory gates" to learn long-term dependencies in the data sequence.

🧪 Preprocessing Steps
Datetime Indexing: Converted string dates into a time-based index.

Min-Max Scaling: Normalized data to a range of (0, 1) for stable neural network training.

Sliding Window: Created sequences where 12 months of data are used to predict the 13th month.

📈 Key Results
Visualization: The LSTM model captured the seasonal "peaks" of summer travel more accurately than the standard Random Forest model.

Performance: (Enter your MAE values from your Google Colab results here).

🚀 How to Run
Open the .ipynb file in this repository.

Click the "Open in Colab" badge at the top.

Run all cells to see the data visualizations and model comparisons.
