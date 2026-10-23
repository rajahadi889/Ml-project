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
