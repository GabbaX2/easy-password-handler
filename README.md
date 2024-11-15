Password Generator and Manager

This project is a Flask-based web application for securely generating, storing, and managing passwords. It provides an intuitive interface for users to create strong passwords, save them securely, and manage their saved passwords.

About the Author

Hi! My name is Gabriella, and I am a student currently learning to use Python, Flask, and databases. This project is part of my learning journey to improve my skills in web development and backend programming. If you have any suggestions or feedback, I’d love to hear from you!

Features

1. Password Generator

	•	Generates random passwords with a customizable length.
	•	Supports uppercase letters, lowercase letters, and digits.

2. Password Storage

	•	Stores generated passwords in an SQLite database with the associated account name and timestamp.
	•	Automatically creates the database table (passwords) if it does not exist.

3. Password Management

	•	View all saved passwords in a structured table.
	•	Update a saved password with a new randomly generated one.
	•	Delete saved passwords if no longer needed.

4. Responsive Design

	•	Fully responsive, with a modern, user-friendly interface styled using TailwindCSS and DaisyUI.

5. Dark Mode Support

	•	Adapts to the user’s preferred theme for improved usability.

Installation and Setup

1. Prerequisites

	•	Python 3.x installed
	•	Flask installed (pip install flask)
	•	SQLite (pre-installed with Python)

2. Clone the Repository

git clone https://github.com/your-username/password-manager.git
cd password-manager

3. Install Dependencies

Ensure you have Flask installed:

pip install flask

4. Run the Application

Start the Flask development server:

python app.py

Access the application at http://127.0.0.1:5000/.

Project Structure

password-manager/
├── app.py                # Main Flask application
├── templates/            # HTML templates
│   ├── index.html        # Password generator page
│   ├── view_passwords.html # Saved passwords management page
├── static/               # Static assets (optional)
│   └── css/              # Custom CSS (if needed)
├── passwords.db          # SQLite database (auto-generated)
└── README.md             # Project documentation

Usage

Generate a Password

	1.	Open the app at http://127.0.0.1:5000/.
	2.	Enter the desired password length and associated account name.
	3.	Click Generate Password to create a random password.
	4.	Optionally, click Copy to copy the password to your clipboard.

View and Manage Saved Passwords

	1.	Click View Saved Passwords to access all saved passwords.
	2.	Use the Update button to generate and save a new password for an account.
	3.	Use the Delete button to remove a password from the database.

Security Considerations

	•	Passwords are stored in plain text in the SQLite database. For better security, consider hashing or encrypting passwords before storage.
	•	Ensure the app is deployed securely in production with HTTPS and proper Flask configurations.

Dependencies

	•	Flask: pip install flask
	•	SQLite: Pre-installed with Python
	•	TailwindCSS: Included via CDN
	•	DaisyUI: Included via CDN

Future Improvements

	•	Add user authentication for additional security.
	•	Implement encryption for stored passwords.
	•	Add a feature to customize password complexity (special characters, etc.).

Author: Gabba


