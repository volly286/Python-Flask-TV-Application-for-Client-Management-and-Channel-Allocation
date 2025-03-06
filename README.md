# Python/Flask Application Documentation

**Author:** Marin Valentin-Gabriel 432B

---

## Introduction

The presented application is developed using Python with the Flask framework for the backend and technologies such as HTML, CSS, and Bootstrap for the frontend. It manages an N:M relationship between two entities: clients and TV stations.

---

## Technologies Used

### Python and Flask:
- The Flask framework was used to develop the application's backend. Flask provides an easy-to-use and scalable architecture for web applications.

### HTML, CSS, and Bootstrap:
- The frontend utilizes HTML and CSS for structure and design, while Bootstrap ensures responsiveness and a modern interface style.

### MySQL:
- The database used is MySQL, and the connection with the Flask application was made using the `mysql-connector` library.

---

## Application Description

The application is built to manage the N:M relationship between two main entities:
- **Clients** - represented by attributes: first name, last name, and email.
- **TV Stations** - each with a name and description.

Application functionalities include:
- CRUD (Create, Read, Update, Delete) operations for the `clients` and `tvstations` tables.
- Associating and disassociating the `clients` and `tvstations` entities through an intermediate table (`clients_tvstations`).

---

## Database Diagram

The database diagram represents the N:M relationship between `clients` and `tvstations` through the `clients_tvstations` table. This diagram was generated using MySQL Workbench and is included in the next section (also accessible via the `MySQL_Diagram.html` file in the resources folder).

---

## Application Folder Structure

The complete project structure can be found in the `resources` folder, under the name `Project_Structure_Python.html`.

---

## Key Code Sections

### CRUD Functionalities:

#### List Clients:
- Displays the list of existing clients in the database. If the user enters a search parameter (email), the function filters results by that email.

#### Add Client:
- Allows adding a new client to the database via a form.

#### Edit Client:
- Enables updating the information of an existing client.

#### Delete Client:
- Deletes a specified client from the database.

---

## Installation and Usage Guide

### Python Installation:
1. Download and install Python 3.9.10 from the official website or the resources folder.
2. Run the installer and check the "Add Python to PATH" option to add Python to environment variables.
3. Follow the installation steps.

### MySQL Installation:
1. Download and install MySQL Server 8.0.40 from the official MySQL website or the resources folder.
2. Follow the installation wizard steps:
   - Select "Server only" if other MySQL components are not required.
   - Configure the server:
     - **Username:** Choose a username (e.g., root).
     - **Password:** Set a strong password.
3. Complete the installation.

### MySQL Configuration:
1. Open MySQL Workbench or any other MySQL client.
2. Connect to the server using the credentials set during installation.
3. Create a new database and import the `db.sql` file from the `resources` folder.
4. Navigate to the application's `src` folder and locate the `config.py` file.
5. Open the file and replace the `*****` placeholders with your credentials:
   - Database name
   - MySQL username
   - MySQL password

### Running the Application:
1. After verifying the above steps, run the application using the provided executable.
2. **Important:** The executable-based applications may be flagged as a virus by antivirus software. Temporarily disable your antivirus to run the application correctly.

---

## Bibliography:
- **Python Software Foundation, "Python 3.9 Documentation,"** [Online]. Available: https://docs.python.org/3.9/.
- **Flask Project, "Flask Documentation,"** [Online]. Available: https://flask.palletsprojects.com/.
- **The Bootstrap Team, "Bootstrap Documentation,"** [Online]. Available: https://getbootstrap.com/.
- **Oracle Corporation, "MySQL 8.0 Reference Manual,"** [Online]. Available: https://dev.mysql.com/doc/.
- **Oracle Corporation, "MySQL Workbench User Guide,"** [Online]. Available: https://dev.mysql.com/doc/workbench/en/.
- **IEEE, "Conference Publishing Templates,"** [Online]. Available: https://www.ieee.org/conferences/publishing/templates.html.
