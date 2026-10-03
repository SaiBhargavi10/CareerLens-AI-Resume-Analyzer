# CareerLens – AI Resume Analyzer

CareerLens is an AI-powered resume analysis web application that helps users analyze and improve their resumes. Users can upload their resumes and receive AI-based insights about their resume quality, strengths, weaknesses, missing skills, improvement suggestions, and interview preparation.

## Features

* Upload resumes in PDF and DOCX formats
* AI-powered resume analysis
* ATS compatibility analysis
* Resume summary generation
* Identify resume strengths
* Identify resume weaknesses
* Detect missing or relevant skills
* Provide resume improvement suggestions
* Generate interview questions based on the resume
* Downloadable analysis report

## Tech Stack

### Frontend

* React.js
* Vite
* Axios
* CSS

### Backend

* Python
* FastAPI
* Google Gemini API
* pdfplumber
* python-docx

## Project Structure

```text
CareerLens/
│
├── backend/
│   ├── app/
│   └── uploads/
│
├── frontend/
│   └── src/
│
├── screenshots/
├── .gitignore
├── package-lock.json
├── requirements.txt
└── README.md
```

## Prerequisites

Before running the project, make sure the following are installed:

* Python 3.9 or later
* Node.js and npm
* Git
* A Google Gemini API key

## Installation and Setup

### 1. Clone the Repository

```bash
git clone https://github.com/SaiBhargavi10/CareerLens-AI-Resume-Analyzer.git
cd CareerLens
```

### 2. Backend Setup

Open a terminal and navigate to the backend directory:

```bash
cd backend
```

Create a Python virtual environment:

```bash
python -m venv venv
```

Activate the virtual environment.

For Windows:

```bash
venv\Scripts\activate
```

Install the required Python packages:

```bash
pip install -r ../requirements.txt
```

### 3. Configure the Gemini API Key

Create a `.env` file inside the `backend` directory:

```text
GEMINI_API_KEY=YOUR_GEMINI_API_KEY
```

Replace `YOUR_GEMINI_API_KEY` with your own Gemini API key.

**Do not upload the `.env` file or your API key to GitHub.**

### 4. Start the Backend

From the `backend` directory, run:

```bash
uvicorn app.main:app --reload
```

The backend will be available at:

```text
http://127.0.0.1:8000
```

### 5. Frontend Setup

Open another terminal and navigate to the frontend directory:

```bash
cd frontend
```

Install the required packages:

```bash
npm install
```

Start the frontend:

```bash
npm run dev
```

The frontend will be available at the URL displayed in the terminal, usually:

```text
http://localhost:5173
```

## How to Use

1. Open the CareerLens application.
2. Upload your resume in PDF or DOCX format.
3. Submit the resume for analysis.
4. The application processes the uploaded document.
5. AI analyzes the resume.
6. Review the generated:

   * Resume summary
   * ATS analysis
   * Strengths
   * Weaknesses
   * Missing skills
   * Improvement suggestions
   * Interview questions
7. Review or download the generated analysis report.

## Environment Variables

The backend requires the following environment variable:

```text
GEMINI_API_KEY=YOUR_GEMINI_API_KEY
```

Keep your API key private and never commit it to the repository.

## Author

**Bhargavi**
