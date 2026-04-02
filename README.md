Finance Tracking Backend System

 Overview

This project is a Python-based backend application built using FastAPI. It allows users to manage financial transactions such as income and expenses and provides useful analytics.

##Features

* Create, Read, Delete transactions
* User login system
* Role-based access control (Admin, Analyst, Viewer)
* Financial summaries:

  * Total income
  * Total expense
  * Balance
* Category-wise analysis
* Monthly financial reports

---

## Tech Stack

* Python
* FastAPI
* SQLAlchemy
* SQLite
* Pydantic

---

## API Endpoints

### 👤 User

* POST `/users/` → Create user
* POST `/login/` → Login

### 💰 Transactions

* POST `/transactions/` → Add transaction
* GET `/transactions/` → View transactions
* DELETE `/transactions/{id}` → Delete transaction

### 📊 Analytics

* GET `/summary/` → Income, Expense, Balance
* GET `/category-summary/` → Category analysis
* GET `/monthly-summary/` → Monthly report

---

## ▶️ How to Run

### 🔹 Using Local Machine

1. Install dependencies:

   ```
   pip install fastapi uvicorn sqlalchemy pydantic
   ```

2. Run the server:

   ```
   uvicorn main:app --reload
   ```

3. Open in browser:

   ```
   http://127.0.0.1:8000/docs
   ```

---

### 🔹 Using Google Colab

* Run the notebook
* Open generated ngrok link
* Add `/docs` at the end

---

## 🌐 Deployment

This project was tested using ngrok in Google Colab for public API access.

---

## 🧠 Assumptions

* Simple authentication system without JWT
* Roles are passed manually in API requests
* SQLite used for simplicity

---

## 📌 Conclusion

This project demonstrates backend API design, CRUD operations, role-based access control, and financial data analysis using Python and FastAPI.

---

## 🙌 Author

Navaneetha
