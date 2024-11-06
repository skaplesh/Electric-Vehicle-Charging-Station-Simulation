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
## Dataset

The project uses the `station_data_dataverse.csv` dataset, which includes data on EV charging sessions such as:
- `sessionId`: Unique identifier for each charging session
- `kwhTotal`: Total kilowatt-hours charged
- `dollars`: Charging cost in dollars
- `startTime`, `endTime`: Charging session start and end times
- `chargeTimeHrs`: Duration of the charging session in hours
- Additional fields covering weekday, location, and facility type.

Ensure the dataset is placed in the `station_data_dataverse.csv` directory or update the path in the Jupyter Notebook as necessary.

## Installation


Clone this repository:

```bash
git clone https://github.com/your-username/ev-charging-simulation.git
cd ev-charging-simulation

## Installation dependencies:

pip install -r requirements.txt





