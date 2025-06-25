# Country Clustering Analysis using K-Means

# 📋 Project Overview
This project applies K-Means clustering to group countries based on socio-economic indicators using the Country-data.csv dataset. The analysis aims to identify distinct country profiles based on factors like child mortality, income, life expectancy, and GDP per capita.

# 📁 Dataset Summary
The dataset contains data for multiple countries with the following features:

child_mort: Child mortality per 1,000 live births

exports/imports: As % of GDP

health: Public health expenditure as % of GDP

income: Net income per person (USD)

inflation: Annual inflation rate (%)

life_expec: Life expectancy at birth (years)

total_fer: Total fertility rate

gdpp: GDP per capita (USD)

# 🛠️ Methodology
# 1. Data Preparation
Loaded and inspected the dataset using pandas.

Removed the non-numeric country column.

Scaled numeric features using MinMaxScaler for normalization.

# 2. Exploratory Data Analysis
Created scatter plots to examine relationships between each feature and GDP per capita.

# 3. Clustering
Used K-Means clustering with values of k ranging from 2 to 10.

Determined the optimal number of clusters (k=3) using:

Elbow Method (Inertia plot)

Silhouette Score

# 4. Cluster Visualization
Visualized clusters on two key feature spaces:

Child Mortality vs GDPP

Inflation vs GDPP

Used color-coded plots to distinguish between clusters.

# 📈 Results
Optimal clusters: 3

Silhouette Score: ~0.34 (moderate clustering structure)

Clear separation of countries based on development indicators:

One cluster contains low-GDP, high-mortality countries.

Another contains high-GDP, low-mortality countries.

# 🔍 Key Insights
Child Mortality and Income are strong indicators of country development.

Inflation appears to cluster independently, reflecting economic stability.

The analysis helps segment countries into development tiers for policy prioritization or aid targeting.

# 🧰 Technologies Used
Python

Pandas, NumPy

Scikit-learn

Seaborn, Matplotlib

