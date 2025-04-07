# 🌸 Iris Flower Classification API

This is an end-to-end data science project that trains a machine learning model to classify iris flowers into species based on their sepal and petal measurements. The trained model is deployed using Flask as a REST API.

---

## 📁 Project Files

- `iris.csv` - Dataset used for training the model.
- `train_model.py` - Script to train the machine learning model.
- `model.pkl` - Trained machine learning model saved for reuse.
- `label_encoder.pkl` - Label encoder to convert species names.
- `app.py` - Flask app that serves the prediction API.
- `test_api.py` - Python script to test the API.
- `requirements.txt` - Python libraries required to run the project.
- `README.md` - Project documentation.

---

## ⚙️ How to Run the Project

### Step 1: Install Dependencies
Make sure you have Python installed. Then install the required libraries:

```bash
pip install -r requirements.txt
Step 2: Train the Model
Run the model training script:

bash
Copy
Edit
python train_model.py
This will generate model.pkl and label_encoder.pkl.

Step 3: Start the Flask API
Run the API:

bash
Copy
Edit
python app.py
The server will start at http://127.0.0.1:5000/

✅ How to Test the API
Option 1: Using Python (Recommended)
Run the test script:

bash
Copy
Edit
python test_api.py
You will see output like:

bash
Copy
Edit
Prediction: {'prediction': 'setosa'}
Option 2: Using Terminal (curl)
bash
Copy
Edit
curl -X POST http://127.0.0.1:5000/predict -H "Content-Type: application/json" \
-d '{"sepal_length": 5.1, "sepal_width": 3.5, "petal_length": 1.4, "petal_width": 0.2}'
📊 Dataset Info
This project uses the Iris dataset which contains 150 rows and 4 features:

Sepal Length

Sepal Width

Petal Length

Petal Width
Target: Species (setosa, versicolor, virginica)

🙋 About
Developed by Kartik Shripatre as part of a Data Science Internship (Task 3 - End-to-End Deployment).

vbnet
Copy
Edit

