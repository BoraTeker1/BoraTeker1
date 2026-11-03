## Bora

CS graduate from the University at Buffalo, currently based in Istanbul.

I mainly work with Python and Java, building backend applications and experimenting with AI agents. Recently, I've been learning how to build agents from scratch, focusing on tool calling, planning, routing, and testing their outputs.

### Projects

**[lumos-spray-copilot](https://github.com/BoraTeker1/lumos-spray-copilot)**

Built a tool to help farmers decide when to spray pesticides. It checks things like harvest timing, safety restrictions, and pesticide usage rules before sending recommendations to an agronomist for review. Includes a Next.js dashboard, decision history, and automated tests.

`Python, FastAPI, SQLAlchemy, Next.js, pytest`

**[queuepilot-incident-api](https://github.com/BoraTeker1/queuepilot-incident-api)**

An incident management API built with Spring Boot. Handles incident status changes, prevents duplicate alerts, tracks changes in PostgreSQL, and publishes events through Kafka.

`Java, Spring Boot, PostgreSQL, Kafka`

**[network-ai](https://github.com/BoraTeker1/network-ai)**

A job search tool I built to make finding relevant new-grad roles easier. It collects job postings, compares them against a resume, and ranks matches using a rule-based scoring system. Each match includes an explanation of its score.

`Python, FastAPI, SQLAlchemy, Pydantic`

**[job-description-analyzer](https://github.com/BoraTeker1/job-description-analyzer)**

Compares a resume against a job description and suggests improvements, including missing skills, relevant keywords, and stronger resume bullets.

`Python, OpenAI API, Gradio`

### AI Agent Projects

I've recently been building small agents from scratch to better understand how they work beyond calling an LLM API.

**01 — ReAct Agent**

Built an agent that can decide when to use tools, execute them, and use their results to answer a question. Supports web search, calculations, and date lookups, with a step limit to prevent endless loops.

**02 — Planning Agent**

An agent that breaks a request into smaller steps before executing it. Uses Pydantic to structure plans, tracks completed steps, and can revise the plan based on intermediate results.

**03 — Code-Fixing Agent**

An agent that writes Python code, runs it through pytest, reads the failures, and tries to fix its mistakes. Uses a generator-critic loop with a maximum of three attempts.

**04 — Intelligent Router**

Built a router that classifies requests as coding, research, support, or unclear, then passes them to the appropriate handler. Tested routing decisions against 30 sample requests while measuring accuracy and latency.

`Python, OpenAI API, Pydantic, pytest`

### Tech Stack

- **Languages:** Python, Java, C, C++, TypeScript, JavaScript, SQL
- **Backend:** FastAPI, Spring Boot, SQLAlchemy, PostgreSQL, SQLite, Kafka
- **AI:** OpenAI API, LLM agents, tool calling, planning, RAG, evaluation
- **Tools:** Git, Docker, GitHub Actions, pytest, Next.js

### Contact

- **Email:** [tekerbora@gmail.com](mailto:tekerbora@gmail.com)
- **LinkedIn:** [linkedin.com/in/borateker](https://www.linkedin.com/in/borateker/)
