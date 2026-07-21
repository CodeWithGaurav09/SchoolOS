# NYC School Management App

A simple NYC school management system built with Streamlit and a small CLI fallback. The app tracks students, teachers, and grades using a local JSON data file.

## Project Structure

- `NYC-Management-App-main/app.py` - Main Streamlit dashboard and user interface for registering students and teachers, adding grades, and viewing details.
- `NYC-Management-App-main/main.py` - Command-line interaction script for basic student and teacher registration, grade entry, and detail lookup.
- `NYC-Management-App-main/school_data.json` - Local JSON storage for registered students, teachers, and grades.

## Features

- Student registration with name, age, email, and roll number
- Teacher registration with name, age, email, subject, and employee ID
- Add grades for registered students
- View student details and average score
- View teacher details and subject assignments
- Streamlit dashboard with a polished UI and summary statistics

## Requirements

- Python 3.8+
- `streamlit`

## Installation

1. Open a terminal in the project folder.
2. Install dependencies:

```bash
pip install streamlit
```

## Run the Streamlit app

From the outer project root:

```bash
streamlit run NYC-Management-App-main/app.py
```

Or from inside `NYC-Management-App-main/NYC-Management-App-main`:

```bash
streamlit run app.py
```

Then open the local Streamlit URL shown in the terminal.

## Run the CLI script

From the inner project folder:

```bash
python main.py
```

## Data Storage

The app stores all records in `NYC-Management-App-main/school_data.json`.

## Notes

- Email validation is basic and checks only for `@` and `.` characters.
- All data is stored locally in a JSON file, so the app is best for demos and small testing scenarios.
- The Streamlit app provides a nicer UI, while `main.py` supports quick terminal-based operations.
