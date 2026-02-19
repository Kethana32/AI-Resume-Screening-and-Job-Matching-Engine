**Download the .ipynb file to preview it**
**NOTE**: Resume data of our project has not been uploaded directly due to the github's "size limitations". 
Download it from the below link:
### https://www.kaggle.com/datasets/snehaanbhawal/resume-dataset? 

AI Resume Screening and Job Matching Engine

📌 Project Description

The AI Resume Screening and Job Matching Engine is an intelligent recruitment assistance system designed to automate the process of evaluating and ranking job candidates. Traditional resume screening is time-consuming and subjective, requiring recruiters to manually analyze hundreds of resumes. This project leverages Natural Language Processing (NLP) and AI-based semantic understanding to automatically analyze resumes and rank candidates based on their relevance to a given job description.

The system reads multiple resumes in PDF format, extracts textual information, understands the semantic meaning of the content using transformer-based language models, and compares each resume with a recruiter-provided job description. Instead of relying only on keyword matching, the model evaluates contextual similarity, ensuring that candidates with relevant experience are correctly identified even when different wording is used.

The project combines two evaluation strategies:

1. **Semantic Similarity Analysis** – Uses a pre-trained Sentence Transformer model to understand the meaning of resumes and job descriptions and measure how closely they match.
2. **Skill-Based Matching** – Extracts technical skills from resumes and compares them with required job skills to calculate a skill compatibility score.

A weighted scoring mechanism combines both approaches to produce a final ranking score. Candidates are then sorted from most suitable to least suitable, helping recruiters quickly identify top applicants.

This system simulates real-world Applicant Tracking Systems (ATS) used by companies and demonstrates how AI can significantly improve recruitment efficiency, reduce manual effort, and enable data-driven hiring decisions.



⚙️ Technologies Used

- Python
- Google Colab
- Natural Language Processing (NLP)
- Sentence Transformers (all-MiniLM-L6-v2)
- Cosine Similarity
- PyPDF2 (PDF text extraction)
- Scikit-learn
- Pandas & NumPy
- Matplotlib (visualization)



🧠 Working Methodology

1. **Resume Upload**
   - Multiple resumes are uploaded in ZIP format.
   - PDF files are extracted automatically.

2. **Text Extraction**
   - Resume content is extracted using PyPDF2.
   - Raw text is prepared for analysis.

3. **Semantic Embedding Generation**
   - Sentence Transformer converts text into numerical embeddings representing semantic meaning.

4. **Similarity Calculation**
   - Cosine similarity measures how closely each resume matches the job description.

5. **Skill Extraction**
   - A predefined skills list is used to detect relevant technical skills in resumes.

6. **Final Score Calculation**
   - Final Score = 70% Semantic Similarity + 30% Skill Match Score.

7. **Candidate Ranking**
   - Resumes are ranked automatically based on final scores.

8. **Visualization & Export**
   - Ranking results are visualized using charts.
   - Final ranked candidates are exported as a CSV file.



▶️ How to Execute the Project

### Step 1: Open Notebook
Open the provided `.ipynb` file in **Google Colab**.

### Step 2: Install Dependencies
Run the installation cells to install required libraries:
sentence-transformers
PyPDF2
scikit-learn

### Step 3: Upload Dataset
Download the dataset from the provided link:
https://www.kaggle.com/datasets/snehaanbhawal/resume-dataset?
Upload the ZIP file containing resume PDFs when prompted.

### Step 4: Extract Files
Execute the unzip cells to extract resumes into folders.(already included in code)

### Step 5: Provide Job Description
Edit the job description text inside the notebook according to the target role.

### Step 6: Run All Cells
Run all cells sequentially:
- Resume text extraction
- Embedding generation
- Similarity calculation
- Skill matching
- Ranking computation

### Step 7: View Output
The system generates:
- Ranked candidate list
- Similarity and skill scores
- CSV file containing final rankings


✅ Output

The project produces:
- Ranked resumes based on job relevance
- Matching score for each candidate
- Missing skills analysis
- Exportable recruiter-ready results file


🎯 Applications

- Automated Resume Screening
- HR Recruitment Assistance
- Applicant Tracking Systems (ATS)
- AI-powered Hiring Analytics




