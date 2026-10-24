# 👨‍💼 Employee Management System

A simple and user-friendly **Employee Management System** built using React.js. This web application helps users manage employee information through an interactive interface that supports viewing, adding, updating, deleting, and searching employee records.

🌐 **Live Demo:** [Employee Management System](https://employeemanagement-0n2q.onrender.com)

---

## 📌 Table of Contents

* [Project Overview](#-project-overview)
* [Purpose of the Project](#-purpose-of-the-project)
* [Features](#-features)
* [Technologies Used](#-technologies-used)
* [How the Application Works](#-how-the-application-works)
* [Project Structure](#-project-structure)
* [Prerequisites](#-prerequisites)
* [Installation and Setup](#-installation-and-setup)
* [Running the Application](#-running-the-application)
* [Available Routes](#-available-routes)
* [Deployment](#-deployment)
* [Current Limitations](#-current-limitations)
* [Future Enhancements](#-future-enhancements)
* [Author](#-author)

---

## 📖 Project Overview

The Employee Management System is a React-based web application designed to simplify basic employee information management.

The application provides a straightforward interface for displaying employee records and performing common employee management operations. It is suitable as a beginner-friendly project for learning React.js, component-based development, state management, and client-side routing.

The application is deployed on Render and can be accessed through a web browser.

## 🎯 Purpose of the Project

Managing employee information manually can be time-consuming. This project demonstrates how a web application can make basic employee record management easier.

The main objectives are to:

* Display employee information in an organized format.
* Add new employee records.
* Update existing employee details.
* Delete employee records.
* Search for employees.
* Provide a simple and accessible user interface.
* Demonstrate React.js development and deployment.

## ✨ Features

### 1. Employee List

Displays employee records, including their ID, name, email, phone number, department, and designation.

### 2. Add Employee

Allows users to enter employee details and add a new record to the list.

### 3. Update Employee

Provides a page for modifying the details of an existing employee.

### 4. Delete Employee

Allows users to remove an employee record from the displayed list.

### 5. Search Employee

Provides a dedicated page for searching employee records.

### 6. Client-Side Navigation

Uses React Router to navigate between the employee list, add employee, update employee, and search pages.

### 7. Web-Based Interface

Can be accessed through a compatible web browser without requiring users to install the application locally.

---

## 🛠️ Technologies Used

| Technology     | Purpose                                       |
| -------------- | --------------------------------------------- |
| React.js       | Building the user interface                   |
| JavaScript     | Application logic and functionality           |
| HTML5          | Structuring the web application               |
| CSS3           | Styling and layout                            |
| React Router   | Navigation between pages                      |
| Node.js        | JavaScript runtime used for development tools |
| npm            | Installing dependencies and running scripts   |
| Git and GitHub | Version control and source code hosting       |
| Render         | Hosting the deployed web application          |

---

## ⚙️ How the Application Works

The application is built using reusable React components.

1. The **Employee List** component displays the available employee records.
2. The **Add Employee** component collects information for a new employee.
3. The **Employee Profile Update** component allows existing employee details to be edited.
4. The **Employee Search** component provides the employee search interface.
5. React state manages the employee records while the application is running.
6. React Router manages navigation between the application's pages.

**Note:** The current implementation uses React state to manage employee records. It does not include a persistent database or backend API. Changes to employee records may be lost when the application is refreshed.

---

## 📂 Project Structure

The main project files are organized as follows:

```text
EmployeeManagement/
│
├── public/
│   └── index.html
│
├── src/
│   ├── components/
│   │   ├── EmployeeList.js
│   │   ├── AddEmployee.js
│   │   ├── EmployeeProfileUpdate.js
│   │   └── EmployeeSearch.js
│   │
│   ├── App.js
│   ├── App.css
│   └── index.js
│
├── .gitignore
├── package.json
├── package-lock.json
└── README.md
```

*Note: This is an example of the expected structure. Your actual filenames and folders may differ slightly.*

---

## 📋 Prerequisites

Before running the project locally, install the following:

* **Node.js:** Required to run the JavaScript development environment.
* **npm:** Included with Node.js.
* **Visual Studio Code:** Recommended code editor.
* **Web Browser:** Microsoft Edge, Google Chrome, or another modern browser.
* **Git:** Required if you want to manage and upload the project using GitHub.

Check whether Node.js and npm are installed by running:

```bash
node -v
npm -v
```

If these commands display version numbers, the tools are available.

If not, install Node.js from the official website:

https://nodejs.org/

---

## 🚀 Installation and Setup

Follow these steps to run the project on your computer.

### Step 1: Open the Project Folder

Open the `EmployeeManagement` project folder in Visual Studio Code.

Alternatively, open Command Prompt and navigate to your project directory:

```cmd
cd /d F:\employeemanagment
```

Replace the path if your project is stored in a different location.

### Step 2: Install Dependencies

Open the terminal in VS Code:

**Terminal → New Terminal**

Run:

```cmd
npm install
```

This installs the dependencies listed in `package.json`.

You generally need to run this command after downloading or cloning the project, or when dependencies change.

### Step 3: Start the Development Server

Run:

```cmd
npm start
```

If the command succeeds, the development server will start. In a typical Create React App project, the application opens at:

http://localhost:3000

If it does not open automatically, enter that address in your browser.

Keep the terminal open while using the local development server.

---

## ▶️ Running the Application

After starting the application, follow these steps:

1. Open the application in your browser.
2. View the employee list on the home page.
3. Navigate to the Add Employee page to enter new employee information.
4. Select an employee to access the update page, if supported by the interface.
5. Use the search page to locate employee information.
6. Use the delete option to remove an employee record.
7. Test the available features and verify the results.

### Useful Terminal Commands

| Command         | Description                                   |
| --------------- | --------------------------------------------- |
| `npm install`   | Installs project dependencies                 |
| `npm start`     | Starts the local development server           |
| `npm run build` | Creates a production build                    |
| `npm test`      | Runs the configured test script, if available |

**Important:** These commands assume your project uses Create React App. If your `package.json` uses Vite or another build tool, the available commands may differ.

---

## 🧭 Available Routes

The application uses React Router to manage navigation.

| Route                 | Purpose                                             |
| --------------------- | --------------------------------------------------- |
| `/`                   | Displays the employee list                          |
| `/addemployee`        | Opens the Add Employee page                         |
| `/updateemployee/:id` | Opens the employee update page for the specified ID |
| `/search`             | Opens the employee search page                      |

Example local URLs:

* Employee List: `http://localhost:3000/`
* Add Employee: `http://localhost:3000/addemployee`
* Search Employee: `http://localhost:3000/search`

The update route requires an employee ID, for example:

`http://localhost:3000/updateemployee/1`

---

## ☁️ Deployment

The application is hosted on **Render**.

### Live Application

🔗 https://employeemanagement-0n2q.onrender.com

### Deployment Workflow

The project can be maintained using GitHub and Render.

1. Make changes to the source code in Visual Studio Code.
2. Test the changes locally.
3. Commit and push the changes to the connected GitHub repository.
4. Render builds and deploys the updated application when automatic deployment is enabled.
5. Open the live website to verify the latest version.

### Git Commands

After saving and testing your changes, open the terminal in the project folder and run:

```cmd
git status
git add .
git commit -m "Update Employee Management System"
git push
```

If Git reports that there are no changes to commit, check `git status`. If the project has not been connected to a remote GitHub repository, configure the remote before pushing.

---

## ⚠️ Current Limitations

* Employee records are maintained in React state.
* The application does not currently use a backend API or database for permanent storage.
* Employee changes may be lost after a page refresh.
* The application does not currently include user authentication or role-based access control.

These limitations describe the current implementation and can be addressed in future versions.

---

## 🔮 Future Enhancements

The project can be extended with the following features:

* Integrate a backend API using Node.js, Express, or FastAPI.
* Connect a database such as MySQL or PostgreSQL.
* Store employee information permanently.
* Add user authentication and authorization.
* Implement department-wise filtering and advanced search.
* Add employee profile photos.
* Add data validation and improved error handling.
* Create reports and employee statistics.
* Improve responsive design for mobile devices.
* Add automated tests.

---

## 👩‍💻 Author

**Sujithra Dineshraja**

B.Tech – Artificial Intelligence and Data Science

GitHub: [dineshrajasujithra04](https://github.com/dineshrajasujithra04)

---

## 📄 License

This project was developed for educational and learning purposes.

A formal open-source license can be added if the project is intended for public reuse.
