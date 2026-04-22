# ⚡ Who's Next | Employee Attrition Analytics

Who's Next is a premium HR Analytics platform designed to help organizations proactively identify and mitigate employee attrition risk. By combining machine learning predictions with AI-driven insights, the platform provides managers with actionable strategies to retain top talent.

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
- **Framework**: FastAPI (Python 3.12)
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
cd backend
```
Install the required Python packages:
```bash
pip install fastapi uvicorn pandas numpy scikit-learn joblib google-genai python-dotenv
```

Create a `.env` file in the `backend` folder and add your Gemini API Key:
```env
GEMINI_API_KEY=your_google_gemini_api_key
```

### 2. Frontend Setup
Navigate to the `frontend` directory:
```bash
cd frontend
```
Install the dependencies:
```bash
npm install
```

---

## 🏃 How to Run

### Start the Backend
From the `backend` folder:
```bash
uvicorn main:app --reload --port 8000
```
The API will be available at `http://localhost:8000`. You can view the interactive documentation at `http://localhost:8000/docs`.

### Start the Frontend
From the `frontend` folder:
```bash
npm run dev
```
The application will be accessible at `http://localhost:5173`.

---

## 📊 Data Source
The project utilizes the **IBM HR Analytics Employee Attrition & Performance** dataset (`WA_Fn-UseC_-HR-Employee-Attrition.csv`), which includes features such as employee demographics, job involvement, and satisfaction levels.

---

## 🤖 AI Recommendations
The system uses the **Gemini 2.5 Flash** model to analyze ML risk drivers and generate 3-4 professional recommendations for managers. This bridge between "data" and "action" is the core value proposition of Who's Next.
