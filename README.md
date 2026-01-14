# CitiBike x Insurance – Data Science Challenge

Recommendation: Check out the report first.

## Task

Citi Bike operates a bike-sharing system in New York City with over 12,000 bikes across 750 stations and publishes trip data to the public. In this project, the goal is to use Citi Bike trip data (e.g., monthly tripdata files) and optionally combine it with public NYPD traffic accident data to create value—such as outlining potential cooperation opportunities between Citi Bike and an insurance provider (or vice versa). All analysis results and code should be version-controlled with Git and shared as a complete package (documents + code) ahead of the scheduled meeting.

## Data Sources

- Citi Bike Trip Data: https://s3.amazonaws.com/tripdata/index.html
- NYPD Motor Vehicle Collisions: https://data.cityofnewyork.us/Public-Safety/Motor-Vehicle-Collisions-Crashes/h9gi-nx95/about_data
- Weather Data: https://open-meteo.com/en/docs/historical-weather-api?start_date=2012-07-01&end_date=2025-12-29&latitude=40.7143&longitude=-74.006

## Project Structure

- `notebooks/` analysis and modeling
- `reports/` report
- `data/` local only (not tracked by git)
- `models/` trained models

## How to run

1. Create the environment (see `environment.yml`).
2. Download the Motor Vehicle Collisions dataset and the weather data into `data/`.
3. Download Citi Bike data from 11-2024 to 10-2025 into `data/citi_bike_raw/zip_files`, then unpack into `data/citi_bike_raw/unpacked`.
4. Run the notebooks in order.

## Results

- Architecture of a dynamic pricing model (described in `reports/`)
- Daily accident prediction model
- Probabilistic end-station prediction model for Citi Bike trips

## To Do

- MoG for accident density depending on latitude, longitude, and time of day
- MoG for traffic Density depending on latitude and longitude
- Combine all results to realize the end-to-end dynamic pricing model

