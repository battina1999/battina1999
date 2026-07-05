<h1 align="center">Hi, I'm Dhanush 👋</h1>

<p align="center">
  <b>Data Engineer</b> — I build data systems across <b>batch, streaming, and AI</b>.
</p>

<p align="center">
  <a href="https://www.linkedin.com/in/dhanush-gopal-battina"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?logo=linkedin&logoColor=white"></a>
  <a href="mailto:dhanushbattina09@gmail.com"><img src="https://img.shields.io/badge/Email-EA4335?logo=gmail&logoColor=white"></a>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Python-3776AB?logo=python&logoColor=white">
  <img src="https://img.shields.io/badge/SQL-4479A1?logo=postgresql&logoColor=white">
  <img src="https://img.shields.io/badge/dbt-FF694B?logo=dbt&logoColor=white">
  <img src="https://img.shields.io/badge/Apache%20Airflow-017CEE?logo=apacheairflow&logoColor=white">
  <img src="https://img.shields.io/badge/Apache%20Kafka-231F20?logo=apachekafka&logoColor=white">
  <img src="https://img.shields.io/badge/Spark-E25A1C?logo=apachespark&logoColor=white">
  <img src="https://img.shields.io/badge/Snowflake-29B5E8?logo=snowflake&logoColor=white">
  <img src="https://img.shields.io/badge/Docker-2496ED?logo=docker&logoColor=white">
</p>

---

I design and ship end-to-end data platforms — ingestion, data quality, dimensional
modelling, orchestration, real-time streaming, and analytics — with a focus on
work that **actually runs** and is **cloud-portable**. Below are three projects on
one coherent airline-operations domain, each runnable on a laptop with a single
command and ready to scale to the cloud.

## 🚀 Featured Projects

### ✈️ [Airline Data Pipeline & Analytics Platform](https://github.com/battina1999/airline-data-platform)
End-to-end **batch ELT**: Talend-style ingestion → **Great Expectations** data
quality → **dbt** star schema (staging → dims/facts → marts) → source-to-target
reconciliation → **Apache Airflow** orchestration → **Power BI**/Streamlit.
Local-first on **DuckDB**, cloud-ready for **Snowflake**. 30 dbt tests + 25 GE checks.
> `Python` · `SQL` · `dbt` · `Airflow` · `Great Expectations` · `DuckDB/Snowflake` · `Power BI` · `Docker`

### 🔎 [RAG-Based Data Documentation Assistant](https://github.com/battina1999/rag-data-docs-assistant)
A **grounded RAG** assistant that answers questions about data documentation with
**source citations** and **refuses to guess** when the answer isn't documented.
**LangChain + FAISS** retrieval, a relevance-gated anti-hallucination fallback, a
SQL data catalog, a **FastAPI** service, and an evaluation harness (100% refusal
accuracy). OpenAI-powered; runs offline without a key.
> `Python` · `LangChain` · `FAISS` · `OpenAI API` · `FastAPI` · `SQLite` · `Docker`

### 📡 [Real-Time Streaming Pipeline with Anomaly Detection](https://github.com/battina1999/streaming-anomaly-pipeline)
A **real-time** pipeline that detects **five classes of data anomaly in-stream**
(volume spikes, missing values, duplicates, late-arriving data, freshness gaps),
loads SQL monitoring aggregations, and raises severity-graded alerts. **Kafka +
Spark Structured Streaming** in production behind a bus abstraction that also runs
in-memory for local dev and tests.
> `Python` · `Apache Kafka` · `Spark Structured Streaming` · `SQL` · `DuckDB/Snowflake` · `Power BI` · `Docker`

## 🛠️ Tech Stack

**Languages & data:** Python, SQL, Pandas
**Pipelines & modelling:** dbt, Apache Airflow, Great Expectations
**Streaming:** Apache Kafka, Spark Structured Streaming
**Warehouses:** DuckDB, Snowflake
**AI / LLM:** LangChain, FAISS, OpenAI API, RAG
**Serving & BI:** FastAPI, Power BI, Streamlit
**Tooling:** Docker, Git, pytest, Make

## 📫 Contact

- 📧 **dhanushbattina09@gmail.com**
- 📧 **battina1999@gmail.com**
- 💼 [linkedin.com/in/dhanush-gopal-battina](https://www.linkedin.com/in/dhanush-gopal-battina)

<p align="center"><i>Every project above runs with one command, is tested, cloud-portable, and ships with a written architecture + report.</i></p>
