# Tanzania Faulty Water Pumps Prediction

## Pumps States Analysis and Modelisation 

Mahdi KRIAA

In this project we aim to leverage machine learning techniques to predict the operational status of water pumps in Tanzania. The goal is to identify faulty water pumps before they fail, allowing for timely maintenance and minimizing downtime. Water supply in Tanzania is critical, and pump failures can have significant impacts on local communities. By predicting these failures, we can ensure a more reliable water supply and improve the quality of life for these communities.

## Data Source:
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
