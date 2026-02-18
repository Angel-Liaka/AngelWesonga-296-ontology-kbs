# 📘 University Advising Ontology Knowledge-Based System

## 👤 Student Information

Name: Angel Wesonga<br>
Course: Knowledge Based Systems

## 🧠 Overview

This project demonstrates a simple ontology-based Knowledge-Based System (KBS) for a university advising scenario.
The system includes students, courses, and prerequisite relationships, and applies inference to determine whether a student is eligible to take a course and which courses should be recommended next.
The implementation is written in Python and executed using a Jupyter Notebook.

## 🧩 Ontology Design

Concepts (Classes):<br>
Student<br>
Course

Relationships (Properties):
requires (Course → Course) – course prerequisites<br>
completed (Student → Course) – courses a student has completed<br>
eligibleFor (Student → Course) – inferred relationship showing course eligibility

## 🔄 Inference Process

The system checks whether a student has completed all the prerequisite courses required for a given course.
If all prerequisites are met, the student is inferred to be eligible to take the course.
If some prerequisites are missing, the system returns the missing courses.
The system also recommends courses that a student is eligible for but has not yet completed.

## ✅ Expected Output

Eligibility results for different students and courses<br>
Missing prerequisite courses when a student is not eligible<br>
A list of recommended courses for each student based on completed courses<br>

Example:<br>
Tarah eligibility for Discrete Math: (True, set())<br>
Erick eligibility for Discrete Math: (False, {'Calculus 2'})<br>
Stacy eligibility for Probability and Statistics: (True, set())<br>
Stacy eligibility for Machine Learning: (False, {'Probability and Statistics'})<br>
Tarah course recommendations: ['Discrete Math']<br>
Erick course recommendations: ['Calculus 2']<br>
Stacy course recommendations: ['Probability and Statistics']

## Repo Structure
AngelWesonga-296-ontology-kbs/
├──AngelWesonga-296-ontology-kbs.ipynb
└── README.md


## ▶️ How to Run The Notebook

Open the file AngelWesonga-296-ontology-kbs.ipynb in VS Code or Jupyter Notebook<br>
Run all cells from top to bottom<br>
Ensure all outputs are visible below the cells

## ▶️ How to Run Tests
All tests are included in the last cell of the notebook. 
To run the tests, execute the final cell. You should see output showing that all tests pass.


## ⚠ Originality

I expanded the lecturer’s example by adding more students, more courses, and multi-level prerequisite relationships.
I also included course recommendation functionality and validation checks to make the system more realistic.