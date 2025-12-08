# Parallel-Text-Handling-Processor-for-Job-Description-Skill-Extraction
This project focuses on developing system that processes large volumes of job descriptions to identify and extract required technical skills. Job postings are unstructured and written in varied formats making it difficult to analyze skill demands. The system uses a combination of text cleaning and parallel processing techniques to analyze job data.

# OBJECTIVES

- Automate extraction of skills from unstructured job descriptions.

- Use parallel processing to significantly improve execution speed.

- Maintain skills in a database for easy updates without modifying code.

- Clean and normalize job text for better accuracy.

- Perform skill frequency analysis to identify high-demand technologies.

- Generate visual insights like bar graphs for presentation and reporting.

# KEY FEATURES

- Parallel Skill Extraction using ThreadPoolExecutor

- SQLite Database Integration for storing skill keywords

- Text Cleaning Module for preprocessing job descriptions

- Dynamic Regex Pattern built from database skills

- Structured Output stored in CSV files

- Skill Frequency Analysis with automatic bar graph plotting


# WORKFLOW

-> Load Job Dataset
Reads a CSV file containing job descriptions.

-> Clean Text
Removes HTML tags, special characters, and extra spaces.

-> Load Skills from SQLite Database
Skills are stored and retrieved dynamically.

-> Build Regex Pattern
Converts the skill list into a case-insensitive search pattern.

-> Parallel Processing
Uses a ThreadPool to process multiple job descriptions simultaneously.

-> Extract Skills
Finds and records skills appearing in each job description.

-> Skill Counting
Uses collections.Counter to count how many times each skill appears.

-> Save Results
Saves structured outputs (cleaned_job_skills_output_db.csv and skill_counts_from_db.csv).

-> Visualization
Plots the top N most frequent skills in a bar graph.

# TECHNOLOGIES USED

- Python

- SQLite (skills database)

- Pandas (data handling)

- Regex / RE module

- ThreadPoolExecutor (parallel processing)

- Matplotlib (visualization)

# HOW TO RUN THE PROJECT

- Place your job description dataset in CSV format.

- Ensure extract_with_db.py and skills.db are in the same directory.

- Run the script:

    python extract_with_db.py

- View outputs:

    Cleaned data → cleaned_job_skills_output_db.csv

    Skill frequency → skill_counts_from_db.csv

    Visual graph → skill_frequency_bar_chart.png



# WHY THIS PROJECT IS USEFUL

- Helps identify which skills companies want most

- Can process thousands of job descriptions quickly

- Database makes skill updates easy

- Resulting data can help students, HR teams, and educators

