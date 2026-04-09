📝 AI‑Powered Resume Screening & Candidate Matching Assistant
A lightweight, intelligent resume analysis tool that extracts key skills, evaluates candidate relevance, and matches applicants to job descriptions using modern NLP techniques.

Designed to demonstrate practical AI applications in HR automation, talent filtering, and document understanding.

🚀 Key Features
🔍 1. Automatic Resume Parsing
Extracts:

Skills

Experience

Education

Technical keywords

Relevant achievements

Works with PDF or text resumes.

🤖 2. Job Description Matching
Compares each resume against a job description and generates:

A relevance score

A strengths summary

A gap analysis

A suitability verdict

🧠 3. AI‑Generated Insights
Provides human‑like explanations such as:

“This candidate is a strong match because they have 3+ years of Python experience and direct exposure to NLP workflows.”

🧹 4. Clean, Structured Output
Each evaluation includes:

Extracted skills

Match score

Summary

Missing skills

Final recommendation

Perfect for HR dashboards, automated hiring tools, or internal screening systems.

🧰 Tech Stack
Component	Technology
LLM	phi‑3 via Ollama
NLP Framework	LangChain
Document Parsing	PyMuPDF
Vector Store	ChromaDB
Frontend	Gradio
Language	Python

📁 Project Structure
Code
📦 Resume Screener
 ┣ 📂 resumes/                # Input resumes
 ┣ 📂 chroma_resu/            # Vector database
 ┣ 📜 resume_screener.py      # Main application
 ┣ 📜 requirements.txt        # Dependencies
 ┣ 📜 README.md               # Documentation
⚙️ How It Works
Load Resume Files  
PDFs are parsed and cleaned.

Chunk & Embed  
Resume content is split into semantic chunks and embedded.

Store in ChromaDB  
Embeddings are indexed for fast similarity search.

Match Against Job Description  
The LLM generates:

A match score

A summary

Missing skills

A final recommendation

Serve via Gradio UI  
Users upload resumes and job descriptions through a simple interface.

🧪 Use Cases
HR automation

Candidate pre‑screening

Internal hiring tools

Talent filtering

Resume‑to‑job matching systems

📦 Installation
bash
pip install -r requirements.txt
Make sure Ollama is installed and running:

bash
ollama serve
ollama pull phi3
▶️ Run the App
bash
python resume_screener.py
🌟 Why This Project Matters
Recruiters spend hours manually reading resumes.
This tool shows how AI can:

Reduce manual workload

Improve consistency

Highlight top candidates

Speed up hiring decisions

It’s a practical demonstration of how NLP can transform HR workflows.
