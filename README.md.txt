Table of Contents
Dataset
Installation
Project Structure
Scenarios
Encryption
Usage
Contributing
License
Dataset
The project uses the station_data_dataverse.csv dataset, which includes data on EV charging sessions such as:

sessionId: Unique identifier for each charging session
kwhTotal: Total kilowatt-hours charged
dollars: Charging cost in dollars
startTime, endTime: Charging session start and end times
chargeTimeHrs: Duration of the charging session in hours
Additional fields covering weekday, location, and facility type.
Ensure the dataset is placed in the data/ directory or update the path in the Jupyter Notebook as necessary.

Installation
Clone this repository:

bash
Copy code
git clone https://github.com/your-username/ev-charging-simulation.git
cd ev-charging-simulation
Install dependencies:

bash
Copy code
pip install -r requirements.txt
Project Structure
data/: Directory to store input datasets.
EV_Charging_Simulation.ipynb: Jupyter Notebook file containing the code for simulations and visualizations.
encryption_utils.py: Script with AES encryption/decryption functions for handling sensitive data.
README.md: Project documentation.
Scenarios
Price Surge
This scenario simulates a sudden increase in charging prices at selected stations and observes how it affects demand.

Overload Simulation
Models increased demand at certain stations and dynamically adjusts prices based on the increased load.

Dynamic Pricing Based on Peak and Off-Peak Hours
Adjusts prices according to peak and off-peak hours using a game theory approach, accounting for competitive pricing.

Malicious User Detection - Resource Hoarding
Detects abnormal user behavior, such as resource hoarding, using anomaly detection with Isolation Forest, and adjusts pricing for detected malicious behavior.

Encryption
To secure sensitive data (e.g., reservation counts and actual usage), the project uses AES encryption. This is implemented in the encryption_utils.py script. Sensitive fields in the dataset are encrypted before analysis, and decrypted only in a secure environment.

Usage
To run the simulations and view the results, open the Jupyter Notebook:

bash
Copy code
jupyter notebook EV_Charging_Simulation.ipynb
Run each cell in the notebook to execute the simulation scenarios and visualize demand and pricing data. The notebook includes code for generating various plots to analyze the effects of pricing and demand changes.

Contributing
Contributions are welcome! Please fork this repository, create a feature branch, and submit a pull request with your changes.

License
This project is licensed under the MIT License.