# Airbnb Price Prediction in Rome

This project predicts Airbnb prices in Rome using Bayesian inference, focusing on identifying the most relevant features that impact pricing.

## 💾 Dataset
The dataset was sourced from [Inside Airbnb](https://insideairbnb.com/rome/), a free platform providing public data on Airbnb listings. It includes 72 features, of which the most relevant were selected:
- **Price:** Nightly rate (target variable)
- **Accommodates:** Number of guests
- **Beds:** Number of beds
- **Room Type:** Type of accommodation
- **Latitude & Longitude:** Coordinates of the listing
- **Availability365:** Number of available days in a year
- **Host Acceptance & Response Rate:** Host behavior metrics
- **Number of Reviews & Review Scores**: Communication, location, cleanliness
- **Neighborhood & Property Type**

## 🔧 Feature Engineering
To enhance the dataset, I:
1. Created new features by calculating the Haversine distance from each listing to four iconic landmarks in Rome:
   - Colosseum
   - Vatican
   - Trastevere
   - Piazza di Spagna
2. Normalized numerical features and handled missing values.
3. Transformed categorical variables and binarized certain features (e.g., guest capacity).

## 📊 Exploratory Data Analysis (EDA)
Visualizations revealed:
- High listing density in the historic center, Trastevere, Vatican, and Piazza di Spagna.
- Price variations based on neighborhood and property type.
- Entire homes/apartments dominate the market.
- Strong correlation between price and distance to landmarks.

## 🧠 Modeling
- Frequentist Linear Regression
- Bayesian Linear Model
- Advanced Bayesian Model


## 🟢 Model Comparison
| Model                      | R-Squared |
|----------------------------|-----------|
| Frequentist Linear Model   | 4.8631    |
| Bayesian Linear Model      | 0.4622    |
| Advanced Bayesian Model    | 0.4621    |
