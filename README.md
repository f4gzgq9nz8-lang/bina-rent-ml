# Bina.az Rent Price Prediction (ML Project)

This project builds a Machine Learning model to predict apartment rental prices in Baku based on apartment features such as area, number of rooms, floor, building type, and location.

## Project Structure

Python_Classes/
│
├── scraper/
│   └── bina_scraper.py
│
├── data/
│   └── raw/
│       └── evler.csv
│
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

1. Install dependencies:
```bash
pip install -r requirements.txt
Train the model:

bash
Kodu kopyala
python model.py
Run the API:

bash
Kodu kopyala
uvicorn api:app --reload
Open in browser:

arduino
Kodu kopyala
http://127.0.0.1:8000/docs
Example Usage
After running the API, you can send a POST request to the /predict endpoint with apartment features:

json
Kodu kopyala
{
  "rooms": 2,
  "area": 55,
  "floor": 3,
  "total_floors": 5,
  "repair_type": "Yeni tikili",
  "building_type": "Bakixanov",
  "location": "Bakıda"
}
The API will return the predicted monthly rent price, e.g.:

json

{
  "predicted_price": 423.5
}
Notes
Make sure the evler.csv file exists in data/raw/ before training the model.

This project uses a Random Forest model saved as model.joblib.

For API testing, you can use Swagger at http://127.0.0.1:8000/docs or Postman.

yaml

git commit -m "Update README with full project instructions"
git push
