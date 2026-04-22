# ⚡ Who's Next | Employee Attrition Analytics

Who's Next is a premium HR Analytics platform designed to help organizations proactively identify and mitigate employee attrition risk. By combining machine learning predictions with AI-driven insights, the platform provides managers with actionable strategies to retain top talent.

---

## 🔗 Live Application
- **Frontend (Live):** [https://who-s-next-three.vercel.app](https://who-s-next-three.vercel.app) *(Replace with your actual Vercel URL)*
- **Backend API:** [https://who-s-next.onrender.com](https://who-s-next.onrender.com)

---

## 🚀 Key Features

- **Predictive Attrition Modeling**: Real-time risk probability scoring using an ensemble of Machine Learning models (Random Forest, Logistic Regression, Gradient Boosting).
- **Risk Driver Analysis**: Automatic identification of the primary factors contributing to an employee's flight risk (e.g., Overtime, Income discrepancy, Job Satisfaction).
- **AI-Powered Recommendations**: Integration with **Google Gemini 2.5 Flash** to provide highly specific, actionable retention strategies tailored to each employee's profile.
- **Interactive Dashboard**: A modern React-based interface for filtering and exploring workforce data by department, job role, and risk level.
- **"What-If" Analysis**: Simulate changes to employee factors (like salary increases or overtime reduction) to see immediate impacts on their risk score.

---

## 🛠️ Tech Stack

### Backend
- **Framework**: FastAPI (Python 3.12+)
- **Machine Learning**: Scikit-learn, Pandas, NumPy
- **Model Persistence**: Joblib
- **AI Integration**: Google GenAI (Gemini 2.5 Flash)

### Frontend
- **Framework**: React JS (Vite)
- **Styling**: Tailwind CSS
- **Icons/UI**: Lucide React, Recharts

---

## ⚙️ Setup & Installation

### 1. Backend Setup
Navigate to the `backend` directory:
```bash
cd Who-s-Next-main/backend
```
Install dependencies:
```bash
pip install -r requirements.txt
```
Create a `.env` file:
```env
GEMINI_API_KEY=your_google_gemini_api_key
```

### 2. Frontend Setup
Navigate to the `frontend` directory:
```bash
cd Who-s-Next-main/frontend
```
Install dependencies:
```bash
npm install
```
Create a `.env` file:
```env
VITE_API_URL=http://localhost:8000
```

---

## 🏃 How to Run Locally

### Start the Backend
```bash
uvicorn main:app --reload --port 8000
```

### Start the Frontend
```bash
npm run dev
```

---

## 📊 Data Source
The project utilizes the **IBM HR Analytics Employee Attrition & Performance** dataset, which includes features such as employee demographics, job involvement, and satisfaction levels.
