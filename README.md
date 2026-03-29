#  Smart Resume–Job Matching Agent

##  Overview

This project builds an AI-based system that matches resumes with job descriptions using Natural Language Processing (NLP) techniques. The system preprocesses textual data, converts it into numerical representations, and computes similarity scores to recommend the most relevant jobs for each resume.

---

##  Objectives

* Automate resume-job matching
* Reduce manual hiring effort
* Improve recommendation accuracy
* Demonstrate NLP-based similarity modeling

---

##  Project Structure

project/
│
├── Resume.csv
├── training_data.csv
│
├── cleaned_resumes.csv
├── cleaned_jobs.csv
│
├── resume_vectors.pkl
├── job_vectors.pkl
│
├── matches.csv
├── top3_matches.csv
│
├── 01_data_preprocessing.ipynb
├── 02_feature_engineering.ipynb
├── 03_unsupervised_model.ipynb
├── 04_visualization.ipynb
├── 05_evaluation_ethics.ipynb
│
└── README.md

---

##  Technologies Used

* Python
* Pandas
* NumPy
* Scikit-learn
* NLTK
* Matplotlib

---

##  Dataset

* **Resume Dataset** → Contains resume text and categories
* **Job Dataset** → Contains job descriptions and job titles

---

##  Execution Order (IMPORTANT)

Run the notebooks in the following order:

1. `01_data_preprocessing.ipynb`

   * Cleans text data
   * Removes stopwords
   * Saves cleaned CSV files

2. `02_feature_engineering.ipynb`

   * Converts text into TF-IDF vectors
   * Saves vector files

3. `03_unsupervised_model.ipynb`

   * Computes cosine similarity
   * Generates best match and top-3 matches

4. `04_visualization.ipynb`

   * Plots similarity distributions

5. `05_evaluation_ethics.ipynb`

   * Calculates accuracy
   * Provides ethical analysis

---

##  Methodology

1. Text Cleaning

   * Lowercasing
   * Removing special characters
   * Removing stopwords

2. Feature Engineering

   * TF-IDF Vectorization

3. Matching Model

   * Cosine Similarity

4. Ranking

   * Top-1 and Top-3 job recommendations

---

##  Output

* Best job match for each resume
* Top-3 ranked job recommendations
* Similarity scores
* Visualization graphs

---

##  Evaluation

* Threshold-based accuracy calculation
* Statistical insights (mean, max, min scores)

---

##  Ethical Considerations

* Possible bias due to keyword-based matching
* Lack of explainability in model decisions
* Should assist, not replace human recruiters
* Fairness and transparency must be ensured

---

##  How to Run

### Step 1: Install dependencies

pip install pandas numpy scikit-learn nltk matplotlib

### Step 2: Run Jupyter Notebook

jupyter notebook

### Step 3: Execute notebooks in order (as listed above)

---

