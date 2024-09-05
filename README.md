# House Sales in King County Analysis: Tableau Implementation

## Overview

This details the analysis questions, visualizations, and analyses conducted for House Sales in King County – Tableau Implementation.

## 1. Data Set Details

The dataset used is `kc_house_data.xlsx`, which contains information on house sale prices in King County, including Seattle. The dataset covers homes sold from May 2014 to May 2015.

- **File Size:** 2,457 KB
- **Sheet Name:** `kc_house_data`
- **Number of Rows:** 21,613
- **Number of Columns:** 21

### Column Descriptions

- `id`: Unique ID for each home sold
- `date`: Date of the home sale
- `price`: Price of each home sold
- `bedrooms`: Number of bedrooms
- `bathrooms`: Number of bathrooms (0.5 denotes a room with a toilet but no shower)
- `sqft_living`: Square footage of the interior living space
- `sqft_lot`: Square footage of the land space
- `floors`: Number of floors
- `waterfront`: Indicates if the property overlooks the waterfront (dummy variable)
- `view`: Index from 0 to 4 indicating the quality of the view (0 = No view, 4 = Excellent)
- `condition`: Index from 1 to 5 indicating the condition of the property (1 = Poor, 5 = Very Good)
- `grade`: Index from 1 to 13 indicating the construction and design quality
- `sqft_above`: Square footage of the interior space above ground level
- `sqft_basement`: Square footage of interior space below ground level
- `yr_built`: Year the house was built
- `yr_renovated`: Year of the last renovation
- `zipcode`: Zip code of the property
- `lat`: Latitude
- `long`: Longitude
- `sqft_living15`: Square footage of interior living space for the nearest 15 neighbors
- `sqft_lot15`: Square footage of land lots of the nearest 15 neighbors

Additionally, a `meta-data.xlsx` file includes geographical data and indices related to conditions, waterfront properties, and views.

## 2. Data Connections and Relationships

### Data Connections

Data connections were established using the 'Extract' connection method to ensure that visualizations are based on a static snapshot of the data at a specific point in time. The Data Interpreter in Tableau was used to enhance data understanding and preparation.

### Data Relationships

Effective relationships between tables in Tableau were established, particularly connecting `kc_house_data` with information from the `meta-data` file.

## 3. Visualization and Analyses

### Question 1: Distribution of Bedrooms and Bathrooms

- The distribution of bedrooms and bathrooms shows that three bedrooms and two and a half bathrooms are common, with notable frequencies in houses with this configuration.
- Higher prices are associated with houses having three or four bedrooms and two and a half bathrooms.

### Question 2: Average House Price and Year Built, Age, and Condition

- Newer constructions generally command higher prices, although older houses from 1905 and 1933 also show high prices.
- Renovations in 2001 and 1987 contribute to higher house prices, indicating the value of recent updates.

### Question 3: House Prices by Location

- Higher prices are observed in central areas such as Medina, Beaux Arts, and Mercer Island, suggesting a premium for central locations.

### Question 4: Impact of Square Footage on House Prices

- The square footage of living space is more significant than lot size in determining house prices.
- Larger living spaces, both above ground and in the basement, correspond to higher prices.
- Maps illustrate the variations in living space and lot size across locations, with certain cities showing larger areas and higher prices.

### Question 5: Effect of View, Waterfront Access, and Condition on Prices

- Houses with a waterfront, even with an average view or condition, have higher prices.
- The view's quality is a significant factor, but the number of floors does not significantly interact with the view quality in affecting house prices.

### Question 6: Month-by-Month Sales Growth Rates

- June and July 2014 saw the highest sales growth, indicating a favorable summer trend in the housing market.
- A decline in sales from November 2014 to February 2015 suggests potential seasonal effects.

### Question 7: Forecast of Housing Prices

- The forecast suggests that housing prices will peak in early July 2015 and remain relatively stable afterward.
- Newer houses (post-2013) are expected to see a substantial increase in prices, with a general decline post-2023 aligning with historical trends.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
