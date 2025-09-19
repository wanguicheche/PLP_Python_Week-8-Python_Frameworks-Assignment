# 📊 CORD-19 Research Data Explorer

This project analyzes the **CORD-19 dataset** (COVID-19 research papers) using Python (pandas, matplotlib) and presents findings in an interactive **Streamlit app**.

---

## 🚀 Project Overview
- **Dataset**: `metadata.csv` from [CORD-19 Kaggle dataset](https://www.kaggle.com/allen-institute-for-ai/CORD-19-research-challenge)  
- **Goals**:
  1. Load & explore real-world research data
  2. Clean and prepare the dataset
  3. Analyze publication trends, journals, and keywords
  4. Build a simple interactive **Streamlit app**
  5. Reflect on challenges and insights  

---

## 📂 Repository Structure
├── analysis.ipynb # Notebook with Parts 1–3 (exploration, cleaning, analysis)
├── app.py # Streamlit app (Part 4)
├── cord19_clean_sample.csv # Cleaned sample dataset (<100 MB)
├── requirements.txt # Python dependencies
└── README.md # Project documentation

📒 Run the Notebook (Parts 1–3)
Open analysis.ipynb in VS Code.
You’ll find:
Part 1: Data loading & exploration
Part 2: Data cleaning & preparation
Part 3: Analysis & visualizations

🌐 Run the Streamlit App (Part 4)





📊 Features in the App
Filter research papers by year range
View publication counts per year
Explore top journals publishing COVID-19 research
Preview a sample of the dataset interactively

📝 Reflection (Part 5)
## Challenges
- Large file size → solved with `nrows` sampling.
- Messy/absent dates → handled via `errors='coerce'`.
- Many nulls in some columns → dropped where necessary; filled journals with "Unknown".
- Streamlit was not running -> Finally managed to get it started on GitBash then copied the network url to Microsoft Edge browser to view it.

## What I learned
- Practical pandas cleaning steps (dates, nulls, new features).
- Basic visualization in matplotlib.
- Building a minimal Streamlit dashboard from a cleaned CSV.
- Gitbash doesn't recognize long paths, thus quote marks are needed.
- Need to understand what each line of code represents and does.
- Streamlit cannot be viewed from my local machine or network, thus it's easier to deploy it online.
