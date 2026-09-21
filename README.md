<h1 align="center">Raj Wankhede</h1>

<p align="center">
  <b>AI engineer. I build LLM systems that are safe to put in front of real users.</b>
</p>

<p align="center">
  Grounded RAG &nbsp;·&nbsp; agent guardrails &nbsp;·&nbsp; human-in-the-loop &nbsp;·&nbsp; evaluation you can fail a build on
</p>

<p align="center">
  <img alt="Python" src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white">
  <img alt="FastAPI" src="https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white">
  <img alt="PostgreSQL + pgvector" src="https://img.shields.io/badge/PostgreSQL%20%2B%20pgvector-4169E1?style=flat-square&logo=postgresql&logoColor=white">
  <img alt="AWS" src="https://img.shields.io/badge/AWS%20Bedrock%20%26%20Serverless-FF9900?style=flat-square&logo=amazonwebservices&logoColor=white">
  <img alt="Azure OpenAI" src="https://img.shields.io/badge/Azure%20OpenAI-0078D4?style=flat-square&logo=microsoftazure&logoColor=white">
  <img alt="React" src="https://img.shields.io/badge/React-61DAFB?style=flat-square&logo=react&logoColor=black">
  <img alt="Docker" src="https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white">
</p>

---

## What I actually do

Most LLM demos work. Most LLM *products* break the first time someone asks a question the knowledge base cannot answer — and the model answers anyway, fluently and wrongly.

Closing that gap is the work. I design and ship retrieval and agent systems where the unglamorous parts are in place from day one:

**Grounded, or honestly silent.** Hybrid retrieval (pgvector similarity + PostgreSQL full-text, fused with Reciprocal Rank Fusion), reranking, evidence-sufficiency checks, contradiction resolution by source authority, and validation of every citation, number, date and entity before a user sees a word. No evidence, no answer — the system says so and offers a human instead of guessing.

**Governance as a deployment condition, not a retrofit.** Tool calls classified by risk, human approval gates in front of irreversible actions, unknown tools failing closed to high risk, per-call cost tracking, and an audit trail behind every decision.

**Production shape from the first commit.** Multi-tenancy enforced in SQL, role-based access control, versioned document ingestion with atomic activation, prompt-injection defences, structured logs and per-stage traces, migrations, Docker, CI.

**Measured, not vibed.** Golden-dataset evaluation with enforced thresholds for groundedness, citation correctness, abstention accuracy and hallucination rate — running in CI, allowed to fail the build.

Currently building a German-language enterprise AI platform (KI-Plattform) at **[Beyondles](https://github.com/beyondles-ai)**.

## Selected work

| Project | What it is |
| --- | --- |
| **[AI-Agent-Customer-Support-RAG](https://github.com/raj-wankhede-github/AI-Agent-Customer-Support-RAG)** | A support agent that answers only from an approved knowledge base, cites the exact evidence, and abstains or hands off to a human when the evidence is missing, weak or contradictory. FastAPI + pgvector hybrid RAG, React support console, multi-tenant, evaluated against a golden dataset in CI. |
| **[agent-guardrail](https://github.com/raj-wankhede-github/agent-guardrail)** | A framework-agnostic safety layer between an agent and its tools: risk classification, human approval for irreversible calls, Bedrock Guardrails content/PII checks, cost tracking and a full audit log — in ~250 lines of FastAPI. |
| **[decision-making-simulator](https://github.com/raj-wankhede-github/decision-making-simulator)** | Takes a decision, finds the uncertain variables, runs 10,000 simulations of how it could go, and shows where the futures cluster and how bad the tail really is. |
| **[rag-assistant](https://github.com/raj-wankhede-github/rag-assistant)** | A fully local RAG assistant over your own PDFs, powered by Claude. |
| **[RAG-Bedrock-OpenAI-AzureOpenAI](https://github.com/raj-wankhede-github/RAG-Bedrock-OpenAI-AzureOpenAI)** | The same RAG pipeline across three providers — useful when the question is "what does switching actually cost us?" |
| **[image-generation-via-openai-azureopenai-bedrock](https://github.com/raj-wankhede-github/image-generation-via-openai-azureopenai-bedrock)** | One image-generation interface, three clouds behind it. |

## Toolbox

**Languages** Python · TypeScript · SQL  
**AI** Anthropic Claude · OpenAI · Azure OpenAI · Amazon Bedrock · Ollama · RAG · agents & tool use · evaluation harnesses  
**Backend** FastAPI · Pydantic · SQLAlchemy (async) · Alembic · PostgreSQL + pgvector · Neo4j  
**Cloud & ops** AWS (Lambda, ECS, S3, Bedrock, API Gateway) · Azure · Docker · GitHub Actions · structured logging  
**Frontend** React · Vite · Tailwind  

## A principle I keep coming back to

> A model that is confidently wrong once costs more trust than a hundred correct answers earn.

So my systems are allowed to say *"I don't know"* — and are built so that they actually do.

## Say hello

<p>
  <a href="https://www.linkedin.com/in/rajwankhede"><img alt="LinkedIn" src="https://img.shields.io/badge/LinkedIn-0A66C2?style=flat-square&logo=linkedin&logoColor=white"></a>
  <a href="https://github.com/raj-wankhede-github?tab=repositories"><img alt="Repositories" src="https://img.shields.io/badge/My%20repositories-181717?style=flat-square&logo=github&logoColor=white"></a>
</p>
