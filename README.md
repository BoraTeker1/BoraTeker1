## Bora Teker

Computer Science graduate, University at Buffalo. Based in Istanbul.

I write backend services, mostly in Python and Java. Most of what I've built lately has an
LLM somewhere in it, and the hard parts have usually been everywhere else: showing how a
result was reached, deciding what the system should do when its input data isn't
trustworthy, and keeping records that still make sense to someone reading them months later.

### Selected projects

**[lumos-spray-copilot](https://github.com/BoraTeker1/lumos-spray-copilot)**
Decision support for pesticide spray timing, with an agronomist reviewing every
recommendation before it reaches a grower. FastAPI and SQLAlchemy backend with 25 Alembic
migrations, a rule-based decision engine, and a provenance layer that records where each
compliance-critical value came from. Imported values always escalate to human review, since
nothing unverified is allowed to produce an automatic approval. The audit trail is
append-only. Next.js review UI. CI runs the backend test suite and asserts the LLM layer is
mocked, so tests can never reach a live API.
`Python, FastAPI, SQLAlchemy, Alembic, pytest, Next.js, GitHub Actions`

**[queuepilot-incident-api](https://github.com/BoraTeker1/queuepilot-incident-api)**
An incident tracker with a real lifecycle behind it. Status changes go through an explicit
state machine, so an illegal transition returns a 400 instead of quietly corrupting the
record. Repeated alerts carrying the same dedupe key collapse into one incident, backed by a
unique constraint in the database. Every change appends a row to an audit table, and a
single exception handler maps each failure type to a structured error body. Opening an
incident publishes to Kafka.
`Java 21, Spring Boot, JPA, Kafka, PostgreSQL`

**[network-ai](https://github.com/BoraTeker1/network-ai)**
Pulls new-grad job postings by parsing HTML tables out of a public README, which is messier
than it sounds: continuation rows inherit the company above them, and half the markup is
decorative. Postings are deduplicated by a content hash enforced at the database level.
Scoring against a parsed resume is a deterministic 0 to 100 rule set with no model call in
the path, and the API hands back the reasoning behind each score along with it.
`Python, FastAPI, SQLAlchemy, Pydantic`

**[job-description-analyzer](https://github.com/BoraTeker1/job-description-analyzer)**
Takes a job description and a resume and streams back a structured report: how well they
fit, what's missing, which keywords to add, and how to rewrite specific bullets. The system
prompt holds the model to experience that actually appears in the resume.
`Python, OpenAI API, Gradio`

### Technical

| | |
|---|---|
| **Languages** | Python, Java, C, C++, JavaScript/TypeScript, SQL |
| **Backend** | FastAPI, Spring Boot, SQLAlchemy, JPA/Hibernate, Alembic, REST API design, PostgreSQL, SQLite, Kafka |
| **AI/ML** | LLM application development, prompt design, streaming responses, rule-based and hybrid decision engines |
| **Tooling** | Git, GitHub Actions, pytest, Gradle, Maven, Next.js |

### Contact

Email: [tekerbora@gmail.com](mailto:tekerbora@gmail.com)
LinkedIn: [linkedin.com/in/borateker](https://www.linkedin.com/in/borateker/)
