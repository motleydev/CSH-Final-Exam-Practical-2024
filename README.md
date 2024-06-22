### Final Project: Simple Note-Taking Application

#### Project Overview
The final project involves creating a simple note-taking application where users can create, view, update, and delete notes. This project will be built entirely in Python using Django to handle both the front-end and back-end functionalities. The application will utilize a SQLite database to store note data and Docker for deployment. The goal is to demonstrate your understanding of front-end development, back-end development, DevOps, and data structures/database management.

A final feature will be revealed on the day of the test, but you are welcome to dry-run the project and bring example code with you. The use of LLMs is also allowed.

### Project Sections

#### 1. Front-end Development
- **Objective**: Develop a minimalistic UI using Django templates.
- **Requirements**:
  - Use Django templates to create HTML pages for the application.
  - Implement features such as note creation, viewing, updating, and deletion.
  - Ensure the UI interacts with the back-end through Django views and forms.
  - Adhere to the principles of clean and simple UI design.

**Prompt for ChatGPT**:
```
Create a minimalistic UI for a note-taking application using Django templates. The application should have the following features:
1. A page that lists all notes with options to edit or delete each note.
2. A form to create new notes.
3. A form to update existing notes.
4. A confirmation step for deleting notes.

Provide the HTML templates for listing notes, creating a note, updating a note, and deleting a note. Use Django's templating system and ensure the forms interact with Django views using CSRF protection. The design should be clean and simple.
```

#### 2. Back-end Development
- **Objective**: Use Django to develop the application's backend.
- **Requirements**:
  - Develop RESTful API endpoints using Django views.
  - Implement CRUD operations (Create, Read, Update, Delete) for managing notes.
  - Handle data validation and error management.
  - Ensure the back-end is well-structured and follows best practices.

**Prompt for ChatGPT**:
```
Develop the backend for a note-taking application using Django. The backend should include the following:
1. Django models to represent notes, with a single field for the note content.
2. Django views to handle HTTP requests for creating, reading, updating, and deleting notes.
3. RESTful API endpoints for the same CRUD operations.
4. Proper data validation and error handling in the views.

Provide the Django models, views, and URL configurations necessary to implement these features. Ensure that the views are well-documented and follow best practices.
```

#### 3. DevOps
- **Objective**: Containerize the application using Docker and manage deployment.
- **Requirements**:
  - Create a `Dockerfile` to containerize the application.
  - Write a `docker-compose.yml` file to orchestrate the deployment of the Django server and database.
  - Ensure the application runs smoothly and consistently across different environments.

**Prompt for ChatGPT**:
```
Create the necessary files to containerize and deploy a Django-based note-taking application using Docker. This includes:
1. A `Dockerfile` to build a Docker image for the Django application. The image should include all necessary dependencies and configurations.
2. A `docker-compose.yml` file to define services, networks, and volumes for the application. The setup should include services for the Django application and an SQLite database.
3. Instructions for building and running the Docker containers, applying migrations, and accessing the application.

Provide the `Dockerfile` and `docker-compose.yml` file content, as well as the steps for deployment.
```

#### 4. Data Structures and Database Management
- **Objective**: Use SQLite to manage note data and implement data structures.
- **Requirements**:
  - Use SQLite for the database.
  - Design the database schema using Django models.
  - Implement data retrieval and manipulation using Django ORM.
  - Ensure efficient and effective database management practices.

**Prompt for ChatGPT**:
```
Design and implement the database schema for a note-taking application using Django ORM with SQLite. The requirements are:
1. Define a Django model for notes with a field for the note content.
2. Implement data retrieval and manipulation methods using Django ORM.
3. Ensure that the database schema is normalized and follows best practices.
4. Provide a script for database migrations and initial setup.

Provide the Django model definition, and examples of ORM queries for creating, reading, updating, and deleting notes. Also, include the necessary migration commands and steps for database setup.
```

### Grading Criteria

Total Points: 50
Each grading criteria is worth 10 points
Total time: 1,5 Hours

1. **Thought Process and Methodical Approach**
   - Clear documentation of the project plan and individual contributions.
   - Logical breakdown of tasks and systematic approach to problem-solving.

2. **Project Structure**
   - Well-organized codebase with clear separation of concerns.
   - Consistent use of modules, functions, and classes.

3. **Naming Convention**
   - Adherence to naming conventions for variables, functions, and classes.
   - Descriptive and meaningful names.

4. **Comment Usage**
   - Comprehensive comments explaining the code logic and decision-making process.
   - Use of docstrings for functions and classes.

5. **Adherence to the Zen of Python**
   - Writing clean, readable, and Pythonic code.
   - Following principles such as simplicity, readability, and explicitness.

### Final Deliverable
- A GitHub repository containing the entire project.
- A Docker Compose setup to run the application locally.
- A brief presentation explaining the project architecture, individual contributions, and key learnings.

### Example Project Structure

```
note_taking_app/
├── manage.py
├── Dockerfile
├── docker-compose.yml
├── requirements.txt
├── app/
│   ├── __init__.py
│   ├── settings.py
│   ├── urls.py
│   ├── wsgi.py
│   ├── asgi.py
│   ├── models.py
│   ├── views.py
│   ├── forms.py
│   ├── templates/
│   │   ├── index.html
│   │   ├── create_note.html
│   │   ├── edit_note.html
│   │   ├── delete_note.html
│   └── migrations/
│       ├── __init__.py
│       └── 0001_initial.py
└── README.md
```

### Instructions for Running the Project

1. **Clone the Repository**:
   ```sh
   git clone https://github.com/yourusername/note_taking_app.git
   cd note_taking_app
   ```

2. **Build and Run the Docker Containers**:
   ```sh
   docker-compose up --build
   ```

3. **Apply Migrations**:
   ```sh
   docker-compose run web python manage.py migrate
   ```

4. **Access the Application**:
   - Open a web browser and go to `http://localhost:8000`.

5. **Creating and Managing Notes**:
   - Use the UI to create, view, update, and delete notes.

### Presentation Outline
- **Introduction**: Brief overview of the project and its objectives.
- **Architecture**: Explanation of the application architecture and how different components interact.
- **Development Process**: Outline the development process, including challenges faced and solutions implemented.
- **Demo**: Live demonstration of the application.
- **Conclusion**: Key learnings and future improvements.

### Additional Notes
- Ensure code quality by following PEP 8 guidelines.
- Use Git for version control and document all major changes with meaningful commit messages.
- Include tests for critical parts of the application to ensure reliability.

By completing this project, you will demonstrate your ability to develop a full-stack web application using Django, manage a database using SQLite, containerize applications with Docker, and follow best practices in software development.
