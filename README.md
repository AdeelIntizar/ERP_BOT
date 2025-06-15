# ERP Chatbot

A smart chatbot that helps with Enterprise Resource Planning (ERP) tasks. This bot uses AI to understand what users need and helps them with different business operations.

## What This Bot Does

The chatbot can help with these main business areas:

### Human Resources
- **Schedule Interviews**: Set up job interviews automatically
- **Check Employee Performance**: Look at how well employees are doing

### Project Management
- **View Project Details**: Get information about current projects
- **Track Project Progress**: See how projects are moving forward

### Financial Management
- **Request Project Money**: Ask for budget approval for projects
- **Handle Financial Tasks**: Manage money-related requests

### Supply Chain Management
- **Track Inventory**: Check what items are in stock
- **Monitor Stock Levels**: Keep track of available products

### Customer Relationship Management
- **Get Client Questions**: Find the latest questions from customers
- **Track Customer Issues**: See what customers are asking about specific projects

## How It Works

### Technology Used
- **AI Model**: BERT (a smart language model that understands text)
- **Database**: PostgreSQL to store all the data
- **Interface**: Gradio web app that users can interact with
- **Programming**: Python code that runs everything

## Setup Instructions

### What You Need First
- Python 3.8 or newer
- PostgreSQL database
- Git installed on your computer

### Step 1: Get the Code
```bash
git clone https://github.com/AdeelIntizar/ERP_BOT.git
cd ERP_BOT
```

### Step 2: Install Required Packages
```bash
# Install all needed Python packages
pip install -r requirements.txt
```

### Step 3: Download the AI Model
1. Go to this link: https://drive.google.com/drive/folders/1lhYipiG7DUd_xxqb06j8Ky8sXCjzDBcP?usp=sharing
2. Download the model files folder
3. Make sure the folder path matches what's written in the code:
   ```python
   model = BertForSequenceClassification.from_pretrained("checkpoint-210", use_safetensors=True)
   ```

### Step 4: Set Up Database
1. **Create Database**: Make a new PostgreSQL database
2. **Run Database Setup**: Execute the `database_tables.py` file to create all needed tables
3. **Update Database Settings**: Change the database connection details in your code to match your setup:
   ```python
   # Update these with your database information
   host = "localhost"
   database = "your_database_name"
   username = "your_username"
   password = "your_password"
   ```

### Step 5: Start the Bot
```bash
python gradio_app_code.py
```

## System Requirements

### Computer Specs Needed
- **Memory**: At least 8GB RAM (16GB is better)
- **Storage**: 5GB of free space
- **Graphics**: GPU is helpful but not required

### Software Needed
- Python 3.8+
- PostgreSQL 12+
- Web browser to use the chatbot

## Important Notes

1. **Model Files**: Make sure you download the model files from Google Drive
2. **Database Connection**: Check that your database settings are correct
3. **File Paths**: Verify all file paths in the code point to the right locations
4. **Dependencies**: Install all packages from requirements.txt before running

## Troubleshooting

### Common Issues
- **Can't find model**: Check if model files are in the right folder
- **Database errors**: Verify database is running and connection details are correct
- **Missing packages**: Run `pip install -r requirements.txt` again
- **Path errors**: Make sure all file paths in the code are correct

## Getting Help

If you run into problems:
1. Check that all files are in the right places
2. Make sure your database is running
3. Verify all Python packages are installed
4. Double-check your database connection settings

## Project Structure
```
ERP_BOT/
├── gradio_app_code.py          # Main application file
├── database_tables.py          # Database setup
├── requirements.txt            # Required Python packages
├── checkpoint-210/             # AI model files (download separately)
└── README.md                   # This file
```

---
*This README.md file provides complete setup and usage instructions for the ERP Chatbot system.*
