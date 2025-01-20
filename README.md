# Traffic Forecasting Rework

The goal of this project is to redo a hackathon project from 2022.

#### Primary objective: Create an app to predict the optimal time to pick up someone from the Austin Bergstrom airport based on your current location (latitude and longitude) and how traffic is in the area.

# Project Tasks

1. Create a framework to grab data from Azure Delta Lake storage.
2. Aquire appropriate traffic volume data (from the DOT - I used data from [here](https://www.fhwa.dot.gov/policyinformation/tables/tmasdata/)).
3. Aquire traffic incident data and combine with the volume data.
   - I started a framework to ingest official government data from [the Austin government traffic incident data API](https://data.austintexas.gov/stories/s/Austin-Travis-County-Traffic-Report-Page/9qfg-4swh/).
4. Aquire weather data to combine with these two datasets (source TBD).
5. Utiliza the flightradar24 API to grab real-time flight data.
6. Create an application to estimate the amount of time it will take given the traffic/weather conditions and when the flight will land.