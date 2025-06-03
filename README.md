# PHISH
A Comprehensive AI-Powered Phishing Detection and Prevention Platform
PISH is a Python-driven application that integrates with a Gmail account to fetch emails and determine whether they are phishing or legitimate using a pre-trained machine learning algorithm.  
![WhatsApp Image 2025-06-03 at 17 59 09_ae79b47c](https://github.com/user-attachments/assets/814552e8-c1ef-4c17-a5a6-1498953786bb)


- Phishing Detection: Utilizes advanced machine learning algorithms to assess emails for phishing content with high accuracy.  
- Email Retrieval: Connects to Gmail via IMAP to fetch emails based on customizable search filters.  
- Secure Access: Ensures secure integration by using encrypted credentials for email account access.  
- User-Friendly Interface: Features a Flask-based web platform for seamless user interaction, including credential input and email analysis.  
- Organized Results: Displays analysis outcomes in a structured table for better readability and understanding.  
- Customizable Criteria: Allows users to tailor email search parameters to suit their specific needs.  
- Scalability: Designed to handle large volumes of emails efficiently for analysis.

  
USAGE WORKFLOW:

### Step 1: Email Extraction  
- Access the web app and log in using your Gmail address and app password.  
- The `email_extract.py` script:  
  - Establishes a connection to Gmail using the IMAP protocol.  
  - Retrieves emails based on specified filters (e.g., sender’s email address).  
  - Extracts the plain text content of each email and records it in a file named `emails.csv`.  

### Step 2: Email Analysis  
- After extraction, the `email_analyzer.py` script:  
  - Cleanses the email content by removing HTML tags, URLs, special characters, and converting it to lowercase.  
  - Employs a pre-trained machine learning model and vectorizer to determine if each email is phishing (1) or legitimate (0).  
  - Stores the results in a file called `classified_emails.csv`.  

### Step 3: Viewing Results  
- Visit the "Results" section of the web app to explore the analysis outcomes, presented in an organized table.  
