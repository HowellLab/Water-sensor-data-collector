

## Table of Contents
1. [Requirements](#requirements)
2. [Project Structure](#project-structure)
3. [Initial Setup](#initial-setup)
4. [Running the Backend (Python)](#running-the-backend-python)
5. [Running the Frontend (React)](#running-the-frontend-react)
6. [Accessing the Application](#accessing-the-application)
7. [Troubleshooting](#troubleshooting)

---

## Requirements
- **Python 3.10+**
- **Node.js 18+** and **npm**
- **Git** 

Instruction for instalation can be found on the following website
- [Python](https://www.python.org/downloads/)
- [Node.js](https://docs.npmjs.com/downloading-and-installing-node-js-and-npm)
- [Git](https://git-scm.com/book/ms/v2/Getting-Started-Installing-Git)
- [MongoDB](https://www.mongodb.com/try/download/community-kubernetes-operator)
- [MongoDB Tools](https://www.mongodb.com/try/download/database-tools)
  - Make sure that you add this to your PATH so you can call this library

-If something is not working, closing the terminal window and opening it back up will sometimes fix it
-Also, the following commands are set for Windows macines, Linux and macOS machines will follow the same commands, however, they may be slightly different. ChatGPT would be a good reasource for command conversions.

---

## Project Structure
- `research-backend/` — Python backend
- `src/` — React frontend
- `public/` — Static files for frontend
- `requirements.txt` — Python dependencies
- `package.json` — Node.js dependencies

---

## Initial Setup

### 1. Open Terminal
-Open up your terminal either inside your IDE (VSCode, Vim, IntelliJ, etc) or outside of it

### 2. Navigate to the Project Folder
-Using the `cd` command, navigate to where you would like the project to live
-Example: `cd HowellLab/Desktop/Github Repos`

### 3. Getting The Project on Your Machine
-Run th command `git clone https://github.com/HowellLab/Water-Sensor.git` inside your terminal
-This will put all of the code onto your machine 

### 4. Install Python Dependencies
-Run these commands individually inside your newly cloned repository
```
cd research-backend
python -m venv .venv
.\.venv\Scripts\activate
python -m pip install -r requirements.txt
```
-This will put all of the dependincies inside your virtual enviroment so that the program can run smoothly
-If you are using an IDE such as VSCode, you will see a .venv folder appead on the left side of your screen

### 5. Install Node.js Dependencies
-Now run each of these commands individually
```
cd ..
npm install
```
This will install of the Node.js dependincies needed to run the program
---

### 6. Getting Database Setup
-Run the command `mongostore --db Rainbows_DB ./db-dump/myappdb`
This will set up the database so that everything runs. 

## Getting the program Running
1. Now that you are inside your virtual enviorment (a little (.venv) should appear in your terminal), run the following commands
-You will need to make sure that you are inside the virtual enviorment each time you want to run the program. Do this by running `.\.venv\Scripts\activate`
```
cd research-backend
python app.py
```
- The backend server should start, usually on `http://127.0.0.1:5000` or similar.

---

2. Now open up a new terminal and type the following commands one at a time
```
cd ..
cd src
npm start
```
- This will start the React app, usually on `http://localhost:3000`. This should also automatically open up and window on your machine, but it might not

---

## Accessing the Application
- Open your web browser (Safari, Chrome, etc.).
- Go to: [http://localhost:3000](http://localhost:3000)
- You should see the application homepage.
- A base username name and password that comes pre instaled is 
-- Username: test2
-- Password: pass
---

## Troubleshooting
- **If you see errors about missing packages:**
  - For Python: Run `pip install -r requirements.txt` again.
  - For Node.js: Run `npm install` again.
- **If a port is already in use:**
  - Try closing other apps or restarting your computer.
- **If you see `ModuleNotFoundError` in Python:**
  - Make sure you activated the virtual environment: `source venv/bin/activate`
- **If you see `command not found: npm` or `node`:**
  - Install Node.js from [https://nodejs.org/](https://nodejs.org/)
- **If you see `command not found: python3`:**
  - Install Python 3 from [https://www.python.org/downloads/](https://www.python.org/downloads/)

---

## Additional Notes
- Always keep the two terminals running for the durration of time you want to use the program.
- To stop a running server, press `Ctrl + C` in both pf the terminal.
- If you make code changes, restart the affected server (backend or frontend).



# Getting Started with Create React App

This project was bootstrapped with [Create React App](https://github.com/facebook/create-react-app).

## Available Scripts

In the project directory, you can run:

### `npm start`

Runs the app in the development mode.\
Open [http://localhost:3000](http://localhost:3000) to view it in your browser.

The page will reload when you make changes.\
You may also see any lint errors in the console.

### `npm test`

Launches the test runner in the interactive watch mode.\
See the section about [running tests](https://facebook.github.io/create-react-app/docs/running-tests) for more information.


