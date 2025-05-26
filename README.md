# ATS resume analyzer

> this project is a personal extension and adaptation of an original tutorial-based implementation by [shivan118](https://github.com/Shivan118/Resume-Analyzer---Smart-ATS-System)

---

## Problem Statement

in today's competitive job market, job seekers face challenges ensuring their resumes align with job descriptions, meeting the criteria of applicant tracking systems (ats).  
ats filters often reject resumes that lack specific keywords or don't match job requirements, reducing the chances of securing interviews.

this project builds upon an open-source tutorial by [shivan118](https://github.com/Shivan118/Resume-Analyzer---Smart-ATS-System), expanding its capabilities and adapting it to new use cases and improved design choices.

---

## Business Use Cases

- **resume optimization for ats**  
  help job seekers tailor their resumes to specific job descriptions by identifying missing keywords and giving actionable feedback

- **personalized resume improvement**  
  deliver detailed suggestions to enhance resume content and increase interview chances

- **efficient resume evaluation**  
  streamline how resumes are evaluated by applicants, recruiters, or career coaches

- **enhancing job search success**  
  give candidates insights on how their resume aligns with job postings

- **scalable job application support**  
  offer a scalable analysis tool for career platforms or hr consultants

---

## Key Features

- **resume-job description match analysis**  
  calculates a match percentage between the resume and job description

- **keyword identification**  
  lists important missing keywords to improve ats compatibility

- **detailed profile summary**  
  provides a breakdown of strengths and areas for improvement

- **user-friendly interface**  
  built with streamlit for smooth and simple interaction

---

## How It Works

1. **upload resume**: upload your resume in pdf format  
2. **provide job description**: paste the job description into the input field  
3. **analyze resume**: the tool uses google gemini to process and compare content  
4. **review results**:
   - match score
   - missing keywords
   - profile summary

*note: this version has upgraded prompt handling, better ui logic with session state, and solid response parsing compared to the original tutorial.*---

## Project Setup

### 1. clone the Repository
```bash
git clone https://github.com/albedimaria/ats-resume-analyzer.git
cd ats-resume-analyzer
```

### 2.create virtual environment
```bash
conda create -p env python=3.10 -y
conda activate ./env
```
or using venv
```bash
python -m venv env
.\env\Scripts\activate   # Windows
source env/bin/activate  # macOS/Linux
```

### 3. install dependencies
```bash
pip install -r requirements.txt
```

### 4. configure environment
Create a .env file in the root directory and add your API key:

```bash
GOOGLE_API_KEY="your_api_key_here"
```

### 5. run the application
```bash
streamlit run app.py
```

