# Bina.az Rent Price Prediction (ML Project)

This project builds a Machine Learning model to predict apartment rental prices in Baku based on apartment features.

## Project Structure

Python_Classes/
- scraper/
  - bina_scraper.py
- data/
  - raw/
    - evler.csv
- eda.py
- model.py
- api.py
- model.joblib
- requirements.txt
- README.md

## Technologies Used

- Python
- Pandas
- Scikit-learn
- FastAPI
- Joblib

## How to Run the Project

Install dependencies:
pip install -r requirements.txt

Train the model:
python model.py

Run the API:
uvicorn api:app --reload

Open in browser:
http://127.0.0.1:8000/docs
