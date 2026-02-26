# energy_anomaly_detection
Building Energy Anomaly Detection using Machine Learning
-->Building Energy Anomaly Detection using Machine Learning

-->Overview
This project focuses on detecting abnormal energy consumption patterns in buildings using an unsupervised machine learning approach.  
The system analyzes multiple energy streams and identifies unusual behavior that may indicate equipment faults, energy inefficiencies, or operational anomalies.
The project uses the **Building Data Genome Project 2 (BDG2)** dataset and applies feature engineering with an **Isolation Forest** model to detect anomalies automatically without labeled data.

-->Objectives
- Analyze multi-energy building consumption data
- Engineer time-based and statistical features
- Detect abnormal energy usage patterns
- Visualize anomalies for practical insights

-->Dataset
Building Data Genome Project 2 (BDG2)
Energy streams used:
- Electricity
- Chilled Water
- Hot Water
- Steam
- Gas
- Water
- Solar
- Irrigation

Each dataset contains time-series energy readings for multiple buildings.

-->Project Pipeline
1.Data Preprocessing
- Timestamp conversion
- Handling missing values
- Dataset reshaping (wide → long format)
- Merging multiple energy datasets

2.Feature Engineering
- Hour, day-of-week, and month features
- Weekend indicator
- 24-hour rolling mean
- 24-hour lag feature
- Absolute deviation from rolling baseline

3.Model
Isolation Forest (Unsupervised Learning)
The model learns normal energy consumption behavior and isolates unusual observations as anomalies.

->Visualizations
1.Electricity Consumption with Detected Anomalies
Red points indicate abnormal energy usage detected by the model.
2.Buildings with Highest Anomaly Counts
Identifies buildings with the most irregular energy behavior.

->Results
- Approximately 1–2% of observations were detected as anomalies.
- The model successfully identified unusual consumption spikes and irregular building behavior.
- Provides actionable insights for energy monitoring and facility management.

Technologies Used
- Python
- Pandas
- NumPy
- Scikit-learn
- Matplotlib
- Jupyter Notebook
