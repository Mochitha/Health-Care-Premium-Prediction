<div align="center">
  <img src="https://github.com/user-attachments/assets/60df1e6f-76d3-4648-83e6-833bc5ae45de" width="500"/>
</div>

This project uses  regression models to predict individual health insurance premiums based on inputs like age, BMI, smoking status, dependents, region, etc. Built with Streamlit, it offers a clean, interactive UI for real-time predictions and is deployed on Streamlit Cloud.

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

To improve prediction accuracy, separate models and scalers were trained and saved based on user segmentation (e.g., young vs. rest). Linear Regressor model is used for the young category, and XGBoost Regressor for the rest, and model performance was validated using standard regression metrics.

⚡ Quick Start

## Setup Instructions

1. Clone the repository:
```bash
git clone https://github.com/Mochitha/health-care-premium-prediction.git
cd health-care-premium-prediction
 ```
2. Install dependencies:
```commandline
pip install -r requirements.txt
 ```

3. Run the Streamlit app:
```commandline
streamlit run main.py
```
📬 Feedback

Feel free to fork the repo, raise issues, or contribute to improve the project.
