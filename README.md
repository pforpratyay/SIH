# 🕵️ Trace-X — AI-Powered Criminal Network Analysis System

### Evidence-Driven Criminal Intelligence & Network Investigation Platform

\<p align="center">
&#x20; \<a href="[https://sih-project-1-yrjs.onrender.com](https://sih-project-1-yrjs.onrender.com)">
&#x20;   \<img src="[https://img.shields.io/badge/Live%20Demo-Open%20Application-00C853?style=for-the-badge](https://img.shields.io/badge/Live%20Demo-Open%20Application-00C853?style=for-the-badge)" />
&#x20; \</a>
&#x20; \<a href="[https://github.com/pforpratyay/SIH](https://github.com/pforpratyay/SIH)">
&#x20;   \<img src="[https://img.shields.io/badge/GitHub-Repository-181717?style=for-the-badge&logo=github](https://img.shields.io/badge/GitHub-Repository-181717?style=for-the-badge\&logo=github)" />
&#x20; \</a>
\</p>

\<p align="center">
&#x20; \<img src="[https://img.shields.io/badge/React-19-61DAFB?logo=react](https://img.shields.io/badge/React-19-61DAFB?logo=react)" />
&#x20; \<img src="[https://img.shields.io/badge/Node.js-Backend-339933?logo=nodedotjs](https://img.shields.io/badge/Node.js-Backend-339933?logo=nodedotjs)" />
&#x20; \<img src="[https://img.shields.io/badge/Express-5-000000?logo=express](https://img.shields.io/badge/Express-5-000000?logo=express)" />
&#x20; \<img src="[https://img.shields.io/badge/MongoDB-Database-47A248?logo=mongodb](https://img.shields.io/badge/MongoDB-Database-47A248?logo=mongodb)" />
&#x20; \<img src="[https://img.shields.io/badge/Python-AI%20Service-3776AB?logo=python](https://img.shields.io/badge/Python-AI%20Service-3776AB?logo=python)" />
\</p>

**Smart India Hackathon 2026 | Team Xenon | SIH26189**

---

## 🌐 Project Links

