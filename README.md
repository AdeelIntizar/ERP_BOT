This is an ERP chatbot which assists the user for followings ERP related tasks:  
**1-	Human Resources**  
  a.	Scheduling an interview  
  b.	Checking performance of an employee  
**2-	Project Management**  
  a.	Check project details  
**3-	Financial Management**  
  a.	Request money for a project  
**4-	Supply chain Management**  
  a.	Track inventory and stock  
**5-	Customer Relationship Management**  
  a.	Getting latest queries of a client on particular project  

  To use this interactive chatbot you first need to clone it using **https://github.com/AdeelIntizar/ERP_BOT.git**  
  After cloning the bot you need to install all depedencies from **requirements.txt** file  
  The Project model is trained on google colab and model files are used  
  So first you need to download model files directory from this link ** **  
  After downloading this directory you need to make sure that the path of directory is correctly added in the code where the model is getting loaded **(model = BertForSequenceClassification.from_pretrained("checkpoint-210", use_safetensors=True))**  
  Secondly the bot is running on locally created database  
  The database here used is Postgresql  
  First you need to create database and after creating the database the tables are created in database_tables.py file so create them make sure to update credentials of database while creating the connection  
  Now just run the gradio_app_code.py file and  make sure all the paths and functions loading from other files are correctly added.  
  
