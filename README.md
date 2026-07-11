<h1 align="center">Hi, I'm Dhanush 👋</h1>

<p align="center">
  <b>Data Engineer</b> — batch, streaming, and AI on one production-shaped platform.
</p>

<p align="center">
  <a href="https://www.linkedin.com/in/dhanush-gopal-battina"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?logo=linkedin&logoColor=white"></a>
  <a href="mailto:dhanushbattina09@gmail.com"><img src="https://img.shields.io/badge/Email-EA4335?logo=gmail&logoColor=white"></a>
</p>

## 🚀 Projects — with live demos

| Project | What it proves | Live | Stack |
|---|---|---|---|
| ✈️ [**Airline Data Platform**](https://github.com/battina1999/airline-data-platform) | **3.45M real US DOT flights** through ingestion → Great Expectations → tested dbt star schema → reconciliation, with green CI | [Dashboard](https://airline-ops-battina.streamlit.app) · [Lineage](https://battina1999.github.io/airline-data-platform/) | Python · SQL · dbt · Airflow · GE · DuckDB/Snowflake · Power BI |
| 🤖 [**Delay Prediction ML**](https://github.com/battina1999/airline-data-platform/blob/main/docs/model_card.md) (same repo) | Features-as-SQL in dbt, honest date-split evaluation (baseline → LightGBM), model card, FastAPI serving, scoring DAG | [Try /predict](https://huggingface.co/spaces/battina1999/flight-delay-api) | LightGBM · scikit-learn · FastAPI · Docker |
| 🔎 [**RAG Documentation Assistant**](https://github.com/battina1999/rag-data-docs-assistant) | Grounded, cited answers over the platform's real docs; hybrid BM25+vector (hit-rate 95%); two-signal anti-hallucination gate; 102-question eval | [Ask it](https://huggingface.co/spaces/battina1999/data-docs-assistant) | LangChain · FAISS · OpenAI · FastAPI |
| 📡 [**Streaming Anomaly Pipeline**](https://github.com/battina1999/streaming-anomaly-pipeline) | Kafka + Spark Structured Streaming detecting 5 anomaly classes in-stream, validated injected-vs-detected, SQL health monitoring + alerting | `make demo` (60s local) | Kafka · Spark · SQL · DuckDB/Snowflake |

**One platform, one domain:** the batch pipeline produces the marts the
dashboard serves, the docs the RAG assistant answers from, and the features the
ML model trains on — while the streaming pipeline guards the same domain in
real time.

```
BTS 3.45M flights ─► ingestion ─► raw ─► dbt (staging ─► star schema ─► marts) ─► BI (Streamlit / Power BI)
                        │              │                     ├─► ML features ─► LightGBM ─► /predict API + scoring DAG
        Great Expectations ✓    reconciliation ✓             └─► docs ─► RAG assistant (cited answers)
                     Kafka + Spark streaming: real-time anomaly detection on the same domain
```

## 🛠️ Tech

**Data:** Python, SQL, dbt, Apache Airflow, Great Expectations, Kafka, Spark,
DuckDB, Snowflake · **ML/AI:** scikit-learn, LightGBM, LangChain, FAISS,
OpenAI API · **Serving/BI:** FastAPI, Streamlit, Power BI · **Ops:** Docker,
GitHub Actions CI, pytest, Make

## 📫 Contact

- 📧 **dhanushbattina09@gmail.com** · battina1999@gmail.com
- 💼 [linkedin.com/in/dhanush-gopal-battina](https://www.linkedin.com/in/dhanush-gopal-battina)

<p align="center"><i>Every repo: green CI, one-command run, written architecture + decision records.</i></p>
