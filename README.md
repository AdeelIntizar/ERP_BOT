# ERP Chatbot
[Page Url :](https://www.iiu.edu.pk/)
This is an ERP chatbot that assists the user with the following ERP-related tasks:

## 1. Human Resources
- Scheduling an interview
- Checking the performance of an employee

## 2. Project Management
- Checking project details

## 3. Financial Management
- Requesting money for a project

## 4. Supply Chain Management
- Tracking inventory and stock

## 5. Customer Relationship Management
- Getting the latest queries of a client on a particular project

---

### **Usage Instructions**

1. **Clone the Repository:**
   To use this interactive chatbot, clone the repository using the following command:
   ```bash
   git clone https://github.com/AdeelIntizar/ERP_BOT.git
2. **Installing dependencies**  
  After cloning the bot you need to install all depedencies from **requirements.txt** file  
3. **Download Model files**  
  The Project model is trained on google colab and model files are used  
  So first you need to download model files directory from this link **https://drive.google.com/drive/folders/1lhYipiG7DUd_xxqb06j8Ky8sXCjzDBcP?usp=sharing**  
  After downloading this directory you need to make sure that the path of directory is correctly added in the code where the model is getting loaded **(model = BertForSequenceClassification.from_pretrained("checkpoint-210", use_safetensors=True))**

   4.**Setup Database**  
  Secondly the bot is running on locally created database  
  The database here used is Postgresql  
  First you need to create database and after creating the database the tables are created in database_tables.py file so create them make sure to update credentials of database while creating the connection

5.**Run the Bot**  
  Now just run the gradio_app_code.py file and  make sure all the paths and functions loading from other files are correctly added.  
  
