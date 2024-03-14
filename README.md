# Phishing URL Detection Project

## Introduction
The Internet has become an indispensable part of our lives, but it also poses risks, such as phishing attacks. Phishers attempt to deceive users by creating fake websites to steal sensitive information. Machine learning offers effective methods for detecting these malicious activities by identifying common characteristics of phishing websites.

## Project Overview
This project aims to detect phishing URLs using machine learning algorithms and a web-based interface. It provides users with the ability to input a URL, select a prediction algorithm, and receive the prediction results on a web interface.

## Components

### 1. app.py
The `app.py` file contains the Flask application responsible for handling user requests, running predictions using trained machine learning models, and displaying results on the web interface.

### 2. feature.py
The `feature.py` module implements feature extraction methods to analyze URLs and extract relevant features used for phishing detection. It utilizes various techniques, such as analyzing URL structure, checking domain registration information, and inspecting HTML content.

### 3. Requirements
The `requirements.txt` file lists all required Python libraries and dependencies necessary to run the project. It includes packages such as Flask, BeautifulSoup, scikit-learn, and requests.



##### 1- beautifulsoup4==4.9.3
##### 2- Flask==2.0.2
##### 3- googlesearch_python==1.0.1
##### 4- numpy==1.21.4
##### 5- pandas==1.3.4
##### 6- python_dateutil==2.8.2
##### 7- requests==2.25.1
##### 8- scikit_learn==1.0.1
##### 9- whois==0.9.13
##### 10-gunicorn==20.1.0





### 4. Directory Tree
The directory structure of the project is organized as follows:

├── pickle
│ └── model.pkl
├── static
│ └── styles.css
│ └── photo
├── templates
│ └── index.html
├── app.py
├── feature.py
├── phishing.csv


### 5. model.pkl
The `model.pkl` file contains a trained machine learning model used in the project. It is created using machine learning algorithms such as Gradient Boosting Classifier to detect phishing URLs. The model includes parameters, weights, and other necessary information to make predictions on input data.

## Usage
1. **Installation**: Ensure Python 3.7 is installed. Install required packages using `pip install -r requirements.txt`.
2. **Running the Application**: Execute `app.py` to start the Flask server.
3. **Accessing the Interface**: Visit `http://localhost:5000` in your web browser to access the web-based interface.
4. **Entering URL**: Enter the URL you want to analyze in the provided input field.

## Conclusion
#### 1- The final take away form this project is to explore various machine learning models, perform Exploratory Data Analysis on phishing dataset and understanding their features.
#### 2- Creating this notebook helped me to learn a lot about the features affecting the models to detect whether URL is safe or not, also I came to know how to tuned model and how they affect the model performance.
#### 3- The final conclusion on the Phishing dataset is that the some feature like "HTTTPS", "AnchorURL", "WebsiteTraffic" have more importance to classify URL is phishing URL or not.
#### 4- Gradient Boosting Classifier currectly classify URL upto 97.4% respective classes and hence reduces the chance of malicious attachments.

## Contributors

Sekandari Hamidreza
