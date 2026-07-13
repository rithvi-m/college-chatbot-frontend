College Chatbot – Frontend

A WhatsApp-style chat interface for the college information chatbot, built with plain HTML and JavaScript and deployed on GitHub Pages.

Live demo: rithvi-m.github.io/college-chatbot-frontend
Backend repo: college-chatbot-backend

How it works

The frontend sends user messages to the FastAPI backend (deployed on Render), which runs a RAG pipeline over college information and returns a generated answer. The chat UI displays the conversation in a familiar messaging-app layout.

Tech stack


HTML — chat UI structure and styling
JavaScript — handles user input, API calls to the backend, and rendering chat messages


Project structure

FilePurposeindex.htmlMain chat interface — layout and stylingknowledge.jsHandles chat logic — sending queries to the backend and rendering responses

Setup

No build step needed — it's a static site.

bashgit clone https://github.com/rithvi-m/college-chatbot-frontend.git
cd college-chatbot-frontend

Open index.html directly in a browser, or serve it locally:

bashpython -m http.server 8000

Then visit http://localhost:8000.

Deployment

Hosted via GitHub Pages, deployed automatically from this repository.

Related

This is the frontend half of a full-stack RAG chatbot project. See the backend repo for the FastAPI + Groq + Hugging Face retrieval pipeline
