🚀 Insurance Price Prediction





This project predicts insurance prices based on various factors such as age, sex, BMI, number of children, and smoking status. It uses TensorFlow for model training and Flask to serve the model via a web API.

📌 Features

Build and train a deep learning model using TensorFlow/Keras.

Use Flask to deploy the model as a REST API.

Accepts input parameters:

Age (numeric)

Sex (male/female)

BMI (Body Mass Index)

Children (number of dependents)

Smoker (yes/no)


Returns the predicted insurance price.


📂 Project Structure

insurance-price-prediction/
│── model/                    # Saved trained model
│── static/                    # Static files (CSS, JS)
│── templates/                 # HTML templates (if UI is added)
│── app.py                     # Flask API
│── model_training.ipynb        # Model training notebook
│── requirements.txt            # Dependencies
│── README.md                   # Documentation


🛠 Installation

⿡ Clone the repository

git clone https://github.com/your-username/insurance-price-prediction.git
cd insurance-price-prediction

⿢ Create a virtual environment (optional but recommended)

python -m venv venv
source venv/bin/activate   # On macOS/Linux
venv\Scripts\activate      # On Windows

⿣ Install dependencies

pip install -r requirements.txt

🎯 Model Training

1. Open model_training.ipynb in Google Colab or Jupyter Notebook.


2. Run the notebook to train the model using TensorFlow.


3. Save the trained model in the model/ directory.



🚀 Running the Flask API

Once the model is trained and saved, start the Flask server:

python app.py

The API will be available at http://127.0.0.1:5000/

📡 API Usage

🔹 Request (POST)

{
  "age": 30,
  "sex": "male",
  "bmi": 28.5,
  "children": 2,
  "smoker": "no"
}

🔹 Response

{
  "predicted_price": 14500.75
}

📊 Dataset

The dataset is taken from Kaggle's Medical Cost Personal Dataset, containing 1338 records with the following columns:

age (numeric)

sex (male/female)

bmi (numeric)

children (integer)

smoker (yes/no)

charges (insurance price)


🛠 Technologies Used

TensorFlow/Keras – Model Training

Flask – API Deployment

Pandas & NumPy – Data Handling

Scikit-learn – Preprocessing


📜 License

This project is open-source under the MIT License.

✨ Contributing

Feel free to fork the repo and contribute!



