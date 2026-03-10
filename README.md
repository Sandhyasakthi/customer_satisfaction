# AI-Driven Customer Satisfaction Prediction System

## Project Overview

The **AI-Driven Customer Satisfaction Prediction System** is a machine learning-based web application that predicts customer satisfaction based on service-related inputs. The system uses a trained **CatBoost machine learning model** integrated with a **Flask web application** to generate predictions in real time.

Users can log in to the system, provide feedback or service ratings, and receive predictions about customer satisfaction. The system also stores the data for reporting and analysis.

---

## Technologies Used

### Frontend

* HTML
* CSS

### Backend

* Python
* Flask Framework

### Machine Learning

* CatBoost Classifier

### Database

* SQLite Database

### Tools

* Git
* GitHub
* VS Code

---

## Project Structure

```
tata_steel_ai_project
│
├── catboost_info/
│
├── model/
│   ├── catboost_model.cbm
│   └── train_model.py
│
├── static/
│   └── style.css
│
├── templates/
│   ├── dashboard.html
│   ├── feedback.html
│   ├── login_signup.html
│   ├── predict.html
│   └── reports.html
│
├── app.py
├── catboost_model.cbm
├── create_db.py
└── database.db
```

---

## Folder Explanation

### model/

Contains machine learning components.

* **train_model.py**
  Used to train the CatBoost machine learning model.

* **catboost_model.cbm**
  The trained model used for prediction.

---

### static/

Contains static frontend files.

* **style.css**
  Defines the styling and layout for the web application.

---

### templates/

Contains HTML pages used by the Flask application.

* **login_signup.html** – User login and registration page
* **dashboard.html** – Main dashboard after login
* **predict.html** – Page where users input service parameters for prediction
* **feedback.html** – Used to collect customer feedback
* **reports.html** – Displays stored reports or prediction results

---

### app.py

The main Flask application file.

Responsibilities include:

* Running the Flask server
* Managing routes and navigation
* Loading the machine learning model
* Handling prediction requests
* Connecting to the database

---

### create_db.py

This script initializes and creates the SQLite database required for the application.

---

### database.db

The SQLite database file that stores:

* User information
* Feedback data
* Prediction results

---

### catboost_info/

Automatically generated during model training and contains training logs and metrics.

---

## Machine Learning Model

The system uses the **CatBoost classification algorithm** to predict customer satisfaction.

### Input Features

Example parameters used for prediction:

* Service Quality
* Product Satisfaction
* Delivery Experience
* Customer Support Rating

### Output

The model predicts whether the customer is:

* **Satisfied**
* **Not Satisfied**

---

## Application Workflow

1. User opens the web application.
2. User registers or logs into the system.
3. User accesses the dashboard.
4. User enters service-related parameters.
5. The Flask backend sends input data to the trained CatBoost model.
6. The model predicts customer satisfaction.
7. The result is displayed on the webpage.
8. Data is stored in the SQLite database for reports.

---

## Installation and Setup

### 1. Clone the Repository

```
git clone https://github.com/your-username/tata_steel_ai_project.git
```

### 2. Navigate to Project Directory

```
cd tata_steel_ai_project
```

### 3. Install Dependencies

```
pip install flask catboost pandas scikit-learn
```

### 4. Create Database

```
python create_db.py
```

### 5. Run the Application

```
python app.py
```

### 6. Open in Browser

```
http://127.0.0.1:5000
```

---

## Future Improvements

* Add data visualization dashboards
* Improve model accuracy with larger datasets
* Implement user role management
* Deploy the application on a cloud platform
* Add advanced analytics for customer insights

---

## Author

Sandhya S

AI and Machine Learning Academic Project

