# Datasets Documentation

This project utilizes several datasets from the U.S. Energy Information Administration (EIA), providing a comprehensive view of energy trends across various sectors. Below is detailed information about each dataset used in our analysis.

## 1. Total Energy Overview Dataset
- **Purpose**: Track production and consumption of various fuels across different sectors and states
- **Variables**: 
  - Energy source (coal, petroleum, natural gas, renewables)
  - Consumption
  - Production
  - End-users
  - State
- **Size**: Several thousand records detailing annual energy production and consumption
- **Limitations**: Some states may have missing data for certain years, especially for newer renewable sources

## 2. Stagewise Renewable Energy Consumption Dataset
- **Purpose**: Provide state-level data on production and consumption of renewable energy sources
- **Variables**:
  - State
  - Energy source (renewable)
  - Production capacity
  - State rankings for energy consumption
- **Size**: Data from 50 U.S. states
- **Limitations**: Some states with smaller renewable energy production may have limited data availability

## 3. CO2 Emissions by Source Dataset
- **Purpose**: Track state-level CO2 emissions from different energy sources
- **Variables**:
  - Year
  - State
  - CO2 emissions (thousand metric tons)
  - Energy source (coal, petroleum, natural gas)
- **Size**: Historical data from 1950 to 2023
- **Limitations**: Some emission values may be interpolated or estimated

## 4. Renewable Energy Production and Consumption by Source Dataset
- **Purpose**: Track renewable energy production and consumption by source from 1949 to 2024
- **Variables**:
  - Year
  - Renewable energy source
  - Production and consumption figures (kilowatt-hours)
  - State
- **Size**: Data spanning several decades
- **Limitations**: Earlier data for renewables may be incomplete

## Data Sources
All datasets are sourced from the U.S. Energy Information Administration (EIA):
- [Total Energy Browser](https://www.eia.gov/opendata/browser/total-energy)
- [Renewable Energy Data](https://www.eia.gov/renewable/data.php#summary)
- [CO2 Emissions Data](https://www.eia.gov/opendata/browser/co2-emissions/co2-emissions-and-carbon-coefficients)
- [Monthly Energy Data](https://www.eia.gov/totalenergy/data/monthly/)
- [State Energy Data](https://www.eia.gov/state/?sid=US)
- [SEDS Complete Data](https://www.eia.gov/state/seds/seds-data-complete.php)

## Data Structure
The analysis primarily worked with the following data points:
- Energy consumption by state and sector
- Renewable energy adoption metrics
- Environmental impact indicators
- Economic correlations

## Data Processing
1. **Data Extraction**
   - Used EIA API endpoints
   - Downloaded structured CSV files
   - Accessed through data browsers

2. **Data Cleaning**
   - Standardized units and measurements
   - Handled missing values
   - Normalized state names and codes

3. **Data Integration**
   - Combined multiple data sources
   - Created unified analysis datasets
   - Established common keys for joining

## Note
Due to the size of the raw data files, they are not included in this repository. All data can be accessed directly through the EIA websites and APIs listed above. 