# Pub_sub_to_BigQ_project
Explore The Google cloud pub/sub to insert btc price to BigQueryTable.
Cloud Functions streaming insert to BigQuery (with Cloud Pub/Sub trigger). In this example, the function will make a REST API call to get a data and insert to BigQuery.

# Step to Run 
Create BigQuery table with a proper schema (using Google Cloud Console).
Create a Pub/Sub topic. When deploy Cloud Functions via Console (web UI), there is a button to create a topic.
Deploy Cloud Function. (alternatively: use make deploy as a prompt deploy command)
Set Cloud Scheduler.

![image](https://github.com/user-attachments/assets/a39a1e38-bb46-42e5-b563-e235b1c12c1a)

# Methodology 
1. Create New Project in GCP
![image](https://github.com/user-attachments/assets/f5e1b053-4af0-4127-a05a-b25830d09a20)

2.Create Dataset and Table in BigQ to store the btc price
![image](https://github.com/user-attachments/assets/0f8ddad4-e91f-4a0c-ba2b-8d60fcabefa9)<br>

3.Create Cloud Function and Env variable <br>
<p align="center">
  <img src="https://github.com/user-attachments/assets/56e591d2-d84e-4135-a11d-3b588c888549"/>
</p>

![image](https://github.com/user-attachments/assets/c9497cd5-cc92-4605-998b-26c6dbb88ce5)

4.Create Scheduler to trigger the Cloud Function
![image](https://github.com/user-attachments/assets/1776ec48-2b95-4c5b-a5c6-e84fad711962)

5.Final Result : The scheduler will trigger the cloud Function and add price data to the Table 
![image](https://github.com/user-attachments/assets/9faf38df-4036-4b5b-bdcb-6ed6cbcc358a)

<p align="center">
  <img src="https://github.com/user-attachments/assets/f3077d39-0255-4d8b-b955-b885f1541eb9"/>
</p>

<p align="center">
  <img src="https://github.com/user-attachments/assets/e3b1be9e-ccda-42ff-9904-22088c3d0b5d"/>
</p>









