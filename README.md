# 🏥 Insurance Premium Category Predictor

A **Machine Learning + FastAPI + Streamlit** project that predicts a person’s **insurance premium category** based on lifestyle and demographic factors.

---

## 🚀 Tech Stack
- **Machine Learning** – Model for insurance premium prediction
- **FastAPI** – Backend REST API for model inference
- **Streamlit** – Interactive frontend for user input and results visualization
- **Requests** – API communication between frontend and backend

---

## 📌 Features
- Input user details such as **age, weight, height, income, smoker status, city, and occupation**
- Get predictions for **insurance premium category** (e.g., Low / Medium / High)
- Optionally view **confidence score** and **class probabilities** (if provided by backend)
- Clean and simple **Streamlit web interface**
- Backend served via **FastAPI endpoint** (`/predict`)

---

## ⚡ How It Works
1. User enters details in the **Streamlit frontend**
2. Data is sent to the **FastAPI backend** (`/predict`)
3. Machine Learning model processes the input and returns predictions
4. Results are displayed with category (and confidence/probabilities if available)

---

## 🛠️ Setup & Run

### 1. Clone the repository
```bash
git clone https://github.com/your-username/insurance-premium-predictor.git
cd insurance-premium-predictor
```

### 2. Create Virtual Environment & Install Dependencies
```bash
python -m venv env

# Activate the environment
# On Mac/Linux:
source env/bin/activate

# On Windows:
env\Scripts\activate

# Install required packages
pip install -r requirements.txt
```
### 3. Run FastAPI Backend
```bash
uvicorn api:app --reload
```

### 4. Run Streamlit Frontend
```bash
streamlit run frontend.py
```
Streamlit will open a local web interface (usually at http://localhost:8501)

## ⚠️ Disclaimer

This project is for **learning and demonstration purposes only**.  

- The data used is **synthetic or hypothetical**.  
- The insurance premium predictions are **not real** and **should not be used for actual financial or medical decisions**.  
- This project is intended to **practice machine learning, FastAPI, and Streamlit integration**.
