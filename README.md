# CSULB-CS-343-26-Fall: Introduction to Modern Software Engineering

**Course Description:**
This course provides a comprehensive introduction to the fundamental principles and practices of software engineering. Students will move beyond simple programming to understand the entire software development lifecycle, from requirements gathering and system design to implementation, testing, deployment, and maintenance. The course covers modern processes, tools, and methodologies used in the industry to build robust, scalable, and maintainable software.

**Core Learning Objectives:**
Upon successful completion of this course, you will be able to:
* Explain key software development processes like Agile and Scrum.

* Elicit and document software requirements and model systems using UML.

* Understand and apply fundamental software architecture patterns (MVC) and object-oriented design principles (SOLID).

* Distributed system, CAP principle, micro-service, cloud computing and containerization.

* Implement various software testing strategies and understand the concept of technical debt.

* Utilize essential modern tooling for version control (Git), Virtual Environment Manager in Python, and CI/CD (Jenkins).

* Discuss project management, risk management, and estimation techniques.

* Mastering vibe coding and harness engineering.

  ---

  **Primary Toolchain:**
  
* **Language & Ecosystem:** Python3, Streamlit FastAPI Django

* **IDE:** Jetbrains Pycharm

* **Build & Dependency Management:** pip conda uv

* **Version Control:** Git & GitHub

* **Modeling:** Draw.io, Mermaid, PDMaas

* **Project Management:** JIRA, Confluence

* **Database:** PostgreSQL Neo4J Milvus

* **CI/CD & DevOps:** Jenkins, Grafana, Prometheus

* **Test:** JMeter pytest

* ---

  

# Course Outline: Introduction to Modern Software Engineering

> *A 16‑week journey that blends core software engineering principles with AI‑augmented practices, balanced difficulty progression, and integrated professional soft skills.*

---

## Weekly Schedule

