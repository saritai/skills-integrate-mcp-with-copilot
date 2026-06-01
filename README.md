# Integrate MCP with Copilot

A hands-on [GitHub Skills](https://skills.github.com) exercise for learning how to integrate Model Context Protocol (MCP) servers with GitHub Copilot.

## About the Project

This project is a **Mergington High School Activities API** — a FastAPI application that allows students to view and sign up for extracurricular activities. It serves as the sample application used to practice integrating MCP tools with Copilot.

### What You Learn

- How MCP servers expose tools that Copilot can use
- How to connect an MCP server to GitHub Copilot
- How Copilot interacts with APIs through MCP tool calls

## Tech Stack

- **Backend**: Python, [FastAPI](https://fastapi.tiangolo.com/), Uvicorn
- **Frontend**: Static HTML/CSS/JS served by FastAPI

## Getting Started

1. Install dependencies:

   ```bash
   pip install -r requirements.txt
   ```

2. Run the server:

   ```bash
   uvicorn src.app:app --reload
   ```

3. Open http://localhost:8000 for the UI, or http://localhost:8000/docs for the interactive API docs.

## API Endpoints

| Method | Endpoint | Description |
|--------|----------|-------------|
| GET | `/activities` | List all extracurricular activities |
| POST | `/activities/{name}/signup?email=...` | Sign up a student for an activity |
| DELETE | `/activities/{name}/unregister?email=...` | Unregister a student from an activity |

## Project Structure

```
├── src/
│   ├── app.py          # FastAPI application
│   └── static/         # Frontend (HTML, CSS, JS)
├── tests/              # Test files
├── requirements.txt    # Python dependencies
└── README.md
```

## Original Exercise

This repo was created from a [GitHub Skills exercise](https://github.com/saritai/skills-integrate-mcp-with-copilot/issues/1) on integrating MCP with Copilot.

