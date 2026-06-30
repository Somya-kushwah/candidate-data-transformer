

# Candidate Data Transformer

## Problem Statement

This project transforms candidate data collected from multiple sources into one clean and unified candidate profile.

The system handles duplicate candidates, cleans data formats, merges information, and generates a standard JSON output.

---

## Data Sources

### Structured Source
- recruiter.csv

Contains:
- Candidate ID
- Name
- Email
- Phone
- Company
- Job Title


### Unstructured Source
- resumes.json

Contains:
- Skills
- Experience
- Education


---

## Processing Pipeline

Input Sources

        ↓

Data Extraction

        ↓

Normalization

        ↓

Duplicate Detection

        ↓

Profile Merging

        ↓

Confidence Calculation

        ↓

Final JSON Output


---

## Features

- Read multiple data sources
- Normalize phone numbers
- Normalize skills
- Detect duplicate candidates using email matching
- Merge candidate profiles
- Generate confidence score
- Export structured JSON output


---

## Output Schema

Example:

{
candidate_id,
full_name,
emails,
phones,
skills,
experience,
education,
provenance,
overall_confidence
}


---

## How To Run

1. Upload files:

recruiter.csv

resumes.json


2. Run notebook cells sequentially


3. Final output generated:

output/candidate_profiles.json


---

## Technologies Used

Python

Pandas

JSON


