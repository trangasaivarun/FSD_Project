# QuizMaster

QuizMaster is a dynamic and interactive quiz web application built with Python, Flask, and MySQL. It allows users to take quizzes, tracks scores, and provides an engaging platform for testing knowledge. The application features user authentication, a timer for quizzes, leaderboards, and an admin dashboard for managing quiz content and viewing analytics.

## Technologies Used
- **Backend:** Python, Flask, Flask-MySQLdb
- **Database:** MySQL
- **Frontend:** HTML5, CSS3, JavaScript
- **Additional:** Werkzeug for password hashing

## Features
- User registration and login
- Interactive quizzes with a timer
- Real-time score calculation and leaderboard
- Admin dashboard for adding, editing, and deleting questions
- Admin analytics and quiz review mode
- Modern, responsive, and visually appealing UI

## Setup Instructions

### Prerequisites
- Python 3.8+
- MySQL Server
- Git

### Installation
1. **Clone the repository:**
   ```bash
   git clone https://github.com/trangasaivarun/QuizMaster.git
   cd QuizMaster
   ```

2. **Set up the Database:**
   - Log in to your MySQL server.
   - Run the provided `schema.sql` file to create the `quiz_app` database and necessary tables.
     ```sql
     SOURCE /path/to/schema.sql;
     ```
   - Update the database credentials in `app.py` (e.g., `app.config['MYSQL_USER']`, `app.config['MYSQL_PASSWORD']`).

3. **Install Dependencies:**
   Create a virtual environment (optional but recommended) and install the required Python packages.
   ```bash
   pip install flask flask-mysqldb werkzeug
   ```

4. **Run the Application:**
   Start the Flask development server.
   ```bash
   python app.py
   ```
   The application will be accessible at `http://127.0.0.1:5000/`.

### Sample Questions
You can use the provided `sample_questions.txt` to quickly populate the database with some initial quiz content via the admin dashboard or by importing it directly if you write a script.
