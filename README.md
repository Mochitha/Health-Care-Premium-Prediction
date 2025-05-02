🏥 Health-Care Premium Prediction

This project predicts individual health insurance premium costs based on user inputs such as age, BMI, smoking status, number of children, and region. It is designed to provide real-time insights using a simple and interactive interface.

🔧 Features

Predicts health insurance premiums using a trained regression model

Streamlit-based web interface for easy interaction

Accepts key health and demographic inputs

Instant prediction results with a user-friendly UI

Deployed on Streamlit Cloud

🚀 Try the Live App

Click below to access the deployed Streamlit app:

👉 Launch the App

📁 Project Structure
 ```commandline
├── artifacts/                    # Directory for serialized models and scalers
│   ├── model_rest.joblib        # Model for the general population
│   ├── model_young.joblib       # Model for younger users
│   ├── scaler_rest.joblib       # Scaler for the general population
│   ├── scaler_young.joblib      # Scaler for younger users
├── .gitignore                   # Files to ignore in version control
├── LICENSE                      # License file
├── README.md                    # Project documentation
├── main.py                      # Main Streamlit app entry point
├── prediction_helper.py         # Helper script for prediction logic
└── requirements.txt             # Python dependencies
```
🛠️ Tech Stack

Python

Pandas, NumPy for data handling

Scikit-learn for model building

Streamlit for deployment and UI

Joblib for model serialization

📊 Model Info

To improve prediction accuracy, separate models and scalers were trained and saved based on user segmentation (e.g., young vs. rest). Linear regression techniques were used, and model performance was validated using standard regression metrics.

📌 How to Run Locally

Clone the repository:

git clone https://github.com/your-username/health-care-premium-prediction.git
cd health-care-premium-prediction

Install dependencies:
```bash
pip install -r requirements.txt
 ```
```commandline
Run the Streamlit app:

streamlit run main.py
```
📬 Feedback

Feel free to fork the repo, raise issues, or contribute to improve the project.
