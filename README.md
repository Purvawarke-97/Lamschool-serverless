# Student Management System (AWS Serverless)

A simple serverless web app to manage student records, hosted directly on AWS[cite: 1, 2]. Built with a static frontend and an event-driven AWS backend, so there are no servers to manage or maintain.


## Architecture

* **Frontend:** HTML, CSS, and JavaScript hosted on **Amazon S3** (Static Website Hosting)[cite: 1, 2, 3].
* **API:** **Amazon API Gateway** routes incoming `GET` and `POST` web requests.
* **Backend:** **AWS Lambda** (Python) processes logic to insert and fetch data.
* **Database:** **Amazon DynamoDB** stores student records in a NoSQL table.
* **Security:** **AWS IAM** provides Lambda permissions to access DynamoDB.


## Features

* Add student details (Student ID, Name, Class, Age)[cite: 3, 4].
* View the list of all registered students in a dynamic table[cite: 3, 5].
* Completely serverless and scales automatically on demand.

---

## Project Structure

##text
├── index.html               # Main landing page[cite: 1]
├── add_student.html         # Form to add a new student[cite: 4]
├── fetch_all_students.html  # Table displaying all students[cite: 5]
├── scripts.js               # API calls to API Gateway[cite: 3]
└── README.md
