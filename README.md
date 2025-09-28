# ✈️ Flight Price Prediction

---


## 📝 Problem Statement

Flight ticket prices are notoriously unpredictable. Today’s fare might be different from tomorrow’s for the same flight. Travelers often experience this inconsistency, making it difficult to plan budgets.

This project aims to use **machine learning** to predict flight ticket prices. Accurate predictions can help:

* ✈️ **Travelers**: Plan their trips and book tickets at optimal times.
* 🏢 **Airlines**: Determine dynamic pricing strategies and maintain competitive fares.

By analyzing historical flight data, the model can estimate expected ticket prices based on key features such as airline, route, departure time, and more.

## 📊 Dataset

The dataset used in this project contains information about flights, including:

* 🛫 **Airline**: The airline operating the flight.
* 📅 **Date_of_Journey**: The date of the flight.
* 🏙️ **Source**: The departure city.
* 🏢 **Destination**: The arrival city.
* 🛤️ **Route**: The flight path taken.
* ⏰ **Departure**: The departure time.
* 🕓 **Arrival**: The arrival time.
* ⏱️ **Duration**: The total duration of the flight.
* 🔄 **Total_Stops**: The number of stops.
* ℹ️ **Additional_Info**: Additional information about the flight.
* 💰 **Price**: The target variable representing the ticket price.

## 🛠️ Tools & Libraries

* 🐍 Python
* 📊 Pandas
* 🔢 NumPy
* 📈 Matplotlib
* 🎨 Seaborn
* 🤖 Scikit-learn

## 🔑 Key Points About the Dataset

* 🎯 **Target Variable**: `Price` (numeric, regression problem)
* 🗂️ **Categorical Variables**: `Airline`, `Source`, `Destination`, `Route`, `Total_Stops`, `Additional_Info`
* ⏳ **Date & Time Columns**: Need feature extraction (Day, Month, Hour, Minute)
* ✏️ **Text Features**: `Duration`, `Route` → convert to numeric for model input
* ❗ **Missing Values**: Some columns like `Additional_Info` or `Stops` may have missing or “No info” values → needs handling
* ⚠️ **Outliers**: Flight prices vary widely; some flights may have extremely high or low prices

## 🧪 Model Training & Evaluation

* 📏 **Linear Regression**: Baseline model
* 🌲 **Random Forest Regressor**: Handles non-linear relationships
* ⚡ **Gradient Boosting**: Advanced ensemble technique

## 🚀 Deployment

The trained model can be deployed using **Flask** or **FastAPI** to create a web application where users can input flight details and receive price predictions.

## 📈 Results

* 📉 Linear Regression: Basic understanding of relationships
* 🌳 Random Forest Regressor: Better accuracy, handles non-linear relationships
* ⚡ Gradient Boosting: Highest accuracy using ensemble techniques

## 🔮 Future Improvements

* 🔧 Hyperparameter tuning for better performance
* ➕ Add more features like flight class, day of the week
* ☁️ Deploy on cloud platforms for scalability
