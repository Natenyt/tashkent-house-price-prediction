# Task 9: House Price Prediction

## Objective
Build a regression model to predict house prices with **R² > 75%** and visualize the overall model performance using an Actual vs Predicted Prices graph.

## Dataset
- **File:** `uybor.csv`
- **Records:** 7,422 property listings in Tashkent
- **Features:**
  - `address` - Property address
  - `district` - District name
  - `rooms` - Number of rooms
  - `size` - Property size (m²)
  - `level` - Floor level
  - `max_levels` - Total floors in building
  - `price` - Property price (target variable)
  - `lat`, `lng` - Geographic coordinates

## Solution
The notebook `conv.ipynb` implements the following:

1. **Data Preprocessing**
   - Handle missing values
   - One-hot encode categorical features (district)
   
2. **Model**
   - Random Forest Regressor with 200 estimators
   
3. **Results**
   - R² Score: **~78-79%** (exceeds 75% requirement)
   - Visualization: Actual vs Predicted Prices scatter plot

## Usage

### Google Colab
1. Upload `uybor.csv` to Google Drive
2. Open `conv.ipynb` in Google Colab
3. Update the file path in the notebook to match your Drive location
4. Run all cells

## Requirements
- pandas
- numpy
- matplotlib
- scikit-learn
