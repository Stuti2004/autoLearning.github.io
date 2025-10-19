# autoLearning.github.io
Machine Learning without any coding
A web-based machine learning application that allows users to upload datasets, perform exploratory data analysis (EDA), configure and train machine learning models, and visualize results.
The project uses a hybrid backend with Node.js for file handling and API endpoints, and Python (Flask) for ML model training.

## Features
- Upload CSV or Excel datasets.
- Perform EDA (data shape, info, head, missing values, correlation, feature importance).
- Configure ML models with customizable features, normalization, and train-test splits.
- Train models using various algorithms (e.g., Linear Regression, Logistic Regression, Random Forest, SVM, Gradient Boosting).
- User authentication (signup/login) with a MySQL database.

## Tech Stack
- **Frontend**: HTML, CSS, JavaScript
- **Backend**:
  - Node.js with Express for API, file uploads, and EDA
  - Python with Flask for ML model training
- **Database**: MySQL
- **Libraries**:
  - Node.js: `mysql2`, `cors`, `multer`, `papaparse`, `xlsx`
  - Python: `flask`, `pandas`, `numpy`, `scikit-learn`, `flask-cors`
- **Tools**: `concurrently` for running both servers


### 1. Clone the Repository

git clone https://github.com/your-username/autolearning.git

cd autolearning


### 2. Set Up the Database

Create a login table with the following SQL:

CREATE DATABASE demo_schema;

USE demo_schema;

CREATE TABLE login (

    id INT AUTO_INCREMENT PRIMARY KEY,
    
    name VARCHAR(255) NOT NULL,
    
    email VARCHAR(255) NOT NULL UNIQUE,
    
    mobile VARCHAR(10) NOT NULL,
    
    password VARCHAR(255) NOT NULL

);



### 3. Install Dependencies

npm install

pip install flask pandas numpy scikit-learn flask-cors


### 4. Run the Application

Start both the Node.js and Python servers simultaneously:

npm run start-both
