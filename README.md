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
