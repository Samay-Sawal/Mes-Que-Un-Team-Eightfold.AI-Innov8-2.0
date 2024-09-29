# Mes-Que-Un-Team-Eightfold.AI-Innov8-2.0
Overview

The Més que un team project involves building an AI-powered HR Decision Support System. The system is designed to assist with resume and recommendation letter analysis for hiring purposes, utilizing advanced Natural Language Processing (NLP) models. The primary goal is to enhance hiring decisions by detecting fraud, analyzing professional connectivity, and evaluating candidates' profiles.

Key Features:   
Fraud Detection: Detects inconsistencies and exaggerated claims in resumes and recommendation letters.
Connectivity Score: Analyzes the professional network strength based on connections and endorsements.
Profile Score: Evaluates candidates' work experience, skills, and suitability for a role.

Project Structure

1. Exploratory Data Analysis (EDA)
Data Summary: Basic overview of the dataset (1000 applicant entries, each with a unique ID).
Visualization: Various charts like bar graphs, word clouds, and pie charts to represent candidate data.
2. Fraud Detection
Reciprocal Endorsements: Detects when two individuals endorse each other, a sign of potential bias.
Exaggerated Recommendations: Uses DistilBERT to detect exaggerated claims in Letters of Recommendation (LORs).
Resume-LOR Correlation: Compares resume and LOR content for consistency using cosine similarity.
3. Connectivity Analysis
LORs: Counts the number of genuine recommendations received and given by a candidate.
Work Experience & Education Overlap: Identifies connections between candidates based on shared education or work history.
Influence Score: Measures a candidate's influence within their field and across other domains using various metrics like Degree Centrality.
4. Profile Score
Experience Analysis: Uses Qwen2 LLM to evaluate the candidate's years of experience.
Skills Filtering: Allows HR users to filter candidates based on job-specific keywords.
5. HR Decision Support Dashboard
A user-friendly interface providing:
Keyword search functionality
Candidate comparison
Fraud detection alerts
Connectivity and Profile Scores
Domain-specific filters
Downloadable CVs and LORs
How It Works

The solution employs three primary scores:

Fraudulent Score: Detects potential fraud based on exaggerated or inconsistent claims in resumes and LORs.
Connectivity Score: Analyzes the candidate's professional network and influence.
Profile Score: Quantifies experience and skills to assess job suitability.
The Decision Tree model is used to calculate and weigh these scores, offering a holistic view of each candidate.

Conclusion

This project delivers a comprehensive AI-powered HR Decision Support System, enhancing hiring efficiency by:

Automatically detecting fraudulent claims
Analyzing professional connections
Evaluating candidate profiles based on experience and skills.
This system allows recruiters to make informed decisions, ensuring the best-fit candidates are selected for a given role.

Annexure

Annexure A: Explains cosine similarity in detecting LOR-CV alignment.
Annexure B: Details the clustering techniques (e.g., KNN) used to identify bias in recommendation letters.
Requirements
Python 3.x
NLP models: DistilBERT, Qwen2
Libraries: scikit-learn, TensorFlow, etc.






