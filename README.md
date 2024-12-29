# Construction Cost Overrun Prediction

## Project Overview
This project aims to predict construction cost overruns based on various factors related to the type, location, and features of a building. The goal is to create a model that helps construction firms estimate the potential for cost overruns during the planning and building phases.

## Data Description
The dataset contains information about property sales, including characteristics of the buildings and the type of sale. The columns in the dataset include:

- `locality`: The location of the property.
- `type_of_property`: The type of building. Either 'House' or 'Apartment'.
- `subtype_of_property`: More detailed classification of the property type. (e.g, House, villa)
- `price`: The final sale price of the property.
- `type_of_sale`: Indicates if the sale was private or through a realtor.
- `number_of_rooms`: Number of rooms in the building.
- `house_area`: The total living area of the house (in square meters).
- `fully_equipped_kitchen`: Indicates if the kitchen is fully equipped.
- `furnished`: Indicates if the house is furnished.
- `open_fire`: Indicates the presence of an open fire.
- `terrace`: Indicates if there is a terrace.
- `terrace_area`: Area of the terrace (in square meters).
- `garden`: Indicates if there is a garden.
- `garden_area`: Area of the garden (in square meters).
- `surface_of_the_land`: Total area of land on which the property is built.
- `surface_of_the_plot_of_land`: Area of the land on which the house is situated.
- `number_of_facades`: Number of facades of the building.
- `swimming_pool`: Indicates if there is a swimming pool.
- `state_of_the_building`: Condition of the building (e.g., new, renovated).
- `construction_year`: Year the building was constructed.

## Problem Statement
The construction industry faces challenges in accurately predicting cost overruns for building projects. This project aims to develop a predictive model that estimates the likelihood of a cost overrun based on the provided features of the property.

## Approach

### Data Preprocessing
1. **Missing Value Handling**: Check for and handle missing values across the dataset.
2. **Feature Engineering**: 
   - Convert categorical features to numerical (e.g., `type_of_property`, `fully_equipped_kitchen`).
   - Normalize numerical features (e.g., `house_area`, `price`) for model compatibility.
3. **Data Splitting**: Split the dataset into training and testing sets.

### Exploratory Data Analysis (EDA)
1. **Univariate Analysis**: Investigate the distribution of key features such as `price`, `house_area`, and `number_of_rooms`.
2. **Correlation Analysis**: Analyze correlations between features and the target variable (`price` or any indicator of cost overrun).
3. **Feature Importance**: Identify the most influential features for predicting cost overruns.
### Feature Engineering


### Modeling
1. **Model Selection**: Train multiple models, including:
   - Linear Regression
   - Decision Trees
   - Random Forest
   - Gradient Boosting Machines (GBM)
2. **Model Evaluation**: Evaluate models using metrics such as R-squared, Mean Absolute Error (MAE), and Root Mean Squared Error (RMSE).

### Cross-Validation
Perform k-fold cross-validation to validate model performance and avoid overfitting.

## Results and Conclusion
- **Model Performance**: Compare the performance of different models.
- **Insights**: Identify key factors influencing construction cost overruns.
- **Business Implication**: Provide recommendations for construction firms on how to mitigate cost overruns.

## Future Work
- Incorporate additional data sources, such as historical project budgets or external economic factors.
- Explore deep learning models to capture complex relationships in the data.

## References
- List any references or research papers consulted during the project.

