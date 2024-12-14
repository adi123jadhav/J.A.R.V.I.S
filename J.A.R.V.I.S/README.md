# JARVIS AI CHATBOT
#### Video Demo:  <URL HERE>
#### Description:
This Project is a chatbot names Jarvis inspired from the Marvel Universe .This is our take on new craze of Genarative AI and Machine Learning .We wanted to make this project to learn about these new booming technologies of the Industry .In this project We tried to keep the UI as minimal as possible with a simple login and a register page.

---

## Features

- **User Authentication:** Lets the User register and log in securely and smoothly.
- **Interactive Chat:** Lets the User chat with Jarvan in a dynamic and responsive interface.
- **Personalized Sessions:** The User's conversations are maintained in real-time with different sessions which starts a new session each time the User logout.


## Getting Started

### Prerequisites

1. **Install Python 3.10 or later.**
2. **Install the Required Libraries:**
    Run the following command to install dependencies:
   ```bash
    pip install -r requirements. txt
   ```
   
3. *Set Up Your API Keys:*
   - LANGCHAIN_API_KEY: Your LangChain API key.
   - GOOGLE_API_KEY: Your Google Cloud API key.


### Database Initialization

Set up the SQLite database to store user data:
```
sqlite3 user.db
```

Ensure your schema.sql file includes:
```
sql
CREATE TABLE IF NOT EXISTS user (
    id INTEGER PRIMARY KEY AUTOINCREMENT,
    username TEXT NOT NULL UNIQUE,
    hash TEXT NOT NULL
);
```

### Running the Application

To start the application, run:
```bash
python app.py
```
Open your browser and navigate to [http://127.0.0.1:5000](http://127.0.0.1:5000) to use Elexa.

---

## API Key Configuration

Add your API keys to a `.env` file or set them directly in your terminal:
```bash
export GOOGLE_API_KEY="your-google-api-key"
```
This key enable the Jarvis to interact with Google Generative AI.

---
## Project Structure

Here’s an overview of the project files and their purposes:

```
├── app.py             # Main application logic
├── templates
│   ├── index.html    # Chat interface
│   ├── login.html    # Login page
│   ├── register.html # Registration page
│   ├── error.html    # Error page 
├── static
│   ├── style.css      # Styling for the index.html
    ├── style.css      # Styling for the login.html,register.html,error.html
│   ├── script.js      # Client-side functionality
├── user.db            # SQLite database
├── requirements.txt   # Requirements of this project
└── README.md          # Project documentation
```

---


### Explanation of Key Files

- **app.py:** The main file that contains the Flask  and application logic and integration with APIs.
- **index.html:** Hosts the chat interface, allowing users to interact with Jarvan.
- **login.html:** Provide user login functionality.
- **register.html:** Provide user registration functionality.
- **error.html:** This page shows the error when something goes wrong.
- **style.css:** Adds custom styles to enhance the user interface.
- **script.js:** Implements client-side interactivity for good chat operations.
- **user.db:** SQLite database file to store user credentials securely.
- **requirements.txt:** Lists all necessary Python libraries need to run this project.

---

## Requirements File

The `requirements.txt` file lists all the Python libraries needed for this project. Install them with:
```
pip install -r requirements.txt
```

Contents of `requirements.txt`:
```
flask
flask-session
cs50
langchain_core
langchain_google_genai
```

---

## How to Use

1. **Register or Log In:** Use the provided forms to aaccess the chating feature.
2. **Start Chatting:** Type a message and click the "send" button to chat  with Jarvan.
3. **Log Out:** End your session with the logout button.

---

## Technologies Used

This project usses a variety of technologies :

### Backend Technologies

- **Flask Framework:** A lightweight web framework for Python, used to manage the server-side logic, route requests, and handle API integrations.
- **LangChain:** A library used for building applications with llms,to facilitate context-aware, intelligent chatbot responses.
- **Google Generative AI:** We used gemini-1.5-flash for this project to give correct replies to the user queries.
- **SQLite:** A lightweight and efficient database solution for managing user authentication and session data.

### Frontend Technologies

- **HTML:** It is used to give the webpages the content of the application, including forms, chat interfaces, and navigation elements.
- **CSS:** It is used to Enhance the aesthetic appeal with:
  - *Background Gradients:* it is to ensure smooth and visually appealing gradients across the layout.
  - *Chat Bubble Styling:* it is to ensure distinguish the user and bot messages, thus improving readability.
  - *Responsive Layouts:* It Ensures the interface adapts to different screen sizes and devices easily.
- **JavaScript:** It is used to add interactivity, such as dynamically appending chat messages and handling user input.

### Supporting Tools and APIs

- **Python Environment:** Facilitates development and testing with its extensive ecosystem of libraries.
- **Google API:** Powers the Jarvan's advanced language understanding capabilities.
- **Flask-Session:** Manages user sessions .

---