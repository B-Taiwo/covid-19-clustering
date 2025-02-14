# COVID-19 Clustering for Targeted Health Action

## Project Overview
This project focuses on analyzing COVID-19 data using clustering techniques to uncover distinct patterns across different regions. By identifying these clusters, we aim to provide actionable insights for public health authorities and policymakers to tailor interventions based on regional needs and characteristics. 
The project explores how certain metrics, such as cases per 1,000 people, hospitalization rates, and population density, can inform the grouping of regions with similar outbreak profiles, allowing for more targeted and effective responses.

Why is this important? Understanding how regions differ in their COVID-19 metrics can help authorities prioritize healthcare resources, guide vaccination campaigns, and inform future pandemic preparedness efforts.
This data-driven approach ensures that responses are customized to each region’s unique situation, leading to more efficient and impactful public health strategies.

## Technologies Used
- Programming Language: Python
- Data Analysis and Processing Libraries: pandas, numpy, scipy
- Visualization: seaborn, matplotlib
- Clustering Algorithm: K-Means, Agglomerative Clustering (from scikit-learn) 
- Outlier Treatment: Winsorization (from scipy)
- Scaling: RobustScaler (from scikit-learn)
- Notebook Environment: Jupyter


## How to Run
To replicate this project,
1. Clone the repository to your local machine.
```bash
   git clone https://github.com/B-Taiwo/covid-19-clustering.git
```
2. Install the necessary dependencies by running:
```bash
pip install -r requirements.txt
```
3. Open and run the Jupyter notebook:
```bash
jupyter notebook Covid-19_Clustering.ipynb
```

## Project Results
The clustering analysis produced three distinct groups of regions based on COVID-19 metrics, 
population densities, and healthcare indicators. The results from K-Means and Agglomerative 
Clustering were compared using their silhouette scores.

K-means achieved a silhouette score of 0.88, indicating very good cluster cohesion and separation, 
while Agglomerative Clustering got a score of 0.79.

### Cluster Profiles
- Cluster 0 (Low-COVID Impact, Sparse Populations): This cluster represents regions with lower 
COVID-19 impact, relatively sparse populations, and lower usage of hospital resources.
- Cluster 1 (High-COVID Impact, Urban Regions): This cluster represents densely populated 
urban regions with a high COVID-19 burden. The high case and death counts suggest severe 
outbreaks or challenges in controlling of the spread, likely due to the dense population.
- Cluster 2 (Medium-COVID Impact, Moderate Populations): This cluster represents regions 
with moderate population density and COVID-19 impact. High testing rates and ICU utilization 
suggest that these regions have significant healthcare activity or readiness

## Actionable Recommendations
1. Maintain Proactive Measures in Low-Density Areas (Cluster 0): Continue preventive measures 
such as vaccination campaigns and health education to maintain the low-impact status and 
prevent future surges.
2. Enhance Testing and Containment in Urban Areas (Cluster 1): Focus resources on increasing 
testing capacity and strengthening containment measures in highly populated areas to reduce 
the high levels of cases and death rates.
3. Support Healthcare Infrastructure in Moderate Regions (Cluster 2): Increase ICU capacities and 
ensure that there are adequate staffing and medical supplies to manage high hospitalization 
and ICU usage rates effectively.

These insights provide a guide for policymakers and healthcare organizations to optimize resource 
allocation, and improve response strategies for pandemics and other healthcare problems.
