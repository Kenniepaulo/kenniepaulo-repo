# kenniepaulo-repo
Credit Card Fraud Detection Application
Overview
This application is designed to help detect fraudulent credit card transactions in real-time. By inputting specific transaction details, the system predicts whether a transaction is fraudulent or legitimate using a pre-trained Neural Network model.

The application features an intuitive interface, quick processing, and is suitable for financial institutions or other users concerned with fraud prevention.

Key Features
Fast Predictions: The system provides instant results to determine if a transaction is fraudulent or legitimate.
Simple Interface: Users can easily input transaction details into the application.
Accurate Detection: Built with a robust Neural Network model optimized for fraud detection.
Variables Involved
Input Variables
These variables are used by the model to make predictions:

Merchant ID

Type: Numeric (float)
Description: A unique identifier for the merchant.
Average Amount/Transaction per Day

Type: Numeric (float)
Description: The average monetary amount per transaction for the day.
Transaction Amount

Type: Numeric (float)
Description: The amount involved in the current transaction.
Is Declined

Type: Numeric (integer, 0 or 1)
Description: Whether the transaction was declined.
0 = No
1 = Yes
Total Number of Declines per Day

Type: Numeric (integer)
Description: The total number of declined transactions for the merchant on the given day.
Is Foreign Transaction

Type: Numeric (integer, 0 or 1)
Description: Indicates if the transaction is foreign.
0 = No
1 = Yes
Is High Risk Country

Type: Numeric (integer, 0 or 1)
Description: Indicates if the transaction originates from a high-risk country.
0 = No
1 = Yes
Daily Chargeback Average Amount

Type: Numeric (float)
Description: The average chargeback amount for the day.
Output
Fraudulent or Legitimate
Type: Categorical (string)
Description: The model predicts whether the transaction is suspicious or safe.
Fraudulent: Transaction is suspicious.
Legitimate: Transaction is safe.
How to Use
1. Setting It Up
Install Python: Download and install Python from python.org.
Install Required Libraries:
Open a terminal or Command Prompt and run:
bash
Copy code
pip install streamlit tensorflow numpy
2. Running the Application
Download the application files:
app.py (main application file).
best_neural_network_model.keras (pre-trained model file).
Ensure both files are in the same folder.
Open a terminal and navigate to the folder:
bash
Copy code
cd "C:/Users/akinb/OneDrive/New folder (2)/app"
Run the application with the command:
bash
Copy code
streamlit run app.py
A browser window will open displaying the app interface.
3. Using the Interface
Input Transaction Details:
Fill in fields for details like Merchant ID, Transaction Amount, etc.
Make a Prediction:
Click the Predict button.
View Results:
The app will show whether the transaction is Fraudulent or Legitimate.
What Happens Behind the Scenes
The app uses a pre-trained Neural Network model stored in the best_neural_network_model.keras file.
The entered transaction details are processed and sent to the model.
The model analyzes patterns in the data and predicts if the transaction is fraudulent.
Troubleshooting
App Not Opening: Ensure you run the correct command:
bash
Copy code
streamlit run "C:/Users/akinb/OneDrive/New folder (2)/app/app.py"
Incorrect Predictions: Check if the input fields are filled correctly with realistic values.
Missing Model File: Confirm that the best_neural_network_model.keras file is in the same directory as app.py.
Contact
If you have any questions, need assistance, or want to provide feedback, feel free to reach out:

Kehinde Paul Akinbile
📧 Email: akinbile.kenny@gmail.com

