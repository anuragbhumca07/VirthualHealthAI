# VirthualHealthAI
Virtual Health AI is a prediction system that analyzes both monthly clinical data and daily vitals to assess risks for four key health conditions: diabetes, heart disease, sleep apnea, and hypertension.

PowerShell commands for both the models.
uvicorn main1:app --reload --host 127.0.0.1 --port 8000
uvicorn main2:app --reload --host 127.0.0.1 --port 8000

Sample input for both the FastAPI.


{
  "fasting_glucose": 110.0,
  "cholesterol": 215.0,
  "hba1c": 6.2,
  "hdl": 45.0,
  "ldl": 130.0,
  "triglycerides": 180.0,
  "vitamin_d": 22.5,
  "vitamin_b12": 350.0,
  "iron": 75.0,
  "hemoglobin": 13.8,
  "rbc_count": 4.7,
  "wbc_count": 6200.0,
  "platelet_count": 240000.0,
  "tsh": 3.1,
  "t3": 1.3,
  "t4": 7.8,
  "family_history": 1,
  "smoking": 0
}


{
  "pulse": 72,
  "systolic_bp": 120,
  "diastolic_bp": 80,
  "spo2": 97,
  "body_temp": 98.4,
  "calories_burned": 250,
  "steps": 5000,
  "stress_level": 3,
  "hrv": 55,
  "label_diabetes": 0.45,
  "label_heart": 0.3,
  "label_sleep_apnea": 0.2,
  "label_hypertension": 0.15
}
