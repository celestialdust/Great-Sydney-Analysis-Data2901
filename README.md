# Greater Sydney Analysis Project

### Overview

This repository contains the code and resources for the **Greater Sydney Analysis Project**, developed as part of the DATA2x01 Data Science and Big Data course. This project aims to compute a "bustling" score for each Statistical Area Level 2 (SA2) region in Greater Sydney, quantifying how well-resourced and active each neighborhood is based on various datasets. 

### Project Goals

The objective of this project is to:
- Integrate diverse datasets and perform spatial data analysis.
- Calculate a "bustling" score for each SA2 area in Greater Sydney using factors such as public transport stops, polling places, school catchment areas, and selected business statistics.
- Extend the score by incorporating additional datasets for further insights.
- Perform a correlation analysis to examine the relationship between the bustling score and median income across SA2 regions.

### Technologies Used

- **Python**: For initial data loading, cleaning, and data pre-processing.
- **PostgreSQL**: To store and manage data, utilizing SQL for data manipulation and score computation.
- **PostGIS**: For spatial data handling within PostgreSQL, used to manage and analyze geographical data.

### Datasets

The project leverages several datasets, including:
- **SA2 Regions**: Digital boundaries for SA2 regions within Greater Sydney.
- **Businesses**: Data on business counts by industry within each SA2.
- **Public Transport Stops**: Locations of bus and train stops in GTFS format.
- **Polling Places**: Locations of polling places from the 2019 Federal election.
- **School Catchments**: Defined areas for school enrollment.
- **Population and Income**: Demographic data to support per-capita and correlation analyses.

Additional datasets sourced by each team member expand the score’s accuracy and relevance.

### Installation

1. **Clone the Repository**:
   ```bash
   git clone <repository-url>
   ```
2. **Install Required Packages**:
   Make sure you have the necessary Python packages:
   ```bash
   pip install psycopg2-binary numpy pandas matplotlib geopandas
   ```
3. **Set Up PostgreSQL with PostGIS**:
   - Install PostgreSQL and the PostGIS extension.
   - Create a PostgreSQL database with spatial data support.

### Usage

1. **Data Import**:
   Load all datasets into PostgreSQL with an organized schema and prepare for SQL-based analysis.
   
2. **Score Calculation**:
   Run the Jupyter Notebook to calculate the bustling score using a custom formula based on normalized values for business presence, transport stops, polling places, and school areas.

3. **Visualizations**:
   Visualize the score across SA2 regions through interactive maps or graphs.

### Contributing

We welcome contributions to enhance this project. Please refer to our contributing guidelines for more information.

### Acknowledgments

We would like to thank:
- The **TensorFlow team** for providing foundational resources.
- **Australian Bureau of Statistics** and **Transport for NSW** for the public datasets.

### License

This project is open-source and available under the MIT License. See the LICENSE file for more details.
