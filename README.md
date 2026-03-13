🌐 IPL Analytics Web Application

A Flask-based web application that consumes the IPL Analytics REST API and provides a simple interactive interface to explore team head-to-head statistics.

The application allows users to select two IPL teams and view their historical match record comparison using data provided by the backend API.

This project demonstrates API consumption, Flask web development, and integration of frontend templates with backend services.

🚀 Features

🏏 Interactive team vs team comparison
🌐 Web interface built with Flask and Jinja2 templates
🔗 Integration with an external REST API
📊 Dynamic dropdown selection of IPL teams
⚡ Real-time API requests using the requests library
📦 Clean HTML rendering of API responses

🧠 What This Project Demonstrates

This project highlights the following backend and integration skills:

API consumption using Python requests
Flask-based web application development
Dynamic HTML rendering with Jinja2 templates
Handling API errors and request failures
Client–server architecture using REST APIs
Integration between frontend UI and backend analytics services

📂 Project Structure
api_use/
│
├── app.py                # Flask web application
│
├── templates/
│     └── index.html      # Web interface template
│
├── requirements.txt      # Project dependencies
│
├── .gitignore
├── LICENSE
└── README.md
⚙️ Architecture Overview

The project works as a client application that consumes the IPL Analytics API.

User Browser
      │
      ▼
Flask Web Application
(app.py)
      │
      │ HTTP Requests
      ▼
IPL Analytics REST API
(http://127.0.0.1:5000)
      │
      ▼
Analytics Engine
(team_stats / player_stats)
      │
      ▼
IPL Datasets
Design Principles

Separation between UI layer and analytics layer
Use of external REST API for data retrieval
Lightweight and simple frontend interface
Clear client–server architecture

🔌 Application Workflow

1️⃣ The web application requests the list of IPL teams from the API

GET /api/teams

2️⃣ Teams are displayed in dropdown menus.

3️⃣ The user selects two teams.

4️⃣ The application sends a request to the backend API:

GET /api/teamvteam

5️⃣ The API response is rendered in the browser.

📊 Example User Flow
Step 1 — Open Application
http://127.0.0.1:7000
Step 2 — Select Teams
Team 1 → Chennai Super Kings
Team 2 → Delhi Daredevils
Step 3 — View Result

Example output:

total_matches: 25
Chennai Super Kings: 15
Delhi Daredevils: 10
draws: 0
🛠 Installation
Clone repository
git clone https://github.com/RudrTyagi1135/api_use.git
cd api_use
Install dependencies
pip install -r requirements.txt
Run the application
python app.py

Server will start at:

http://127.0.0.1:7000
⚠️ Important Requirement

This web application depends on the IPL Analytics API.

Before running this project, ensure the API server is running.

Start the API service:

cd IPL_API_FLASK
python app.py

The API will run at:

http://127.0.0.1:5000
🧪 Example API Calls Used

Get Teams

http://127.0.0.1:5000/api/teams

Team vs Team Record

http://127.0.0.1:5000/api/teamvteam?team1=Mumbai Indians&team2=Chennai Super Kings
📈 Potential Improvements

Future enhancements could include:

Team overall record interface
Batsman analytics dashboard
Bowler analytics dashboard
Interactive charts for team statistics
Frontend styling with Bootstrap
Deployment of frontend and API services
Docker containerization
Authentication and user sessions

🧰 Tech Stack
Technology	Purpose
Python	Programming language
Flask	Web framework
Jinja2	HTML template rendering
Requests	API communication
HTML	Web interface
JSON	API response format
🎯 Learning Outcomes

This project helped build understanding of:

REST API integration in web applications
Client–server architecture
Flask templating with Jinja2
Handling HTTP requests and responses
Building frontend interfaces for backend analytics systems

👤 Author

Rudra

B.Tech Final Year Student
Aspiring MLOps Engineer