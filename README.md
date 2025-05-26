# JS-HTML-Project-1

Here’s a detailed README.md file you can include with your project:

⸻

🔐 User Validation Webpage

This is a simple user validation webpage built with HTML and JavaScript. The application prompts the user for login credentials (username and password), validates the input, checks them against a pre-defined user store, and displays user details if the credentials are correct.

⸻

📄 Table of Contents
	•	Features
	•	How It Works
	•	Technologies Used
	•	File Structure
	•	Setup Instructions
	•	Code Walkthrough
	•	Improvements

⸻

✅ Features
	•	Prompts the user for:
	•	Username
	•	Password
	•	Password confirmation
	•	Validates:
	•	Username length (must be less than 10 characters)
	•	Password length (must be between 6 and 15 characters)
	•	Matching password confirmation
	•	Checks the credentials against a static userStore object.
	•	Displays the user’s first name, last name, email, and profession if the login is successful.
	•	Shows appropriate alerts for invalid input or login failure.

⸻

💡 How It Works
	1.	When the webpage loads, it displays an alert: Welcome!
	2.	The getUserDetails() function is triggered to collect and validate user credentials.
	3.	The function:
	•	Validates that the username is less than 10 characters.
	•	Validates the password length (between 6 and 15 characters).
	•	Ensures the user confirms the password correctly.
	4.	If the provided username exists in the userStore and the password matches, user details are shown in an alert.
	5.	If validation or matching fails, appropriate alerts are displayed.

⸻

🧰 Technologies Used
	•	HTML5 for the webpage structure.
	•	Vanilla JavaScript for logic and user interaction.
	•	Browser prompts and alerts for user input/output.

⸻

📁 File Structure

project/
│
├── index.html       # Main HTML page
├── index.js         # JavaScript file with user logic
└── README.md        # This file


⸻

🛠️ Setup Instructions

To run this project:
	1.	Clone or download the repository.
	2.	Open the index.html file in a web browser.
	3.	Follow the prompts that appear on your screen.

No additional setup or dependencies are required.

⸻

🧾 Code Walkthrough

index.html

<script src="index.js" defer></script>

Links the JavaScript file to the HTML and ensures the script runs after the page loads.

userStore

const userStore = {
  "Qweci": {
    firstName: "Qweci",
    ...
  },
  ...
}

A mock database that stores user credentials and details.

getUserDetails()
	•	Handles all logic for user input, validation, and feedback.
	•	Uses prompts to collect input.
	•	Displays errors and success messages using alert().

Validation Functions

function validateUsername(username) { ... }
function validatePassword(password) { ... }

These ensure that input meets basic constraints.

⸻

🚀 Example Users

You can log in using the following credentials:

Username	Password	First Name	Last Name	Email	Profession
Qweci	12345Ada	Qweci	Paul	Qwecipaul@mail.com	Computer programmer
jemima	12345Yemi	jemima	Amoah	jemimaAmoah12@gmail.com	Software Engineer


⸻

🌱 Possible Improvements
	•	Add registration functionality to allow new users.
	•	Store users in local storage or connect to a backend.
	•	Replace prompt and alert with proper HTML forms and styled UI.
	•	Add better password validation (e.g., include numbers, symbols, etc.).
	•	Add error display inside the webpage instead of using alert().

⸻

📬 Feedback

If you find bugs or have suggestions for improvements, feel free to open an issue or submit a pull request!

⸻

Made with ❤️ using JavaScript.

⸻
