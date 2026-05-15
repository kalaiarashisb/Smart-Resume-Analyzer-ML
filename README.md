# 💼 Smart Resume Analyzer and Job Match AI using Machine Learning

## 📌 Project Overview

Smart Resume Analyzer and Job Match AI is a Machine Learning and Natural Language Processing (NLP) based project developed to automate resume screening and predict resume-job compatibility scores.

The system analyzes candidate resumes, compares skills with job requirements, and predicts matching scores using Machine Learning algorithms. This project demonstrates the integration of NLP preprocessing, TF-IDF vectorization, Exploratory Data Analysis (EDA), and Random Forest Regression for intelligent recruitment analysis.

---

# 🚀 Features

✅ Resume and job description analysis  
✅ NLP-based text preprocessing  
✅ Missing value handling  
✅ Exploratory Data Analysis (EDA)  
✅ Skill extraction and visualization  
✅ TF-IDF text vectorization  
✅ Resume-job matching score prediction  
✅ Random Forest Regression model  
✅ WordCloud and skills visualization  

---

# 🛠️ Technologies Used

| Technology | Purpose |
|---|---|
| Python | Main programming language |
| Pandas | Data preprocessing and analysis |
| NumPy | Numerical computations |
| Scikit-learn | Machine Learning and NLP |
| Matplotlib | Data visualization |
| Seaborn | Statistical visualization |
| WordCloud | Skills visualization |
| Jupyter Notebook | Development environment |

---

# 📂 Dataset Description

The dataset contains resume information, candidate skills, educational qualifications, job requirements, and compatibility scores.

## Important Features Used

| Feature | Description |
|---|---|
| skills | Candidate technical skills |
| related_skils_in_job | Skills related to the target job |
| job_position_name | Job role |
| educational_requirements | Required qualification |
| experiencere_requirement | Required experience |
| skills_required | Required technical skills |
| matched_score | Resume-job compatibility score |

## 🎯 Target Variable

| Target Variable | Description |
|---|---|
| matched_score | Numerical score representing compatibility between resume and job description |

---

# 🧠 Machine Learning Workflow

<img width="459" height="809" alt="WhatsApp Image 2026-05-15 at 10 32 15 PM" src="https://github.com/user-attachments/assets/9e984bdc-83a0-4f38-9382-75c8c52f9f73" />


---

# 🧹 Data Preprocessing

Data preprocessing was performed to clean and prepare the dataset for Machine Learning.

### Preprocessing Steps

- Selecting important columns
- Handling missing values
- Removing noisy text
- Lowercase conversion
- Removing special characters
- Feature engineering
- Combining text columns

---

# ⚠️ Handling Missing Values

Missing values were handled using:

- Row removal using `dropna()`
- Mode imputation for categorical columns

This helped maintain dataset quality while minimizing information loss.

---

# 📊 Exploratory Data Analysis (EDA)

EDA was performed to understand recruitment trends and skill distributions.

## Visualizations Performed

- Missing values heatmap
- Match score distribution
- Top skills analysis
- WordCloud visualization
- Common job roles visualization

---

# ☁️ Skills WordCloud

The project visualizes the most frequently occurring skills using WordCloud.

### Common Skills Identified

- Python
- SQL
- Machine Learning
- Data Analysis
- Hadoop
- Java
- Power BI

---

# 🔍 Feature Engineering

Important text columns were combined into a single feature column to improve semantic understanding between resumes and job descriptions.

Example:

```python
df['combined_text'] = (
    df['skills'].astype(str) + " " +
    df['related_skils_in_job'].astype(str) + " " +
    df['skills_required'].astype(str) + " " +
    df['job_position_name'].astype(str)
)
```

---

# ⚙️ TF-IDF Vectorization

Machine Learning models cannot directly process text data. Therefore TF-IDF Vectorization was used to convert textual information into numerical feature vectors.

### Why TF-IDF?

- Identifies important terms
- Reduces impact of common words
- Improves prediction performance
- Converts text into machine-readable format

---

# 🤖 Machine Learning Model

## Random Forest Regressor

Random Forest Regression was used to predict resume-job compatibility scores.

### Why Random Forest?

✅ Handles high-dimensional data  
✅ Reduces overfitting  
✅ Provides better prediction accuracy  
✅ Works effectively with NLP vectorized data  

---

# 📈 Model Evaluation

The model performance was evaluated using regression metrics.

| Metric | Value |
|---|---|
| Mean Absolute Error (MAE) | 0.078 |
| Root Mean Squared Error (RMSE) | 0.106 |

### Interpretation

- Low MAE indicates low average prediction error
- Low RMSE indicates accurate prediction capability
- The model effectively predicts resume-job matching scores

---

# 💡 Sample Prediction

### Resume Skills

```text
Python SQL Machine Learning
```

### Job Skills

```text
Python SQL Power BI
```

### Predicted Match Score

```text
0.82
```

Meaning:
> The resume has approximately 82% compatibility with the job requirements.

---

# 📸 Project Screenshots

## 📊 Match Score Distribution
<img width="720" height="558" alt="WhatsApp Image 2026-05-15 at 10 34 02 PM" src="https://github.com/user-attachments/assets/7271418b-624d-4b76-903f-02558872edbe" />


---

## 📈 Top Skills Visualization
<img width="760" height="453" alt="WhatsApp Image 2026-05-15 at 10 34 51 PM" src="https://github.com/user-attachments/assets/7a0d6ed3-4b52-47e3-a691-8da51b0b9458" />


---



# 💼 Real-World Applications

- AI-based recruitment systems
- ATS (Applicant Tracking Systems)
- Resume screening automation
- HR analytics platforms
- Job recommendation systems
- Skill matching systems

---

# 🔮 Future Enhancements

Future improvements can include:

- BERT and Transformer-based NLP models
- Deep Learning approaches
- Streamlit/Flask deployment
- Real-time resume upload system
- Interview recommendation system
- Skill gap analysis dashboard

---

# ▶️ Installation

## 1️⃣ Clone Repository

```bash
git clone https://github.com/your-username/Smart-Resume-Analyzer-ML.git
```

---

## 2️⃣ Install Dependencies

```bash
pip install -r requirements.txt
```

---

## 3️⃣ Run Jupyter Notebook

```bash
jupyter notebook
```

---

# 📦 Requirements

```text
pandas
numpy
scikit-learn
matplotlib
seaborn
wordcloud
jupyter
```

---

# 👨‍💻 Author

## Kalaiarashi S B

🎓 M.Tech (CSE) – II Year  
🏫 Sri Krishna College of Engineering and Technology  
📚 Domain: Data Science

---

# ⭐ Conclusion

This project successfully demonstrates how Machine Learning and NLP techniques can automate resume analysis and job matching tasks.

The system performs:
- Data preprocessing
- Missing value handling
- Text cleaning
- Exploratory Data Analysis
- TF-IDF vectorization
- Random Forest Regression

to effectively predict resume-job compatibility scores.

The low MAE and RMSE values indicate good prediction performance, making the project suitable for intelligent recruitment and AI-based resume screening systems.
