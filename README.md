
# Expense Tracker

This is a simple web-based Expense Tracker application built using **Flask** for the backend and **HTML/CSS** for the frontend. It allows users to add, view, and save their expenses to a CSV file.

**Screenshots**
1- The GUI
![image](https://github.com/user-attachments/assets/67b5cae2-ee9d-4b96-ad2f-a40ffce36198)

2- Adding Expense
![image](https://github.com/user-attachments/assets/20999848-fe4e-4fa7-b79a-89615bec7b19)

## Features
- **Add an expense**: Users can input the date, category, description, and amount of an expense.
- **View expenses**: All added expenses are displayed in a table format on the same page.
- **Save to CSV**: Users can download their expenses as a CSV file.
- **Responsive UI**: The frontend is designed to be user-friendly and works on mobile and desktop.

## Technologies Used
- **Backend**: Flask (Python)
- **Frontend**: HTML, CSS
- **Data Storage**: Pandas DataFrame (stored in memory during runtime)
- **CSV File Format**: For exporting expenses

## Requirements
- Python 3.x
- Flask
- Pandas

## Setup and Installation

### 1. Clone the repository
bash
git clone https://github.com/yourusername/expense-tracker.git
cd expense-tracker


**2. Install the required dependencies**
Make sure you have Python 3.x installed on your system. If not, download and install it from the official Python website.

Install the required libraries using pip:
pip install flask pandas


**3. Run the application**
To start the backend server, run the following command:

python app.py


This will start the Flask server at http://localhost:5000. You can open this URL in your web browser to use the app.

**Usage**
1. Adding Expenses
Enter the Date, Category, Description, and Amount of the expense in the form and click the Add Expense button.
The expense will be added to the table below.
2. Viewing Expenses
All added expenses will be displayed in a table below the input form. This table will show the date, category, description, and amount of each expense.
3. Saving Expenses to CSV
Click the Save to CSV button to download the expenses as a CSV file. This will trigger the download of the file containing the list of expenses.


**File Structure**
The project has the following structure:
expense-tracker/
│
├── app.py                # Backend logic (Flask app)
├── templates/
│   └── index.html        # Frontend HTML file
├── static/
│   └── style.css         # CSS styles for the frontend
└── README.md             # This readme file



app.py
This is the main backend file that:

Handles routing (/add_expense, /save_to_csv)
Manages expenses in a Pandas DataFrame
Serves the frontend HTML page
Provides CSV download functionality
templates/index.html
This file contains the HTML structure for the frontend, where users can add expenses, view the expense table, and download the CSV file.

static/style.css
This file contains the CSS styles to make the app look visually appealing and responsive.

Troubleshooting
"######" in the CSV file: If the date is displayed as ######, it means the column width is too narrow in Excel or similar spreadsheet applications. This issue is fixed by ensuring that the date is formatted as a string (YYYY-MM-DD) before saving to CSV.

Missing dependencies: Make sure you have installed all the necessary libraries using the command pip install flask pandas.

Contributing
Feel free to fork the repository, create a new branch, and submit a pull request if you would like to contribute. Please ensure your code is well-documented and tested.

License
This project is open-source and available under the MIT License.
