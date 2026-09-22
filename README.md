## Bora Teker

Computer Science graduate, University at Buffalo. Based in Istanbul, Türkiye.

I build backend services and applied AI systems — mostly Python and Java. The work I find
most interesting is the part around the model rather than the model itself: making a system
explain its own output, refuse to answer when its inputs are not trustworthy, and keep a
record of how it got there.

### Selected projects

**[lumos-spray-copilot](https://github.com/BoraTeker1/lumos-spray-copilot)** —
Decision-support backend for pesticide spray decisions, with an agronomist in the loop.
FastAPI + SQLAlchemy with 24 Alembic migrations, a rule-based decision engine, and an
append-only provenance model: every compliance-critical value carries its source, imported
data can never auto-approve a recommendation, and the audit trail is only ever appended to.
Next.js review UI. CI runs the backend test suite and asserts the LLM layer is mocked so
tests can never reach a live API.
`Python · FastAPI · SQLAlchemy · Alembic · pytest · Next.js · GitHub Actions`

**[queuepilot-incident-api](https://github.com/BoraTeker1/queuepilot-incident-api)** —
Incident-management API where the lifecycle is enforced rather than assumed. Illegal status
transitions are rejected by an explicit state machine, repeated alerts collapse onto a
unique dedupe key instead of opening duplicate incidents, each change appends an immutable
event, and a single exception handler maps every failure to a structured error body.
Publishes to Kafka on incident creation.
`Java 21 · Spring Boot · JPA · Kafka · PostgreSQL`

**[network-ai](https://github.com/BoraTeker1/network-ai)** —
Ingests new-grad job postings by parsing HTML tables out of a public README, deduplicates
them with a content hash enforced at the database level, and ranks them against a parsed
resume using a deterministic 0–100 scorer. No LLM calls in the scoring path — the API
returns the reasoning behind each score, not just the number.
`Python · FastAPI · SQLAlchemy · Pydantic`

**[job-description-analyzer](https://github.com/BoraTeker1/job-description-analyzer)** —
Compares a job description against a resume and streams back a structured report: fit,
gaps, keywords, and suggested bullet rewrites. The system prompt constrains the model to
the candidate's actual experience rather than letting it invent any.
`Python · OpenAI API · Gradio`

### Technical

| | |
|---|---|
| **Languages** | Python, Java, C, C++, JavaScript/TypeScript, SQL |
| **Backend** | FastAPI, Spring Boot, SQLAlchemy, JPA/Hibernate, Alembic, REST API design, PostgreSQL, SQLite, Kafka |
| **AI/ML** | LLM application development, prompt design, streaming responses, rule-based and hybrid decision engines |
| **Tooling** | Git, GitHub Actions, pytest, Gradle, Maven, Next.js |

### Contact

[tekerbora@gmail.com](mailto:tekerbora@gmail.com) · [LinkedIn](https://www.linkedin.com/in/borateker/)
