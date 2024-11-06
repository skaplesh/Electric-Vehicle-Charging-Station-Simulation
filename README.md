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

Follow these steps to set up the project on your local machine:

1. **Clone the repository**  
   Clone the project from the Git repository using the following command:

   ```bash
   git clone https://github.com/your-username/ev-charging-simulation.git


2. **Navigate to the project directory**
Change into the project directory:

```bash
cd Electric-Vehicle-Charging-Station-Simulation

3. **Install Python**
Ensure that Python is installed on your machine, with a minimum version of 3.6.6. You can check your Python version with:

```bash
python --version

If you need to install Python, download and install the correct version from the official Python website.

4. **Install dependencies**

Install all required Python packages listed in requirements.txt:

```bash
pip install -r requirements.txt

Now you’re ready to use the project. For usage instructions, refer to the Usage section.






