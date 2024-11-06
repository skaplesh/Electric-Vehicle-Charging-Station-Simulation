# Electric-Vehicle-Charging-Station-Simulation
This project simulates different scenarios of electric vehicle (EV) charging station operations using Python, focusing on demand prediction, dynamic pricing, and anomaly detection.
## Table of Contents
- [Dataset](#dataset)
- [Installation](#installation)
- [Project Structure](#project-structure)
- [Scenarios](#scenarios)
- [Encryption](#encryption)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)
# Dataset
The project uses the station_data_dataverse.csv dataset, which includes data on EV charging sessions such as:

sessionId: Unique identifier for each charging session
kwhTotal: Total kilowatt-hours charged
dollars: Charging cost in dollars
startTime, endTime: Charging session start and end times
chargeTimeHrs: Duration of the charging session in hours
Additional fields covering weekday, location, and facility type.
Ensure the dataset is placed in the data/ directory or update the path in the Jupyter Notebook as necessary.

# Installation
Clone this repository:
https://github.com/skaplesh/Electric-Vehicle-Charging-Station-Simulation
cd Electric-Vehicle-Charging-Station-Simulation
Install dependencies:
pip install -r requirements.txt
# Project Structure
data/: Directory to store input datasets.
EV_Charging_Simulation.ipynb: Jupyter Notebook file containing the code for simulations and visualizations.
README.md: Project documentation.
# Scenarios
1. Price Surge
This scenario simulates a sudden increase in charging prices at selected stations and observes how it affects demand.

2. Overload Simulation
Models increased demand at certain stations and dynamically adjusts prices based on the increased load.

3. Dynamic Pricing Based on Peak and Off-Peak Hours
Adjusts prices according to peak and off-peak hours using a game theory approach, accounting for competitive pricing.

4. Malicious User Detection - Resource Hoarding
Detects abnormal user behavior, such as resource hoarding, using anomaly detection with Isolation Forest, and adjusts pricing for detected malicious behavior.
#Encryption
To secure sensitive data (e.g., reservation counts and actual usage), the project uses AES encryption. Sensitive fields in the dataset are encrypted before analysis, and decrypted only in a secure environment.

# Usage
To run the simulations and view the results, open the Jupyter Notebook:
jupyter notebook EV_Charging_Simulation.ipynb

Run each cell in the notebook to execute the simulation scenarios and visualize demand and pricing data. The notebook includes code for generating various plots to analyze the effects of pricing and demand changes.

# Contributing
Contributions are welcome! Please fork this repository, create a feature branch, and submit a pull request with your changes.

# License
This project is licensed under the MIT License.
