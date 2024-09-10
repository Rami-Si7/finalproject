# HSTS - High School Test System

# Overview

HSTS (High School Test System) is a computerized information system designed to streamline and enhance the efficiency of the exam process in high schools. It facilitates tasks such as:

* Question creation
* Exam generation
* Distribution of exams to students
* Approval and grading
* Access to grades and exam statistics
The system improves both the reliability and ease of exam administration.


# Features

* Question Bank Management: Create, edit, and store exam questions.
* Exam Generation: Generate exams using predefined templates or custom selections.
* Exam Distribution: Distribute exams to students electronically.
* Grading and Statistics: Manage exam grading and provide insightful statistics on exam performance.


# System Architecture

1. Client Module
* Built using JavaFX and OCSF (Object Client-Server Framework).
* Uses EventBus (following the mediator pattern) to pass events between components, specifically between SimpleClient and PrimaryController.
2. Server Module
* Simple server-side application built using OCSF.
* Handles requests from the client, processes data, and communicates with the database.
3. Entities Module
* Shared module containing all the entities used by both the client and server.
* Represents the data structures, such as users, questions, exams, and grades.

# Technologies

* JavaFX: Used for building the client-side graphical user interface (GUI).
* OCSF: A framework for simplifying the client-server architecture.
* EventBus: Implements the mediator pattern, facilitating the communication between different components.
* MySQL/: database used to store the question bank, student information, exams, and grades.
