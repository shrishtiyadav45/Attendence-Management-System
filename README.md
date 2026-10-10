# 🎓 AI-Powered Attendance Management System

An intelligent, AI-powered attendance management system built using **Python, Hugging Face Inference API, and JSON**. The project enables users to manage, analyze, and update student attendance through natural-language queries, making attendance tracking easier, faster, and more interactive.

Instead of manually calculating attendance percentages or searching through student records, users can interact with an AI assistant to retrieve attendance information and perform supported operations.

## 🚀 Project Overview

The AI Attendance Management System combines traditional attendance record management with Large Language Model (LLM) capabilities. The AI interprets user queries and selects appropriate application tools to retrieve student information, calculate attendance statistics, or perform validated attendance updates.

Student records are maintained in a JSON file, providing a lightweight and easy-to-understand storage solution for an academic mini-project.

## ✨ Key Features

### 🤖 1. AI-Powered Natural Language Interaction
- Ask attendance-related questions in everyday language.
- Convert user queries into supported application operations.
- Receive clear, readable responses from the AI assistant.
- Reduce the need to manually search through student records.

### 📊 2. Attendance Percentage Calculation
- Calculate attendance percentages for individual students.
- Analyze attendance using present days and total working days.
- Identify students with comparatively high or low attendance.
- Support attendance-based academic monitoring.

### 👨‍🎓 3. Student Attendance Management
- Retrieve student information using available identifiers.
- Check attendance records for specific dates.
- Mark a student as present or absent for a supported date.
- Update existing attendance records with validation.
- Prevent invalid attendance updates where supported by the application logic.

### 📅 4. Date-Wise Attendance Tracking
- Maintain attendance records for individual dates.
- Check whether a student was present on a particular day.
- Review attendance across a configured date range.
- Track changes to attendance records through application operations.

### 🧮 5. Automated Calculations and Analysis
- Calculate attendance percentages automatically.
- Compare attendance records across students.
- Identify students who may require attendance follow-up.
- Perform supported basic arithmetic operations.

### 🗂️ 6. JSON-Based Data Storage
- Store student details in a structured JSON file.
- Keep attendance records readable and easy to edit.
- Simplify data exchange between application components.
- Make the project suitable for local development and demonstrations.

### 🔐 7. Configuration and Error Handling
- Use environment variables for API credentials.
- Keep API tokens out of committed source files.
- Validate supported inputs before modifying records.
- Handle invalid queries, missing records, and API errors where implemented.

## 🛠️ Technology Stack

| Technology | Purpose |
|---|---|
| Python | Core application logic |
| Hugging Face Inference API | AI-powered query interpretation |
| Large Language Model (LLM) | Natural-language understanding |
| JSON | Student and attendance data storage |
| Python functions/tools | Controlled attendance operations |
| python-dotenv | Environment-variable configuration |

## 🏗️ System Architecture

1. **User Input:** The user enters an attendance-related question.
2. **AI Processing:** The language model interprets the request.
3. **Tool Selection:** The AI selects an available operation when appropriate.
4. **Application Logic:** Python validates and executes the requested operation.
5. **Data Access:** Student attendance information is read from or updated in JSON.
6. **Response Generation:** The result is returned in a readable format.

```text
           User Query
                |
                v
       AI Attendance Assistant
                |
                v
        Query Interpretation
                |
                v
       Supported Tool Selection
                |
                v
       Python Application Logic
                |
                v
        JSON Student Records
                |
                v
        Result / AI Response
```

## 📂 Project Structure

```text
Attendance-System/
├── app.py
├── students.json
├── requirements.txt
├── .env.example
├── .gitignore
└── README.md
```

*Note: The exact filenames may differ depending on the project version.*

## ⚙️ Installation and Setup

### Prerequisites
- Python 3.10 or a compatible version.
- pip package manager.
- Internet connectivity for API-based AI functionality.
- A valid Hugging Face API token with the required model access.

### Step 1: Clone the Repository

```bash
git clone YOUR_GITHUB_REPOSITORY_URL
cd Attendance-System
```

### Step 2: Install Dependencies

```bash
pip install -r requirements.txt
```

### Step 3: Configure Environment Variables

Create a `.env` file based on `.env.example` and add the required credentials.

```env
HF_TOKEN=your_huggingface_api_token
```

Use the exact variable name expected by your application. Never upload real API tokens to GitHub.

### Step 4: Prepare Student Data

Ensure that `students.json` contains valid student records in the schema expected by the application.

### Step 5: Run the Application

```bash
python app.py
```

## 💬 Example User Queries

The following examples illustrate the intended interaction, provided the corresponding operations are implemented in the project.

- "What is the attendance percentage of student 101?"
- "Was student 102 present on 10 October 2026?"
- "Mark student 103 as present for 12 October 2026."
- "Remove the attendance entry for student 101 on 9 October 2026."
- "Which student has the highest attendance percentage?"
- "Show attendance details for all students."
- "Calculate the attendance percentage of every student."

## 📐 Attendance Calculation

Attendance percentage is calculated using the formula:

**Attendance Percentage = (Days Present / Total Working Days) × 100**

For example, if a student attends 18 out of 20 working days:

```text
Attendance Percentage = (18 / 20) × 100
                      = 90%
```

## 🎯 Project Objectives

- Demonstrate practical applications of Generative AI.
- Integrate an LLM with Python application logic.
- Explore tool calling and natural-language interfaces.
- Automate common attendance calculations.
- Demonstrate structured data storage using JSON.
- Build a foundation for a more complete attendance management platform.

## 🔮 Future Enhancements

- Develop a responsive web dashboard using React or Next.js.
- Add a FastAPI backend with REST endpoints.
- Migrate from JSON storage to PostgreSQL or MySQL.
- Introduce secure login and role-based access for administrators, faculty, and students.
- Generate downloadable attendance reports in CSV and PDF formats.
- Add charts, class-wise statistics, and attendance trends.
- Introduce configurable attendance threshold alerts.
- Add audit logs and confirmation steps for attendance changes.
- Support multiple classes, subjects, semesters, and academic sessions.
- Add automated testing and deployment workflows.

## 🔒 Security and Reliability

- Keep API credentials in environment variables.
- Validate user inputs and student identifiers.
- Restrict the AI to explicitly supported application operations.
- Validate attendance changes before writing to storage.
- Consider backups and audit logs before using the system for real academic records.

## 🎓 Learning Outcomes

This project provides hands-on experience with Python programming, Generative AI integration, LLM-based query interpretation, tool calling, JSON data management, input validation, and application architecture.

## 👨‍💻 Project Type

**B.Tech AI/ML Mini Project**

## 📄 License

Choose an appropriate open-source license, such as the MIT License, before publishing the repository. Add a `LICENSE` file if you decide to distribute the project under that license.

---

**Disclaimer:** This project is an educational prototype. Features described as future enhancements or examples should not be considered implemented unless they are available in the current source code.
