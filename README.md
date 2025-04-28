# Airbnb NYC Listings(2024) EDA & Visualization with Python
<img src = 'https://github.com/user-attachments/assets/886570a4-8927-4f46-8e96-aae51ea00dd5' width = '600'>

## 📋 **Overview**

This project performs an Exploratory Data Analysis (EDA) and Data Visualization on Airbnb listings in New York City for 2024. The goal is to uncover trends, identify outliers, and derive actionable insights from the dataset to understand pricing, availability, and neighborhood dynamics.

----
## 🛠️ **Technologies Used**
- Python
- Pandas (Data Manipulation)
- NumPy (Numerical Operations)
- Matplotlib & Seaborn (Visualizations)
- Jupyter Notebook (Interactive Analysis)

----
## 🎯 **Objective**
The goal of this project is to:
1. Analyze **room types, prices, and availability** across different neighborhoods.
2. Understand **host behavior** and listing patterns.
3. Detect potential **outliers** in prices.
4. Provide recommendations for guests and hosts based on insights.

---

## 📁 **Dataset**
The dataset contains **20,765 entries and 22 features**, including:
- **id**: Unique identifier for each listing  
- **name**: Title of the Airbnb listing  
- **host_name**: Name of the host  
- **neighborhood_group**: Group (borough) where the listing is located  
- **latitude/longitude**: Geolocation of listings  
- **price**: Nightly rental price  
- **room_type**: Type of accommodation (e.g., entire home, private room)  
- **reviews_per_month**: Average monthly reviews for the listing  
- **availability_365**: Number of available days in the year  

----
## ✏️**Steps and Workflow**

### 1. Data Cleaning
- **Handle missing data**: `price`, `neighborhood`, and `beds` columns had null values.
- **Fix data types**: Converted `last_review` to a **datetime** object.
- **Remove outliers**: Listings with prices > $1,000 were capped to avoid skewed visualizations.

### 2. EDA (Exploratory Data Analysis)
1. **Room type distribution**: 
   - Visualized the count of each room type using **bar plots**.
   - Identified **Entire home/apt** as the most common room type.

2. **Neighborhood group insights**:
   - Analyzed **price variations by boroughs**.
   - Manhattan had the **highest average prices**.

3. **Availability trends**:
   - Used **heatmaps** to show correlations among `price`, `availability_365`, `number_of_reviews`, and `beds`.

4. **Price distribution**:
   - Used **histograms** to show the distribution of prices.
   - Majority of the listings were priced between **$50 - $300**.

5. **Host listings**:
   - Analyzed hosts with multiple listings using **boxplots** to identify key contributors.

6. **Review behavior**:
   - Used **pair plots** to show relationships between number of reviews, price, and availability.
---

## 🔍 **Key Findings and Insights**
1. **Price Trends**:  
   - **Manhattan** has the most expensive listings, followed by Brooklyn.  
   - **Entire homes/apartments** cost significantly more than private or shared rooms.  

2. **Room Type Distribution**:  
   - **Entire homes/apartments** are the most common, but **private rooms** offer budget-friendly options.

3. **Outliers in Price**:  
   - Few listings priced at **$10,000+** were detected, indicating the need to filter such extreme values.

4. **Availability Patterns**:  
   - Listings with **high availability** tend to have lower prices and more reviews, likely due to better guest experience.

5. **Host Behavior**:  
   - Some hosts manage **multiple listings**, indicating a trend toward professional hosting.
----
## 📊 **Key Visualizations**
1. **Price Distribution**:<br>
   <img src = 'https://github.com/user-attachments/assets/ee4cb588-2918-4974-a841-a122c8cc6869' width = '450'>
2. **Price by Neighbourhood and Room Type**:<br>
   <img src = 'https://github.com/user-attachments/assets/11531cd1-0cc9-4a64-82c7-7786f03233cf' width = '450'>
3. **Locality and Review Dependency**:<br>
   <img src = 'https://github.com/user-attachments/assets/9eb9fcac-6c1c-435c-83eb-3dab663e7615' width = '450'> <br>
[Access the Jupyter Notebook]('./airbnb_python_eda.ipynb')
## 📌 **Recommendations**
- **For Guests**: 
   - Look for listings with high availability and good reviews for a better experience.
   - **Private rooms** in Brooklyn offer affordable stays compared to Manhattan.

- **For Hosts**:  
   - Improve **availability** and **review response rates** to attract more bookings.
   - Manage pricing effectively to compete within the borough's market.

---

## **Future Work**
- Use **machine learning** to predict prices based on room type and location.
- Perform **sentiment analysis** on reviews to better understand guest experiences.
- Create an **interactive dashboard** using Plotly or Tableau for live monitoring.

---

## ✔️ **Conclusion**
This project offers valuable insights into the New York Airbnb market, helping both guests and hosts make informed decisions. By using **EDA techniques**, we identified key trends and developed actionable recommendations. Future improvements can involve advanced analytics and predictive modeling to further enhance the findings.

---
