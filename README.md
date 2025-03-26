# 🚀 Project Name

## 📌 Table of Contents
- [Introduction](#introduction)
- [Demo](#demo)
- [Inspiration](#inspiration)
- [What It Does](#what-it-does)
- [How We Built It](#how-we-built-it)
- [Challenges We Faced](#challenges-we-faced)
- [How to Run](#how-to-run)
- [Tech Stack](#tech-stack)
- [Team](#team)

---

## 🎯 Introduction
A brief overview of your project and its purpose. Mention which problem statement are your attempting to solve. Keep it concise and engaging.

The objective is to develop an Mulit-agent Agentic AI email classifier, that can efficiently identify the service request type from email content, subject, and attachments. The solution leverages Gemini (or alternative LLaMA models) integrated with LangChain to classify emails based on predefined rules and keyword patterns.
While Generative AI (like Gemini, GPT, and LLaMA) focuses on content creation based on prompts, Agentic AI introduces a more dynamic and autonomous decision-making framework.

Agentic AI can:

✅ Break down complex tasks into smaller steps.

✅ Strategically decide which tools, APIs, or functions to use.

✅ Adapt to changing conditions during runtime.

✅ Maintain context and learn from previous actions.


## 🎥 Demo
🔗 [Live Demo](#) (if applicable)  
📹 [Video Demo](#) (if applicable)  
🖼️ Screenshots:

Email .eml file as input:

![image](https://github.com/user-attachments/assets/c7954877-9180-47ff-aca4-c8b2df91f798)

WORD Doc as Input:

![image](https://github.com/user-attachments/assets/2f7e722e-717b-4da8-b046-de315c9b6e57)


PDF Doc as Input:

![image](https://github.com/user-attachments/assets/bf6a451f-d339-4898-9fc5-3e4c914d16dc)


## 💡 Inspiration
What inspired you to create this project? Describe the problem you're solving.

Looking into the current challenges a bank as an organization faces, we observed that manually extracting content from email and classifying them into different categories is one of the tedious job a person has to do. Though the content might be different in terms of an email, but building a solution could also solve many such problems dealing with text classification.


## ⚙️ What It Does
Explain the key features and functionalities of your project.

The multi-agent AI architecture employed here follows a structured yet flexible design, where specialized agents are assigned distinct tasks. This method breaks down the email classification challenge into modular steps, improving accuracy, efficiency, and scalability.
Proposed solution uses agents performing:
	•  Input Extraction Agent (Content & Attachment Processor), Role: Extracts text from email bodies, attachments, and metadata
 
	•  Preprocessing Agent (Normalization & Cleaning), Role: Cleans and normalizes extracted text for consistency.
 
	• Classification Agent (Service Request Identifier), Role: Identifies the service request type based on content context.
 
	• Duplicate Detection Agent (Email Uniqueness Checker), Role: Prevents redundant email processing by identifying duplicates.
 
	• Confidence Scoring Agent (Trustworthiness Evaluator), Role: Assigns a confidence score to each classification based on content quality and keyword strength.

 	• Output Aggregator Agent (Result Builder), Role: Consolidates outputs from all agents to deliver a structured result.


## 🛠️ How We Built It
Briefly outline the technologies, frameworks, and tools used in development.

Development phases:
**Phase 1:** Requirement Analysis & Problem Understanding:
Went through the hackathon problem statement & sample templates of emails along with output format that’s expected to accurately classify emails into service request types (e.g., AU Transfer, Fee Payment, etc.). Detect duplicate emails to reduce redundant processing.  Handle content from both email bodies and attachments.

**Phase2:** Data Collection & Preparation:
Googled and found different templates for commercial banking service requests
Used ChatGPT to generate some of the data samples in required file formats of .docx, .pdf & .eml files with & without attachments

**Phase 3:** Designed a Multi-agent system using LLM models to generate. Here are the core agents:

	• Input Extraction Agent: Extracts content from email bodies and attachments.
	• Preprocessing Agent: Normalizes content for improved accuracy.
	• Classification Agent: Uses Gemini or LLaMA for intelligent content analysis.
	• Duplicate Detection Agent: Flags repeated content using hashing or semantic comparison.
	• Confidence Scoring Agent: Evaluates model certainty for accurate prioritization.

**Phase 4:** Model Selection & Fine-Tuning. 
Based on the prompt results, we opted for Gemini Pro model for advanced NLU when compared with llama2 models output.
For Prompt Engineering: Created detailed prompts for optimal classification.
Design rules for keywords like “AU Transfer,” “Fee Payment,” etc.

**Phase 5:** LangChain & Streamlit Integration
LangChain was used to streamline the prompt engineering, LLM interaction, and classification logic.
The chain was used to process extracted email content and generate predictions.
Streamlit was used to build an interactive UI for seamless user interaction, testing, and result visualization.


## 🚧 Challenges We Faced
Describe the major technical or non-technical challenges your team encountered.

## 🏃 How to Run
1. Clone the repository  
   ```sh
   git clone https://github.com/your-repo.git
   ```
2. Install dependencies  
   ```sh
   npm install  # or pip install -r requirements.txt (for Python)
   ```
3. Run the project  
   ```sh
   npm start  # or python app.py
   ```

## 🏗️ Tech Stack
- 🔹 Frontend: React / Vue / Angular
- 🔹 Backend: Node.js / FastAPI / Django
- 🔹 Database: PostgreSQL / Firebase
- 🔹 Other: OpenAI API / Twilio / Stripe

## 👥 Team
- **Your Name** - [GitHub](#) | [LinkedIn](#)
- **Teammate 2** - [GitHub](#) | [LinkedIn](#)
