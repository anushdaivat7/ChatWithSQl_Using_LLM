**ChatWithSQl_Using_LLM**

An AI-powered SQL Assistant that allows you to chat with your SQLite or MySQL database using natural language.
Built using LangChain, Groq Llama 3.1 models, and Streamlit, the app automatically converts your query into SQL, executes it, and returns results — in real time.

**🚀 Features**

✅ Chat with your database (SQLite or MySQL)
✅ Converts Natural Language → SQL → Result
✅ Uses Groq’s Llama 3.1 models for fast and accurate reasoning
✅ Clean Streamlit UI
✅ SQL Agent handles schema understanding & SQL planning
✅ Supports streaming responses
✅ Error-handling enabled (handle_parsing_errors=True)

**🛠️ Tech Stack**

Backend & AI

Python 3.10

LangChain 0.1.14

LangChain SQL Agent

Groq LLM (llama-3.1-8b-instant)

SQLAlchemy

SQLite / MySQL

Frontend

Streamlit UI


**📁 Project Structure**
ChatWithSQL_Using_LLM/
│
├── app.py
├── student.db                # example SQLite DB (optional)
├── requirements.txt
├── README.md
└── .gitignore

**⚙️ Installation & Setup**
1️⃣ Clone the Repository
git clone https://github.com/anushdaivat7/ChatWithSQl_Using_LLM.git
cd ChatWithSQl_Using_LLM

2️⃣ Install Dependencies
pip install -r requirements.txt

3️⃣ Run the App
streamlit run app.py

4️⃣ Add Your Groq API Key

The app will ask for GROQ_API_KEY in the left sidebar.

🧠 How It Works

User asks:
“Show all students who scored above 80.”

LLM selects appropriate tool using ReAct format

SQL Agent generates SQL:

SELECT * FROM students WHERE marks > 80;


Database executes query

Results returned back to user

No SQL knowledge needed — the LLM handles everything.

🗄️ Database Support
SQLite

✔ Built-in student.db
✔ No setup required

MySQL

Enter:

Host

Username

Password

DB Name

The agent automatically connects and queries.

