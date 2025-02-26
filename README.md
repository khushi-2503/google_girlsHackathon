# **Tax Assistant Web Application**

## **Overview**
The **TaxWise** is a Flask-based platform designed to help users manage their taxes efficiently. The app offers features like **Form 16 to Excel conversion, tax scenario simulation, AI-powered tax recommendations, investment portfolio suggestions, and tax alerts.**

## **Features**

### 📄 **Form 16 to Excel Conversion**
- Upload a **Form 16 PDF**
- Extracts text using OCR (Tesseract)
- Generates an **editable Excel file** for tax computation

### 📊 **Tax Scenario Simulation**
- Predicts future income, expenses, and tax liabilities over a given number of years
- Displays **a visual tax forecast graph**

### 🔎 **Tax Bracket Monitoring**
- Analyzes income and expenses from financial transactions
- Alerts users about **upcoming tax bracket changes**

### 💡 **AI-Powered Tax Recommendations**
- Uses **Groq AI (Mixtral-8x7b-32768)** to suggest **tax-saving investments**
- Personalized recommendations based on user income and deductions

### 🌱 **Eco-Friendly Tax Savings**
- Fetches **sustainable investment opportunities** via API
- Suggests tax-saving investments based on eco-friendly projects

### 🛎 **Tax Alerts & Regulatory Updates**
- Fetches latest **tax law changes** using AI
- Displays **important tax filing deadlines**

### 📈 **Tax Dashboard**
- Computes **taxable income, tax liability, and potential savings**
- Helps users optimize deductions and investments

### 💼 **AI-Powered Investment Portfolio**
- Generates a **tax-optimized investment plan** based on risk tolerance

## **Installation**

### **Step 1: Clone the Repository**
```sh
git clone https://github.com/your-repo/tax-assistant.git
cd tax-assistant
```

### **Step 2: Set Up a Virtual Environment**
```sh
python -m venv venv
source venv/bin/activate   # On macOS/Linux
venv\Scripts\activate     # On Windows
```

### **Step 3: Install Dependencies**
```sh
pip install -r requirements.txt
```

### **Step 4: Run the Application**
```sh
python app.py
```
- The app runs on **http://127.0.0.1:5000/**

## **API Endpoints**

### 📂 **File Upload & Extraction**
#### `POST /upload`
- Uploads **Form 16 PDF**
- Returns a link to download extracted **Excel file**

### 📊 **Tax Simulation**
#### `POST /simulate_tax_scenario`
- Accepts `income`, `expenses`, `investments`, and `years`
- Returns a **graph predicting future tax liabilities**

### 📡 **Tax Bracket Monitoring**
#### `POST /monitor_tax_bracket`
- Monitors **income vs. expenses**
- Returns an **alert if user is near a new tax bracket**

### 🧠 **AI-Powered Tax Recommendations**
#### `POST /tax_saving_recommendations`
- Accepts `income` and `deductions`
- Returns **personalized investment suggestions**

### 🌱 **Eco-Friendly Tax Savings**
#### `POST /eco_tax_savings`
- Fetches **green investment options**
- Returns tax savings **based on sustainable projects**

### 🔔 **Tax Alerts**
#### `GET /tax_alerts`
- Returns **upcoming tax deadlines** & **latest regulatory changes**

### 📊 **Tax Dashboard**
#### `POST /tax_dashboard`
- Computes **taxable income, liability, and savings**
- Returns a structured financial summary

### 💼 **Investment Portfolio**
#### `POST /investment_portfolio`
- Accepts `income` & `risk_tolerance`
- Returns a **customized investment portfolio**

## **Future Enhancements**
✅ **Gmail API Integration** – Auto-fetch Form 16 from emails
✅ **Conversational Tax AI Chatbot**
✅ **Real-time Tax Score & Monthly Reports**
✅ **Dark Mode & Enhanced UI/UX**