| Week | Date | Topic                                                | Details & Key Concepts                                       | Soft Skills Focus                                            |
| :--: | :--: | ---------------------------------------------------- | ------------------------------------------------------------ | ------------------------------------------------------------ |
|  1   | TBD  | **Foundations & Environment Setup**                  | Python 3, PyPI mirror, PyCharm, Git basics, PostgreSQL. Environment configuration (virtual environments, `.env`). **AI boost:** Use GitHub Copilot to scaffold a simple CLI project; practice prompt‑driven code generation. | **Team onboarding** – setting up shared repos, code style conventions, and initial communication channels. |
|  2   | TBD  | **Requirements Engineering & User Stories**          | Eliciting functional/non‑functional requirements, writing user stories with acceptance criteria. API contract design. **AI boost:** Use ChatGPT to generate story templates, refine ambiguous requirements, and create mock API responses. | **Active listening & interviewing** – role‑play stakeholder meetings to clarify vague requests from the PM. |
|  3   | TBD  | **Visual Modeling with UML**                         | DBA Database modeling. Backend service class, sequence,  and activity diagrams. Tools: Draw.io, Mermaid. **AI boost:** Generate Mermaid code from natural‑language descriptions; use AI to validate diagram consistency. | **Visual communication** – present system design to non‑technical peers using clear diagrams. |
|  4   | TBD  | **Software Architecture & Structural Patterns**      | Monolith, distributed systems(CAP), microservices, cloud technology, containerization (Docker). RESTful vs. GraphQL. **AI boost:** Use AI to compare architectural trade‑offs, generate Dockerfiles, and scaffold microservice skeletons. | **Decision‑making under uncertainty** – weigh CAP, on/off cloud technology selection trade‑offs and justify choices in a group debate. |
|  5   | TBD  | **Object‑Oriented Design & SOLID Principles**        | Deep dive into SOLID, common design patterns (Factory, Observer, Strategy). **AI boost:** Let AI suggest pattern candidates for given problems; use Codex to refactor code toward SOLID. | **Code reviews** – practice giving constructive feedback on design quality via GitHub. |
|  6   | TBD  | **Front‑end Fundamentals**                           | HTML5, CSS3, JavaScript (ES6+), introduction to Vue.js and React. Component‑based UI design and basic HCI. **AI boost:** Use AI to generate component design system. | **User‑centric thinking** – conduct a simple usability test and iterate based on feedback with survey design. |
|  7   | TBD  | **Back‑end Development & API Integration**           | Building RESTful APIs with Flask/FastAPI, database integration (SQLAlchemy), authentication (JWT). **AI boost:** AI‑assisted endpoint generation, automatic API documentation (Swagger), and test data creation. | **Cross‑team collaboration** – coordinate API test with another team via APIFOX. |
|  8   | TBD  | **Software Testing Strategies**                      | Unit testing (pytest), integration testing, black‑box, and load testing. Test coverage and mutation testing. **AI boost:** Generate test cases from code, use AI to find edge cases, and auto‑repair flaky tests. | **Quality culture** – write a testing manifesto and share lessons from a bug‑hunting session. |
|  9   | TBD  | **CI/CD & DevOps**                                   | Jenkins pipelines, GitHub Actions, container orchestration (Kubernetes basics). Monitoring with Grafana/Prometheus. **AI boost:** AI‑driven anomaly detection in logs; auto‑suggest pipeline failed deployment trouble shooting. | **Incident response** – simulate a deployment failure and practice calm, structured troubleshooting. |
|  10  | TBD  | **Software Reuse & Open Source**                     | Leveraging libraries, frameworks, and SDKs. Understanding open‑source licenses (MIT, GPL). **AI boost:** Use AI to recommend suitable libraries for a given task and assess license compatibility. | **Ethical reuse** – discuss attribution and community contribution etiquette. |
|  11  | TBD  | **Agile Project Management & Scrum**                 | Scrum roles, ceremonies, JIRA/Confluence workflows. Backlog refinement and sprint planning. **AI boost:** Use AI to estimate story points, generate sprint reports, and predict velocity. | **Facilitation** – take turns as Scrum Master in a mock stand‑up meeting. |
|  12  | TBD  | **Risk Management & Project Estimation**             | Identifying technical, schedule, and resource risks. Estimation techniques. **AI boost:** AI‑assisted risk matrix generation and Monte Carlo simulation for delivery dates. | **Risk communication** – present a risk mitigation plan to “executives” in a clear, concise manner. |
|  13  | TBD  | **Configuration Management & Version Control**       | Deep Git workflows (feature branching, rebasing, cherry‑picking). Config files (YAML, JSON, properties). **AI boost:** AI‑powered commit message generation and merge conflict resolution suggestions. | **Conflict resolution** – practice resolving merge conflicts in a paired session while maintaining code ownership. |
|  14  | TBD  | **Dependency Management & Security**                 | PyPI/Nexus/JFrog, mirror, dependency vulnerability scanning (OWASP). SonarQube for code quality and security. **AI boost:** AI empowered coding + Larger scale LLM-based vulnerability check and coding style check. | **Security mindset** – perform a threat modeling exercise in small groups like log4j. |
|  15  | TBD  | **Software Evolution, Maintenance & Technical Debt** | Refactoring strategies, technical debt measurement, legacy system modernization. **AI boost:** AI‑recommended refactoring patterns and debt quantification (e.g., SonarQube + AI). | **Long‑term stewardship** – propose a maintenance roadmap and argue for refactoring sprints. |
|  16  | TBD  | **Vibe Coding, AI Agents & Future Trends**           | Harness engineering for LLM agents, loop engineering, prompt chaining, and agent orchestration. **AI boost:** Build a simple python streamlit agent with RAG to solve a real‑world task. | **Adaptability** – reflect on how AI changes the engineer’s role and present a personal learning plan. |

---

## Course Flow & Difficulty Balance

- **Weeks 1–3:** Foundation – environment, requirements, and modeling – *ease into concepts with heavy hands‑on guidance.*
- **Weeks 4–7:** Core design & implementation – architecture, OOD, and full‑stack development – *moderate challenge, integrating front‑end and back‑end.*
- **Weeks 8–10:** Quality & operations – testing, CI/CD, reuse – *increased complexity with automation and real‑world tools.*
- **Weeks 11–14:** Management & governance – agile, risk, version control, security – *advanced topics, mixing technical and managerial skills.*
- **Weeks 15–16:** Evolution & frontier – maintenance and AI‑native development – *synthesis and future‑oriented thinking, culminating in a capstone‑like project.*

