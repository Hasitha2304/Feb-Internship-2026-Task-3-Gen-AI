# Feb-Internship-2026-Task-3-Gen-AI
# AI Resume Screening System

## Objective
The aim of this project is to build an AI-based system that can screen resumes and evaluate candidates based on a given job description using LangChain.

## Features
- Extracts skills, tools, and experience from resumes  
- Compares resume data with job requirements  
- Assigns a score between 0 and 100  
- Provides an explanation for the score  
- Uses LangSmith for tracing and debugging  

## Technologies Used
- Python  
- LangChain  
- HuggingFace models  
- LangSmith  

## Pipeline
Resume → Skill Extraction → Matching → Scoring → Explanation  

## Input
- Three resumes:
  - Strong candidate  
  - Average candidate  
  - Weak candidate  
- One job description  

## Output
For each candidate:
- Score (0–100)  
- Explanation of the result  

## Working
The system first extracts important information such as skills and experience from the resume.  
Then it compares this information with the job description to find matching and missing skills.  
Based on this comparison, a score is generated.  
Finally, the system explains why the candidate received that score.

## LangSmith Tracing
LangSmith is used to track each step of the pipeline. It helps in understanding how the model processes inputs and generates outputs, and also helps in debugging errors.

## Debugging
Initially, there were issues with token length when using GPT-2. This was handled by modifying generation parameters and improving prompts.

## Note
The system does not assume any skills that are not mentioned in the resume and only evaluates based on the given data.
