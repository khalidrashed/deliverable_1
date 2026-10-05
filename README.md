# INF201 – Deliverable 1

## Weather Data Analysis using MET Norway Frost API

This repository contains the solution for Deliverable 1 in INF201 at NMBU.

The project uses weather observations from the **MET Norway Frost API** for the weather station in Ås (`SN17850`).

## Tasks

The notebook contains five tasks:

1. **Daily mean air temperature**
   - Retrieves daily mean temperature for Ås during 2025.
   - Calculates mean, median, minimum and maximum temperature.
   - Visualizes the temperature throughout the year.

2. **Precipitation and temperature**
   - Retrieves daily precipitation for Ås during 2025.
   - Combines precipitation and temperature data.
   - Visualizes both variables in the same figure.

3. **Historical comparison**
   - Compares daily mean temperatures in Ås in 2025 with temperatures from 1925.
   - Provides summary statistics for both years.

4. **Heatwaves**
   - Identifies heatwaves using the Norwegian definition:
     at least 5 consecutive days with a maximum temperature of at least 27 °C.
   - The results are saved to a YAML file.

5. **Seven-day moving average**
   - Calculates a 7-day moving average of the daily mean temperature.
   - Visualizes the daily observations together with the moving average.

## Repository contents

- `deliverable_1.ipynb` – Main Jupyter Notebook containing the complete analysis.
- `heatwave_summary.yml` – Heatwave results for Ås in 2025.
- `README.md` – Description of the project.
- `.gitignore` – Prevents credentials and temporary files from being committed.

## Requirements

The analysis uses Python and the following packages:

- Python 3
- pandas
- requests
- matplotlib
- PyYAML
- Jupyter Notebook

The Frost API requires a MET Norway Frost client ID.

### API credentials

The Frost client ID is **not included in this repository**.

The notebook reads the client ID from a local file called:

```text
client_id.txt
