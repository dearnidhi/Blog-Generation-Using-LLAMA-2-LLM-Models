A local blog generation app built with Streamlit and LLaMA 2, allowing users to generate topic-based blogs in different writing styles using an offline large language model.

# Blog Generator using LLaMA 2 📝🤖

This project is a **blog generation application** built using **Streamlit** and a **locally running LLaMA 2 model** via CTransformers.

It allows users to generate blogs for different audiences by specifying:
- Blog topic
- Number of words
- Writing style

The model runs **fully offline**, making it suitable for local experimentation and learning.

---

## 🚀 Features

- Blog generation using LLaMA 2
- Offline inference (no API required)
- Multiple writing styles
- Custom word-length control
- Simple and clean Streamlit UI

---

## 🧠 How It Works

1. User enters a blog topic
2. Selects target audience (style)
3. Specifies word count
4. LLaMA 2 generates a blog using a prompt template
5. Output is displayed in the UI

---

## 📂 Project Structure

```text
.
├── models/
│   └── llama-2-7b-chat.ggmlv3.q8_0.bin
├── app.py
├── requirements.txt
└── README.md

▶️ Setup Instructions
1️⃣ Clone the Repository
git clone https://github.com/your-username/your-repo-name.git
cd your-repo-name

2️⃣ Create Virtual Environment
python -m venv venv
source venv/bin/activate     # Windows: venv\Scripts\activate

3️⃣ Install Dependencies
pip install -r requirements.txt

🧠 Model Setup
Download the LLaMA 2 7B Chat (GGML) model and place it inside the models/ directory:
models/llama-2-7b-chat.ggmlv3.q8_0.bin
You must obtain the model from an authorized source (e.g. Hugging Face).

▶️ Run the Application
streamlit run app.py

🛠️ Tech Stack
Python
Streamlit
LangChain
CTransformers
LLaMA 2 (local inference)

⚠️ Notes
Designed for educational and local experimentation
Requires sufficient system RAM (LLaMA 2 is heavy)
Output quality depends on prompt and temperature settings
Not intended for production use
