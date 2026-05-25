##Python Fullstack Task2
Flask User Authentication System
A Python Fullstack Web Application built using Flask and SQLite database for secure user authentication.

##📋 Project Overview
This project is a simple User Authentication System developed using Flask.
The application allows users to:
  Register a new account
  Login securely
  Access Dashboard after login
  Logout from the session
The project demonstrates authentication flow, session management, and password security using Flask.

##Features Implemented
✅ User Registration System
✅ Secure User Login
✅ User Logout Functionality
✅ Session Management using Flask Sessions
✅ Password Hashing using Werkzeug Security
✅ Dashboard Access after Login
✅ SQLite Database Integration

##🛠️ Technologies Used
Technology	Purpose
Python	Backend logic
Flask	Web framework
SQLite	Database storage
HTML	Frontend structure
CSS	Styling and design
Werkzeug Security	Password hashing

##📁 Project Structure
python_fullstack_task2/
│
├── app.py                  → Flask backend logic
├── users.db                → SQLite database
│
├── templates/
│   ├── home.html           → Home page
│   ├── register.html       → Registration page
│   ├── login.html          → Login page
│   └── dashboard.html      → Dashboard page
│
└── README.md               → Project documentation

##▶️ How to Run
Step 1 - Clone the repository
git clone https://github.com/kavyatn089/python_fullstack_task2
Step 2 - Go into project folder
cd python_fullstack_task2
Step 3 - Install Flask
pip install flask werkzeug
Step 4 - Run the application
python app.py
Step 5 - Open in browser
http://127.0.0.1:5000

##🔄 Authentication Flow
User Registration
        ↓
Password gets hashed
        ↓
Data stored in SQLite database
        ↓
User Login with email & password
        ↓
Flask verifies credentials
        ↓
Session created successfully
        ↓
User redirected to Dashboard
        ↓
Logout removes session

##📸 Output Screenshots
✅ Registration Page
User enters username, email, and password.
✅ Login Page
User logs in using registered credentials.
✅ Dashboard
Displays welcome message after successful login.
✅ Logout
User session ends securely.

##📊 Sample User Data
ID	Username	Email
1	Kavya	kav@gmail.com
2	Rahul	rahul@gmail.com
3	Priya	priya@gmail.com

##🎯 Learning Outcomes
✅ Understanding Flask Authentication System
✅ Working with Sessions in Flask
✅ Password Security using Hashing
✅ Database Integration with SQLite
✅ Building Secure Web Applications

👩‍💻 Author
Kavya
GitHub: @kavyatn089

📅 Date
May 2026
