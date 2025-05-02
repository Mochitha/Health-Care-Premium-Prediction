<img src="https://github.com/user-attachments/assets/24c99565-2599-469c-948d-4d88c3d6fc28" width="400"/>

This project predicts individual health insurance premium costs based on user inputs such as age, BMI, smoking status, number of dependents, region, etc. It is designed to provide real-time insights using a simple and interactive interface.

🔧 Features

Predicts health insurance premiums using a trained regression model

Streamlit-based web interface for easy interaction

Accepts key health and demographic inputs

Instant prediction results with a user-friendly UI

Deployed on Streamlit Cloud

🚀 Try the Live App

Click below to access the deployed Streamlit app: 

👉 Launch the App https://health-care-premium-prediction.streamlit.app/

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

📊 Model Info

To improve prediction accuracy, separate models and scalers were trained and saved based on user segmentation (e.g., young vs. rest). Linear regression techniques were used, and model performance was validated using standard regression metrics.

⚡ Quick Start

## Setup Instructions

Clone the repository:
```bash
git clone https://github.com/Mochitha/health-care-premium-prediction.git
cd health-care-premium-prediction
 ```
Install dependencies:
```commandline
pip install -r requirements.txt
 ```

Run the Streamlit app:
```commandline
streamlit run main.py
```
📬 Feedback

Feel free to fork the repo, raise issues, or contribute to improve the project.