| Resource             | Link                                                                               |
| -------------------- | ---------------------------------------------------------------------------------- |
| Live Application     | [https://sih-project-1-yrjs.onrender.com](https://sih-project-1-yrjs.onrender.com) |
| GitHub Repository    | [https://github.com/pforpratyay/SIH](https://github.com/pforpratyay/SIH)           |
| AI Reasoning Service | [https://trace-x-d6ss.onrender.com](https://trace-x-d6ss.onrender.com)             |
| API Documentation    | Not publicly available yet                                                         |
| Demo Video           | Coming soon                                                                        |

---

## 📌 Overview

**Trace-X** is an AI-powered criminal network analysis and investigative intelligence platform designed to transform fragmented investigative information into structured, explainable, and evidence-backed relationships.

The platform aims to help investigators analyze heterogeneous datasets, identify entities, discover potential connections, and understand complex criminal networks through interactive visualization and evidence traceability.

It integrates investigative records such as FIR reports, call detail records (CDRs), and other structured or unstructured information through an AI-assisted processing pipeline.

The system emphasizes evidence-backed relationships, confidence-based analysis, explainability, and human verification.

**Core Philosophy:** Every investigative relationship should be traceable to its supporting evidence. AI-generated hypotheses must remain distinguishable from verified findings.

## 🎯 Problem Statement

Investigative agencies often work with fragmented information distributed across multiple reports, records, and datasets.

Major challenges include:

- Unstructured investigative documents.
- Large-scale call detail records.
- Duplicate identities and multiple aliases.
- Hidden relationships across investigative records.
- Difficulties correlating information from different sources.
- Limited traceability of automatically identified relationships.

Trace-X aims to provide a centralized analytical environment to organize, connect, and investigate such information.

## ✨ Key Features

### 🔐 Investigator Authentication

- JWT-based authentication.
- Password hashing using bcrypt.
- Protected backend routes.
- Investigator session management.

### 📂 Investigative Data Processing

- Case intake through the backend.
- CSV file upload and parsing.
- Structured and unstructured report processing.
- Input validation and data normalization.

### 🧠 AI-Assisted Intelligence Processing

- Entity extraction.
- Entity resolution.
- Relationship identification.
- Pattern analysis.
- Evidence-linked analytical results.

### 🕸️ Criminal Network Analysis

- Entity and relationship representation.
- Graph-based investigation.
- Relationship confidence information.
- Evidence and guardrail information.

### ⏳ Timeline & Investigation Insights

- Chronological investigative information.
- Entity-level relationship inspection.
- Case-specific analytical results.

### ⚠️ Explainability & Human Verification

- Supporting evidence for identified relationships.
- Confidence-based assessment.
- Uncertain associations requiring human review.
- AI-generated findings treated as investigative leads rather than established facts.

*Feature implementation and integration status may vary across application modules. Refer to the current repository implementation.*

## 🏗️ System Architecture

```text
             INVESTIGATIVE DATA
          FIR | CDR | CSV | Reports
                    |
                    v
             REACT FRONTEND
             Vite + Tailwind
                    |
                    v
              EXPRESS API
             Node.js Backend
                    |
          ---------------------
          |                   |
          v                   v
       MongoDB           FastAPI AI
       Database          Reasoning
          |                   |
          |             Entity Extraction
          |             Relationship Analysis
          |             AI Processing
          |                   |
          <-------------------
                    |
                    v
          EVIDENCE-LINKED RESULTS
                    |
                    v
           INVESTIGATION SYSTEM
```

The AI reasoning service is maintained separately from this repository and communicates with the Node.js backend through HTTP APIs.

## 🛠️ Technology Stack

| Category            | Technologies                       |
| ------------------- | ---------------------------------- |
| Frontend            | React 19, JavaScript               |
| Build Tool          | Vite                               |
| Styling             | Tailwind CSS 4                     |
| Graph Visualization | React Force Graph 3D, XYFlow       |
| Backend             | Node.js, Express.js 5              |
| Database            | MongoDB, Mongoose                  |
| Authentication      | JWT, bcryptjs                      |
| File Processing     | Multer, csv-parse                  |
| API Communication   | Axios, REST APIs                   |
| AI Service          | Python, FastAPI (external service) |
| Deployment          | Render                             |
| Version Control     | Git, GitHub                        |

## 📁 Project Structure

```text
SIH/
│
├── frontend/
│   ├── public/
│   ├── src/
│   │   ├── api/
│   │   ├── components/
│   │   ├── pages/
│   │   ├── state/
│   │   └── ...
│   ├── package.json
│   └── vite.config.js
│
├── server/
│   ├── config/
│   ├── src/
│   │   ├── controllers/
│   │   ├── middleware/
│   │   ├── models/
│   │   ├── routes/
│   │   ├── services/
│   │   └── utils/
│   ├── tests/
│   ├── package.json
│   ├── server.js
│   └── .env.example
│
├── PROJECT_INTEGRATION_AUDIT.md
├── render.yaml
├── .gitignore
└── README.md
```

## 🚀 Installation & Setup

### Prerequisites

Install the following software:

| Software      | Download                                                                                           |
| ------------- | -------------------------------------------------------------------------------------------------- |
| Git           | [https://git-scm.com/downloads](https://git-scm.com/downloads)                                     |
| Node.js (LTS) | [https://nodejs.org/en/download](https://nodejs.org/en/download)                                   |
| MongoDB       | [https://www.mongodb.com/try/download/community](https://www.mongodb.com/try/download/community)   |
| MongoDB Atlas | [https://www.mongodb.com/products/platform/atlas](https://www.mongodb.com/products/platform/atlas) |
| VS Code       | [https://code.visualstudio.com/download](https://code.visualstudio.com/download)                   |

### Step 1: Clone the Repository

```bash
git clone https://github.com/pforpratyay/SIH.git

cd SIH
```

### Step 2: Setup Backend

```bash
cd server

npm install
```

Create a `.env` file inside the `server` directory using `.env.example` as the template.

Configure the following variables:

```env
PORT=5000
NODE_ENV=development

MONGODB_URI=your_mongodb_connection_string

FASTAPI_BASE_URL=http://127.0.0.1:8000
FASTAPI_TIMEOUT_MS=60000

FASTAPI_INTERNAL_SECRET=your_shared_secret

JWT_SECRET=your_secure_random_secret
JWT_EXPIRES_IN=15m

DEFAULT_INVESTIGATOR_USERNAME=your_username
DEFAULT_INVESTIGATOR_PASSWORD=your_password
```

Replace the example values with your actual configuration.

The FastAPI service must be available at the configured URL for case-processing requests.

Start the backend:

```bash
npm run dev
```

Backend default address:

```text
http://localhost:5000
```

Health check:

```text
http://localhost:5000/health
```

### Step 3: Setup Frontend

Open another terminal:

```bash
cd frontend

npm install
```

Start the frontend:

```bash
npm run dev
```

Frontend default address:

```text
http://localhost:3000
```

### Step 4: Configure AI Reasoning Service

The AI reasoning service is an external component and is not included as a runnable Python application in this repository.

For local development, configure `FASTAPI_BASE_URL` with the actual FastAPI service address and ensure its shared secret matches the backend configuration when authentication is enabled.

The currently configured deployed reasoning-service address is:

[https://trace-x-d6ss.onrender.com](https://trace-x-d6ss.onrender.com)

### Step 5: Access the Application

Open:

[https://sih-project-1-yrjs.onrender.com](https://sih-project-1-yrjs.onrender.com)

For local development:

[http://localhost:3000](http://localhost:3000)

## 📡 Backend API

The backend provides REST API functionality for investigator authentication and case-related operations.

| Method | Endpoint                                | Purpose                        |
| ------ | --------------------------------------- | ------------------------------ |
| GET    | `/`                                     | Backend service information    |
| GET    | `/health`                               | Health check                   |
| POST   | `/api/auth/login`                       | Investigator login             |
| GET    | `/api/auth/verify`                      | Token verification             |
| POST   | `/api/cases`                            | Case intake                    |
| GET    | `/api/cases/:caseId/graph`              | Retrieve case graph            |
| GET    | `/api/cases/:caseId/entities/:entityId` | Entity details                 |
| GET    | `/api/cases/:caseId/timeline`           | Timeline information           |
| GET    | `/api/cases/:caseId/guardrail/:edgeId`  | Evidence and guardrail details |

Authenticated routes require a valid JWT access token.

Interactive Swagger documentation is not currently published.

## 🔄 Application Workflow

1. **Investigator Authentication:** Authenticate through the login interface.
2. **Data Submission:** Submit authorized investigative reports or supported CSV files.
3. **Backend Processing:** Validate and normalize the submitted data.
4. **AI Reasoning:** Forward the processed information to the external reasoning service.
5. **Intelligence Generation:** Receive structured entities, relationships, patterns, and evidence.
6. **Database Persistence:** Store case-specific investigative results.
7. **Network Analysis:** Retrieve graph and entity information through backend APIs.
8. **Investigator Review:** Examine evidence and review uncertain findings.

## 🔐 Security & Responsible AI

Trace-X is designed as an investigative decision-support system.

Security and responsible AI considerations include:

- JWT-based authentication.
- Password hashing.
- Protected investigative endpoints.
- Case-specific data isolation.
- Input validation and file restrictions.
- Evidence traceability.
- Human review of uncertain relationships.
- Secure handling of sensitive information.

AI-generated associations must not be interpreted as proof of criminal activity or guilt.

All consequential findings require independent verification and appropriate human judgment.

## 🧪 Testing

The backend repository contains automated test scripts covering important areas such as:

- Authentication.
- Case intake.
- Graph retrieval.
- Entity details.
- Timeline retrieval.
- Evidence and guardrail handling.
- FastAPI integration failure scenarios.

Run the available backend test scripts using the instructions documented in `server/tests/`.

## 🚧 Current Development Status

The project is under active development.

Some backend APIs and authentication functionality are implemented, while several frontend investigative workflows and the external AI service integration require further development and verification.

The complete production-ready end-to-end workflow is not yet claimed.

## 🔮 Future Scope

- Advanced graph analytics.
- Improved entity resolution.
- Multilingual document processing.
- Advanced relationship discovery.
- Scalable CDR processing.
- Enhanced investigation timelines.
- Explainable AI improvements.
- Blockchain-based evidence integrity and auditability.
- More comprehensive investigator dashboard integration.


## 🤝 Contributing

Contributions and suggestions are welcome.

1. Fork this repository.
2. Create a feature branch.
3. Implement your changes.
4. Test your changes.
5. Submit a pull request with a clear description.

Never commit credentials, confidential records, or sensitive investigative information.

## 📜 License

No open-source license has been specified yet.

All rights remain with the respective project owners until a license is formally added.

## ⚠️ Disclaimer

This project is developed for research, educational, and investigative decision-support purposes.

It does not independently establish criminal liability or replace authorized investigative procedures.

AI-generated findings must be independently reviewed and verified.

---

\<p align="center">   \<b>TRACE-X | TEAM XENON\</b>   \<br/>   Turning fragmented intelligence into explainable investigative insights.   \<br/>\<br/>   \<a href="[https://github.com/pforpratyay/SIH](https://github.com/pforpratyay/SIH)">GitHub Repository\</a> |   \<a href="[https://sih-project-1-yrjs.onrender.com](https://sih-project-1-yrjs.onrender.com)">Live Application\</a> \</p>
