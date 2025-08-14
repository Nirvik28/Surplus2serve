🍽️ Food Surplus Management – Backend
📌 Overview

This is the backend for the Food Surplus Management platform, designed to connect donors, NGOs, and volunteers to reduce food wastage.
Built with Python, Flask, and MySQL.

🚀 Features

User Authentication (Donor, NGO, Volunteer)

Food Listing & Requests

Real-time Status Updates

Database Integration with MySQL

REST API Endpoints for frontend integration

🛠️ Tech Stack

Backend Framework: Flask (Python)

Database: MySQL

Environment Management: venv

Other Tools: SQLAlchemy, Flask-RESTful, JWT Authentication

📂 Project Structure
backend/
│
├── app/                   # Application code
│   ├── __init__.py
│   ├── models/            # Database models
│   ├── routes/            # API endpoints
│   ├── utils/              # Helper functions
│   └── config.py          # App configuration
│
├── requirements.txt       # List of dependencies
├── .gitignore             # Ignored files (includes venv)
└── README.md              # Documentation

📦 Installation & Setup

1️⃣ Clone the repository

git clone https://github.com/yourusername/food-surplus-backend.git
cd food-surplus-backend


2️⃣ Create a virtual environment

python -m venv venv


3️⃣ Activate the virtual environment

Windows

venv\Scripts\activate


Mac/Linux

source venv/bin/activate


4️⃣ Install dependencies

pip install -r requirements.txt


5️⃣ Set up environment variables
Create a .env file in the root folder:

FLASK_APP=run.py
FLASK_ENV=development
DATABASE_URL=mysql+pymysql://username:password@localhost/food_surplus
SECRET_KEY=your_secret_key


6️⃣ Run the backend server

flask run

📡 API Endpoints (Examples)
Method	Endpoint	Description
POST	/auth/register	Register a new user
POST	/auth/login	Login and get token
GET	/food/list	Get all food items
POST	/food/add	Add new food listing
PUT	/food/update/:id	Update food listing
DELETE	/food/delete/:id	Delete food listing
📜 License

This project is licensed under the MIT License — you can freely modify and distribute it.
