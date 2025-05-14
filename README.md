                                                   AI Resume Analyzer
AI Resume Analyzer is a web application that analyzes resumes using Natural Language Processing (NLP) techniques to recommend career fields and courses. It uses libraries like spaCy, NLTK, and PyResparser to extract meaningful data from resumes and matches them with relevant skills.

Live Demo
Currently not deployed. Run locally with Streamlit (instructions below).

Features
•	Upload PDF resume
•	Extracts:
      o	Name, Email, Phone, Skills
      o	Number of Pages
•	Predicts Candidate Level (Beginner/Intermediate/Experienced)
•	Recommends:
      o	Field of interest
      o	Relevant skills
      o	Recommended courses
•	Admin dashboard for activity monitoring

Tech Stack
•	Frontend: Streamlit
•	Backend: Python, spaCy, NLTK, PyResparser
•	Database: MySQL
•	Libraries: pandas, pymysql, pdfminer, PIL

Folder Structure
AI-Resume-Analyzer/
├── App/
│   ├── App.py                # Main Streamlit app
│   ├── style.css             # Custom CSS for styling
│   └── Admin.py              # Admin dashboard
├── Logo/
│   └── RESUM.png             # Banner image
├── Uploaded_Resumes/        # Uploaded PDF files
├── Assets/                  # Additional assets like icons
├── README.md
└── requirements.txt         # Required Python libraries

How to Run Locally
Step 1: Clone the Repo
        git clone https://github.com/Nihareeka40/AI-Resume-Analyzer.git
        cd AI-Resume-Analyzer
Step 2: Create Virtual Environment (Windows)
        python -m venv venv
        venv\Scripts\activate
Step 3: Install Dependencies
        pip install -r requirements.txt
        python -m nltk.downloader stopwords
        python -m spacy download en_core_web_sm
Step 4: Start MySQL Server
        Make sure MySQL is running on port 3306 and the cv database exists. Update credentials in App.py:
        pymysql.connect(host='localhost', user='root', password='yourpassword', db='cv')
Step 5: Run the App
        streamlit run App/App.py

Author
•	Nihareeka Makwana
•	Email: nmmakwana031@gmail.com
•	GitHub: Nihareeka40
•	College: Charotar University of Science and Technology (CHARUSAT)

License
This project is open-source and free to use.

