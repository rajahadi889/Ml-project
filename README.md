# Ml-project
This repo contains my ml projects on credit analysis and diamond price prediction. I have tested linear and logistic regression on these datasets and found out useful findings.

#Credit Analysis ML Web App
Overview
This project uses machine learning to identify serious loan delinquency with Logistic Regression. It includes a FastAPI backend and an HTML frontend, allowing users to interact with the model through a web page.

Requirements
Install the required libraries by running this command:

pip install pandas numpy scikit-learn joblib fastapi uvicorn
How to Run
Open Credit_Analysis.ipynb in Google Colab or Jupyter Notebook.

Upload the cs-training.csv dataset to the location specified in the notebook.

Run the notebook cells in order to prepare the data, train the model, and save it.

Run the relevant notebook cells to create main.py and index.html.

Start the FastAPI backend by running:

uvicorn main:app --reload
Open http://127.0.0.1:8000 in your browser to access the web app.

Features
Classifies serious loan delinquency
Uses FastAPI for the backend
Provides an HTML user interface
Note
Keep the trained model files, main.py, and index.html in the same project folder. Make sure the dataset path matches your setup so the notebook can find the file

#Diamond Price Prediction ML Web App
Overview
This project uses Linear Regression to predict diamond prices based on their characteristics, such as carat, cut, color, clarity, depth, table, and dimensions. It includes a FastAPI backend and an HTML frontend that allows users to enter diamond details and receive a predicted price.

Requirements
Install the required libraries by running:

pip install fastapi uvicorn joblib scikit-learn pandas numpy matplotlib
How to Run
Open diamond_price.ipynb in Google Colab or Jupyter Notebook.
Upload the diamonds.csv dataset. If you have diamonds_csv.zip, extract it first.
Run the notebook cells in order to explore and clean the data, train the Linear Regression model, and evaluate its performance.
Run the remaining cells to save the trained model and performance metrics, set up the FastAPI backend, and create the HTML frontend.
Run the server cell in the notebook.
Open the displayed web app link to start predicting diamond prices.
If you are running the app locally, start the backend with:

uvicorn main:app --reload
Then open http://127.0.0.1:8000 in your browser.

Features
Predicts diamond prices in US dollars
Uses Linear Regression for price prediction
Takes diamond characteristics as input
Estimates dimensions when exact measurements are unknown
Displays prediction results through an HTML interface
Shows model performance metrics, including R², MAE, and RMSE
Keeps a history of recent predictions
Note
The notebook expects the dataset at /content/diamonds.csv in Google Colab. Make sure the file is available at the correct path before running the cells.

The trained model and metrics are saved as diamond_linear_regression.joblib and diamond_metrics.joblib. Keep these files available when running the backend.
