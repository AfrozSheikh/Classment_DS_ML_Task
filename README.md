Job Role Recommendation Engine

Overview:
This project is a simple recommendation engine that suggests the most similar job roles based on shared required skills. It uses cosine similarity to measure skill-based similarity between job roles.

Features
Accepts a job role as input and recommends the top N most similar roles.

Uses cosine similarity to compare roles based on shared skills.

Handles case-insensitive inputs and invalid role names gracefully.

Implements binary encoding for skill representation.

Technologies Used
Python

Pandas

Scikit-learn

Installation & Setup
Clone this repository:

git clone https://github.com/AfrozSheikh/Classment_DS_ML_Task.git
cd job-role-recommendation
Install dependencies:
pip install pandas scikit-learn
Run the Jupyter Notebook in VS Code or Jupyter Lab.

Usage
Run the function in your Jupyter Notebook:


print(get_top_recommendations_cosine("ML Engineer"))
Example Output:

['AI Researcher', 'Data Scientist', 'NLP Engineer']
Methodology
1. Data Preparation
A dataset of job roles and their required skills was created.

Skills were converted into a binary matrix using MultiLabelBinarizer.

2. Similarity Calculation
Cosine similarity was used to compare skill vectors.

Similarity scores range from 0 to 1 (higher values indicate more similarity).

3. Recommendation Process
The system identifies top N roles with the highest similarity scores.

Outputs a list of recommended roles.

Why Cosine Similarity?
✅ Works well with binary data (1 = skill present, 0 = skill absent).
✅ Focuses on skill overlap rather than total number of skills.
✅ Provides clear similarity scores for easy interpretation.