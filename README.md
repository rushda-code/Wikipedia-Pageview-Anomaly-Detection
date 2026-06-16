# Wikipedia Pageview Anomaly Detection

## Overview

This project analyzes Wikipedia pageview traffic and detects unusual spikes in user interest using time series forecasting and anomaly detection techniques.

Daily pageview data is collected directly from the Wikimedia Pageviews API. A Prophet forecasting model is used to learn normal traffic behavior, and anomalies are identified when actual pageviews exceed the model's expected confidence range.

The project demonstrates how online attention patterns can be analyzed and linked to real-world events.

---

## Objectives

* Collect daily Wikipedia pageview data using the Wikimedia Pageviews API.
* Perform exploratory data analysis (EDA).
* Forecast expected pageviews using Prophet.
* Detect anomalous traffic spikes.
* Visualize trends, forecasts, and anomalies.
* Interpret anomalies as potential real-world events.

---

## Dataset

**Source:** Wikimedia Pageviews REST API

Data is fetched dynamically using:

https://wikimedia.org/api/rest_v1/

Articles analyzed:

* Cristiano Ronaldo
* Donald Trump
* Oppenheimer (Film)
* FIFA

Time Period:

* January 2022 – December 2024

---

## Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Prophet
* Requests
* Scikit-learn

---

## Methodology

1. Collect pageview data from Wikimedia API.
2. Clean and prepare the dataset.
3. Perform exploratory data analysis.
4. Split data into training and testing sets.
5. Train a Prophet forecasting model.
6. Generate future forecasts.
7. Compare actual vs predicted values.
8. Detect anomalies using Prophet confidence intervals.
9. Visualize detected anomalies.

---

## Results

* Successfully forecasted Wikipedia pageview trends.
* Detected 51 anomalous dates in the test period.
* Identified significant spikes that likely correspond to major real-world events.
* Demonstrated the effectiveness of Prophet for trend forecasting and anomaly detection.

---

## Evaluation Metrics

* Mean Absolute Error (MAE)
* Mean Absolute Percentage Error (MAPE)

---

## Future Improvements

* Compare Prophet with SARIMA and LSTM models.
* Build a real-time monitoring dashboard.
* Integrate news APIs to automatically explain anomalies.
* Analyze a larger set of Wikipedia articles.

---

## Conclusion

This project shows how time series forecasting and anomaly detection can be used to identify unusual patterns in Wikipedia traffic. The detected anomalies provide insights into periods of heightened public interest and demonstrate the relationship between online information consumption and real-world events.
