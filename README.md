# Bina.az Rent Price Prediction (ML Project)

This project builds a Machine Learning model to predict apartment rental prices in Baku based on apartment features.

## Project Structure

Python_Classes/
|
├── scraper/
│   └── bina_scraper.py
|
├── data/
│   └── raw/
│       └── evler.csv
|
├── eda.py
├── model.py
├── api.py
├── model.joblib
├── requirements.txt
└── README.md

## Technologies Used

- Python
- Pandas
- Scikit-learn
- FastAPI
- Joblib

## How to Run the Project

### 1. Install dependencies  

```
python model.py
```
uvicorn api:app --reload
```
http://127.0.0.1:8000/docs


```bash
pip install -r requirements.txt
