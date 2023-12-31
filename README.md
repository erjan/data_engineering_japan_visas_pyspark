# data_engineering_japan_visas_pyspark
data engineering project - visualize visa numbers by country, time issued from japan

This is small data engineering project to learn how to install apache spark cluster on server, learn the workflow of interaction with apache spark/local machine via pyspark. 

Original tutorial: https://www.youtube.com/watch?v=f-IcM8mFmDc&t=160s

Visualized map:

![Screenshot_8](https://github.com/erjan/data_engineering_japan_visas_pyspark/assets/4441068/85eda6ae-18a5-445b-9dbd-4026496426c3)


 2nd map:
![Screenshot_13](https://github.com/erjan/data_engineering_japan_visas_pyspark/assets/4441068/e8d0fe19-0c77-40ec-af3d-99163e0f0c2e)

 
1. create venv in local project folder: python -m venv japan-visa-de

2. download dataset of japan visa csv file - https://www.kaggle.com/datasets/yutodennou/visa-issuance-by-nationality-and-region-in-japan

3. create vm in ec2 (t2.xlarge), download ssh key, move ssh key to project folder using "scp" cmd

4. chmod 400 your private_key.pem

5. install docker compose via image

6. run docker compose to bring up spark cluster

6. enable inbound rule in sec group in aws ec2 to see spark master web ui on port 9090

7. write pyspark code , upload on the spark cluster machine and execute using spark-submit

8. download back results of work to local machine - visualized images/html
   
