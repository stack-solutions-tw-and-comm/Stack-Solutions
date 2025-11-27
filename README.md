# STACK SOLUTIONS

**Financial Investment Website for Consulting Users on their Investment Decisions**

---

## Project Documentation

This section provides links to all project-related documentation, including wiki pages and in-repository drafts.

### Wiki

* [Wiki Home](../../wiki)
* [Design (Wiki)](../../wiki/Design)
* [Proposal (Wiki)](../../wiki/Proposal)

### In-Repo Drafts (Reviewed via PRs)

* [Design: User Stories & Acceptance](Project%20Docs/Wiki/Design/user-stories.md)
* [Design: Architecture & Components](Project%20Docs/Wiki/Design/Architecture.md)
* [Design: Data & Content](Project%20Docs/Wiki/Design/data-content.md)
* [Design: Risks & Constraints](Project%20Docs/Wiki/Design/risks-constraints.md)

---

## Usage Guide: How to Run Stack Capital Locally

This guide explains how to set up and run the Stack Capital Investment Dashboard on your local machine. The application requires **Node.js** and **Python** to be installed.

### Steps to Run

1.  **Install Dependencies:**
    Ensure all required Node.js packages (Express, etc.) are installed by running the following command in your terminal (e.g., Git Bash, Command Prompt, or PowerShell):
    ```bash
    npm install
    ```

2.  **Start the Server:**
    Launch the **Node.js server** (`server.js`), which handles routing, serving static files, and executing the backend logic.
    ```bash
    node server.js
    ```

3.  **Access the Site:**
    Once the server is running, open your web browser and navigate to the following link to view the dashboard:
    [http://localhost:3000](http://localhost:3000)

    The application's homepage (`homepage.html`) will load, and the dashboard will be ready to use.

### Using Core Features

* **Risk Assessment:** Navigate to the Quiz page. When you submit your answers, the Node.js server executes the Python script (`quiz.py`) to process the data and return your risk profile.
* **Market News:** The homepage automatically fetches real-time financial data by having the server act as a proxy to the external Alpha Vantage API.

---

## Technology & Citation

This project uses a **Node.js server** (`server.js`) to connect front-end pages (`homepage.html`, `quiz.html`, `chatbot.html`) with backend logic (`quiz.py`).

### APIs and Other Components

| Component | Description | Citation |
| :--- | :--- | :--- |
| **Alpha Vantage Market News API** | Used by the Node.js server (`server.js`) to fetch real-time financial news and sentiment data. The API call is processed and data is filtered before serving to the client. | Vantage, A. (n.d.). *Free Stock APIs in JSON & Excel \| Alpha Vantage*. https://www.alphavantage.co/ |
| **Jotform Chatbot** | The AI Chatbot feature relies on an external Jotform embed script for conversational investment advice (`chatbot.html`). | EASIEST ONLINE FORM BUILDER. (n.d.). *Jotform*. https://www.jotform.com/ |

### Programming Languages & Frameworks

| Technology | Role | Citation |
| :--- | :--- | :--- |
| **Node.js / Express** | Used for the server environment, routing, and handling API proxy calls (`server.js`). | Node.js — Run JavaScript everywhere. (n.d.). https://nodejs.org/en <br> Express - Node.js web application framework. (n.d.). https://expressjs.com/ |
| **Python** | Utilized for the Risk Assessment logic (`quiz.py`), processing user input and calculating the risk profile. | |
| **HTML/CSS/JavaScript** | Core technologies for responsive front-end design and user interaction. | |

---

## Teamwork Process

The team adopted an **Agile (Scrum-based)** software development approach to manage the project. This methodology allows for flexibility, quick feature iteration, and rapid adjustments based on weekly feedback.

### Team Structure and Roles

The team consists of four members, with defined roles to ensure clear responsibilities:

* **Coordinator/Facilitator:** Pranav Gusain
* **Scribe/Documentation:** Aaden
* **QA/Reviewer:** Tony
* **Dev/Prototype Lead:** Mahad Ramzi

### Communication and Conflict Plan

A clear communication strategy was established to maintain continuous progress:

| Area | Details |
| :--- | :--- |
| **Meetings** | Quick check-in **Stand-ups** during lab sessions and a **Weekly Lab Brief** for status updates and progress review. |
| **Channels** | Communication is maintained across **MS Teams, iMessage, and Email**. |
| **Conflict Resolution** | Conflicts are first discussed as a **group**; if unresolved, they are escalated to the professor. |
| **Response Time** | All team members committed to a response time of within **24 hours**. |