---

## AI Integration Summary

Each week embeds **AI‑augmented tasks** that are not optional but complementary – they accelerate learning, automate routine work, and teach students to critically evaluate AI outputs. Tools include Claude, ChatGPT, automated test generators, security scanners, and custom prompts for planning and estimation.

---

## Soft Skills Thread

Beyond the technical curriculum, every session includes a dedicated **soft skills activity** – from role‑playing stakeholder interviews, leading stand‑ups, delivering architecture presentations, to handling incident post‑mortems. These are designed to build collaboration, communication, leadership, and ethical judgement – essential for modern engineering teams.

---

# Weekly Deliverables & Assignments

> **Instruction for Students:** Each deliverable is due by Sunday 11:59 PM. Submit all deliverables via your GitHub Classroom repository Youtube or the canvas. Clearly label each submission with the corresponding week number.

| Week | Topic                                                | Weekly Deliverable                                           | Submission Format                                            |
| :--: | ---------------------------------------------------- | ------------------------------------------------------------ | ------------------------------------------------------------ |
|  1   | **Foundations & Environment Setup**                  | **Environment Validation & AI-Assisted Hello World.** Set up Python 3, PyCharm, Git, and PostgreSQL & Dbeaver. GitHub SSH. | **GitHub repo for your self introduction** and pictures of the installed software |
|  2   | **Requirements Engineering & User Stories**          | **User Story Map & API Contract Draft.** Write 5–8 user stories for a small e-commerce checkout flow. Use AI to refine ambiguous acceptance criteria. Generate an API YAML specification for the core endpoints. | **PDF/Markdown document** with user stories and the `api.yaml` file. Include a **1-paragraph reflection** on how AI helped clarify ambiguous requirements. |
|  3   | **Visual Modeling with UML**                         | **AI-Generated UML Sequence Diagram.** Describe the "user login with 2FA" process in natural language. Use an AI tool (e.g., ChatGPT/Claude) to convert your description into a Mermaid sequence diagram. Manually validate and correct the diagram. | **Mermaid code snippet** embedded in a Markdown file, plus a **screenshot** of the rendered diagram. Attach a **brief audit note** (2–3 bullets) listing what you corrected after the AI's first output. |
|  4   | **Software Architecture & Structural Patterns**      | **Architectural Decision Record (ADR).** You are building a real-time chat app and a fintech banking app. Write an ADR comparing Monolith vs. Microservices for this specific use case. Use AI to generate the initial pros/cons table, then refine it with your own judgment. | **Markdown ADR file** following the standard template (Context, Decision, Consequences). |
|  5   | **Object-Oriented Design & SOLID Principles**        | **SOLID Refactoring Exercise.** Take the provided "legacy" code (provided by the instructor). Use AI to suggest refactoring candidates. Refactor the code to adhere to at least 3 SOLID principles. Provide a "before-and-after" diff. | **Pull Request (PR)** created on GitHub, containing the refactored code. In the PR description, explicitly list which SOLID principles were applied and **why**. |
|  6   | **Front-end Fundamentals**                           | **Reusable UI Component Library.** Build a small set of reusable Vue/React components (e.g., Button, Input, Card, Modal). Use AI to generate the initial template and CSS styling suggestions. Ensure the components are responsive. | **Build your own design system** Include a **brief style guide** (2 pages) as a PDF. |
|  7   | **Back-end Development & API Integration**           | **Secure REST API Endpoint.** Build a `/api/users/register` endpoint using FastAPI/Flask with JWT authentication and SQLAlchemy ORM. Use AI to generate test payloads and edge cases for validation. Connect it to your front-end components from Week 6. Make sure front-end page button debouncing and idempotency. | **GitHub repo** with both front-end and back-end code. Include a **Postman** export with pre-configured requests. |
|  8   | **Software Testing Strategies**                      | **Comprehensive Test Suite & Bug Report.** Write unit tests (pytest) and at least one integration test for your Week 7 API. Use AI to uncover edge-case inputs (e.g., SQL injection, long strings). Run a mutation test (or pressure test) and document any flaky tests. | **Test report (HTML/XML)** generated by pytest-cov. Submit a **Bug Report Issue** on GitHub describing one interesting edge-case bug you found and fixed. |
|  9   | **CI/CD & DevOps**                                   | **Automated Deployment Pipeline.** Create a GitHub Actions pipeline that runs your Week 8 tests and deploys your containerized app to a staging environment (e.g., Heroku, Render, or local Docker Compose). Use AI to debug a failed pipeline run. | **Pipeline run link** showing a green build. Submit a **1-page "Incident Post-mortem"** documenting one issue you encountered during pipeline setup and how you resolved it. |
|  10  | **Software Reuse & Open Source**                     | **Library Evaluation & Licensing Report.** Find 3 libraries that solve a specific problem (e.g., orm). Use AI to compare their features, performance, and license compatibility (MIT vs. GPL). Write a recommendation memo for your "team lead". | **Memo (PDF)** with a clear recommendation matrix. Include a **spreadsheet/CSV** with license compatibility checks against your project's existing dependencies. |
|  11  | **Agile Project Management & Scrum**                 | **Sprint 0 Planning Artifacts.** Create a JIRA/Confluence (or Trello) board for a 2-week sprint. Write 10-15 backlog items. Use AI to estimate story points (e.g., by prompting for complexity scores). Hold a mock sprint planning meeting (recorded). | **Board export/screenshot** and a **meeting recording link** (or timestamped notes). Submit a **velocity prediction** based on AI's estimates. |
|  12  | **Risk Management & Project Estimation**             | **Risk Register & Monte Carlo Simulation.** Identify 5–7 major risks for your project. Use AI to build a simple Monte Carlo simulation (in Python/Excel) to predict the 50th and 85th percentile completion dates. Present your findings. | **Risk register matrix (Excel/Google Sheets)** and a **Jupyter Notebook** containing the simulation code and charts. Attach a **1-slide executive summary** (PDF). |
|  13  | **Configuration Management & Version Control**       | **Git Mastery: Conflict Resolution Log.** git, status, add, checkout, branch, reset, rebase, pull, commit, -force, log. Artificially create or be assigned a merge conflict (between two branches). Resolve it using the command line. Use AI to suggest a clean commit message. and reset back. Document your resolution steps. | **Shell history log** or video snippet showing the conflict resolution. Submit a **"Conflict Resolution Guide"** written for junior developers, including the final clean commit hash. |
|  14  | **Dependency Management & Security**                 | **Security & Quality Audit.** Run OWASP Dependency Check and SonarQube (or equivalents) on your Week 9 codebase. Use AI to prioritize the top 3 vulnerabilities (CVEs) and propose concrete fixes. Implement at least one fix. | **SonarQube/Scan report (PDF)** highlighting the issues. Submit a **Pull Request** with the fix for one vulnerability, plus a short **justification** for why the other two can be postponed (deferred risk). |
|  15  | **Software Evolution, Maintenance & Technical Debt** | **Technical Debt Refactoring Roadmap.** Analyze the codebase from Week 7-9. Measure its current technical debt (using SonarQube or manual calculation). Use AI to recommend 5 refactoring targets. Write a 6-month maintenance roadmap. | **Roadmap document (Markdown/PDF)** with a prioritized list of refactoring tasks (Effort vs. Impact). Include a **"Debt Interest" calculation** (how much time is lost per sprint due to current debt). |
|  16  | **Vibe Coding, AI Agents & Future Trends**           | **Functional LLM Agent Prototype.** Build a simple agent using LangChain RAG to solve a multi-step user real world problem. Reflect on the "harness engineering" challenges encountered. Make a video and upload on Youtube. | **GitHub repo** with the agent code and a `demo.md` containing conversation logs. Submit a **2-page reflective essay** on how AI agents might reshape the software engineer's daily workflow in the next 1 year. |
