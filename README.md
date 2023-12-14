# Tanzania Faulty Water Pumps Prediction

## Project Description 

This project aims to leverage machine learning techniques to predict the operational status of water pumps in Tanzania. The goal is to identify faulty water pumps before they fail, allowing for timely maintenance and minimizing downtime. Water supply in Tanzania is critical, and pump failures can have significant impacts on local communities. By predicting these failures, we can ensure a more reliable water supply and improve the quality of life for these communities.

## Data Source
The data for this project comes from Kaggle and it is originally comes from the Taarifa waterpoints dashboard, which aggregates data from the Tanzania Ministry of Water.

Link to dataset : https://www.kaggle.com/datasets/sumeetsawant/pump-it-up-challenge-driven-data?select=training_Set_values.csv
https://drive.google.com/file/d/1syH81TVrbBsdymLT_jl2JIf6IjPXtSQw/view

For this dataset, there were 59400 rows and 41 columns.

## Data Dictionary
amount_tsh: Total static head (amount water available to waterpoint)
\
date_recorded: The date the row was entered
\
funder: Who funded the well
\
gps_height: Altitude of the well
\
installer: Organization that installed the well
\
longitude: GPS coordinate
\
latitude: GPS coordinate
\
wpt_name: Name of the waterpoint if there is one
\
num_private: is it private
\
basin: Geographic water basin
\
subvillage: Geographic location
\
region: Geographic location
\
region_code: Geographic location (coded)
\
district_code: Geographic location (coded)
\
lga: Geographic location
\
ward: Geographic location
\
population: Population around the well
\
public_meeting: True/False
\
recorded_by: Group entering this row of data
\
scheme_management: Who operates the waterpoint
\
scheme_name: Who operates the waterpoint
\
permit: If the waterpoint is permitted
\
construction_year: Year the waterpoint was constructed
\
extraction_type: The kind of extraction the waterpoint uses
\
extraction_type_group: The kind of extraction the waterpoint uses
\
extraction_type_class: The kind of extraction the waterpoint uses
\
management: How the waterpoint is managed
\
management_group: How the waterpoint is managed
\
payment: What the water costs
\
payment_type: What the water costs
\
water_quality: The quality of the water
\
quality_group: The quality of the water
\
quantity: The quantity of water
\
quantity_group: The quantity of water
\
source: The source of the water
\
source_type: The source of the water
\
source_class: The source of the water
\
waterpoint_type: The kind of waterpoint
\
waterpoint_type_group: The kind of waterpoint
\
group_state: Water pump state 

## Methodologie

We will employ various data preprocessing techniques to handle missing values and categorical variables. We will explore different machine learning models, including random forests and gradient boosting, to predict the operational status of the pumps. Model performance will be evaluated based on accuracy, precision, recall, and F1 score.

## Exploratory Data Analysis

### Explanatory Visuals

The exploratory visuals include the following plots:

    - a boxplot and histogram was visualized for each numeric column.
    - an histogram was visualized for each categorical column.
    - a contingency matrix for some categorical columns
    
<p align = "center"> 
  <img src = "https://github.com/Mahdi-Kriaa/faulty_water_pumps_predicton/blob/main/Images/pumps_states_histogram.png">
</p>

This histogram shows that the "fonctional needs repair" state is the minority one and the "non functional" state represente a significante part of the dataset.

### Explanatory Visuals

<p align = "center"> 
  <img src = "https://github.com/Mahdi-Kriaa/faulty_water_pumps_prediction/blob/main/Images/pumps_sates_over_45.png">
</p>

The magority of pumps states is non functional when the pump is oprating over 45 years so there is high risk of failure over this operating period.

<p align = "center"> 
  <img src = "https://github.com/Mahdi-Kriaa/faulty_water_pumps_prediction/blob/main/Images/pumps_sates_vs_management.png">
</p>

The majority of non functional states are vwc managed. So it's most likely that there is a problem with this type of management.
