<h1 align="center">Hi, I'm Dhanush 👋</h1>

<p align="center">
  <b>Data engineering, SQL analytics, and applied AI</b><br>
  Python · SQL · dbt · ETL · ML data pipelines · RAG
</p>

<p align="center">
  <a href="https://www.linkedin.com/in/dhanush-gopal-battina"><img alt="LinkedIn" src="https://img.shields.io/badge/LinkedIn-0A66C2?logo=linkedin&logoColor=white"></a>
  <a href="mailto:dhanushbattina09@gmail.com"><img alt="Email" src="https://img.shields.io/badge/Email-EA4335?logo=gmail&logoColor=white"></a>
</p>

I build data pipelines, analytics models, and applied AI tools. These independent portfolio projects connect airline-data ingestion and quality checks with SQL analytics, flight-delay modeling, document retrieval, and event monitoring.

## Projects

| Project | Implementation | Explore | Main tools |
|---|---|---|---|
| ✈️ [**Airline Data Platform**](https://github.com/battina1999/airline-data-platform) | Python/SQL ingestion, dbt star schema, incremental facts, SCD Type 2 snapshot, quality checks, and reconciliation. The recorded data profile covers **3.45M US DOT flight records across six selected months**. | [Dashboard](https://battina1999.github.io/airline-data-platform/) · [Lineage](https://battina1999.github.io/airline-data-platform/lineage/) · [Data profile](https://github.com/battina1999/airline-data-platform/blob/main/docs/data_profile.md) | Python · SQL · dbt · Airflow · Great Expectations · DuckDB |
| 🤖 [**Flight Delay Prediction**](https://github.com/battina1999/airline-data-platform/blob/main/docs/model_card.md) | SQL feature pipelines, logistic regression and LightGBM with chronological evaluation, a model card, FastAPI endpoint implementation, and scoring DAG. | [Model card](https://github.com/battina1999/airline-data-platform/blob/main/docs/model_card.md) · [API source](https://github.com/battina1999/airline-data-platform/blob/main/ml/api.py) · [Demo overview](https://huggingface.co/spaces/battina1999/flight-delay-api) | scikit-learn · LightGBM · FastAPI |
| 🔎 [**RAG Documentation Assistant**](https://github.com/battina1999/rag-data-docs-assistant) | Hybrid BM25/vector retrieval, source citations, relevance-based refusal checks, and a SQLite catalog. Evaluation set contains **103 questions: 73 answerable and 30 out of scope**. | [Browser demo](https://huggingface.co/spaces/battina1999/data-docs-assistant) · [Backend](https://github.com/battina1999/rag-data-docs-assistant/blob/main/app/rag.py) · [Evaluation](https://github.com/battina1999/rag-data-docs-assistant/blob/main/eval/evaluate.py) | LangChain · FAISS · OpenAI API · FastAPI · SQLite |
| 📡 [**Streaming Anomaly Pipeline**](https://github.com/battina1999/streaming-anomaly-pipeline) | Local Python pipeline with five anomaly checks, SQL health aggregates, and threshold alerts. Separate Kafka/Spark path implements missing-field filtering, watermarking, deduplication, and windowed counts. | [Local implementation](https://github.com/battina1999/streaming-anomaly-pipeline/blob/main/streaming/anomaly.py) · [Spark implementation](https://github.com/battina1999/streaming-anomaly-pipeline/blob/main/spark/streaming_job.py) | Python · SQL · DuckDB · Kafka · Spark |

### How the projects connect

The airline platform produces analytics marts, SQL features for flight-delay modeling, and documentation used by the RAG assistant. The streaming project demonstrates event-quality monitoring in the same domain.

### Demo and evaluation scope

- The flight-delay demo link opens an overview/fallback page. The prediction endpoint implementation is available in the repository; the demo page is not a live inference API.
- The RAG browser demo uses curated passages. The full LangChain/FAISS backend is a separate implementation.
- RAG evaluation distinguishes retrieval, response coverage, refusals, and citation presence. Response coverage and citation presence do not by themselves establish factual answer accuracy.
- Five anomaly classes are implemented in the local streaming pipeline. The Spark path currently writes to console and has a narrower feature set.
- Recorded benchmark and CI results describe their documented runs. Check each repository for the latest status, setup, and limitations.

## Tools used in these projects

**Data:** Python, SQL, dbt, Airflow, Great Expectations, DuckDB, Kafka, Spark  
**ML and AI:** scikit-learn, LightGBM, LangChain, FAISS, OpenAI API  
**Applications and testing:** FastAPI, Streamlit, Docker, GitHub Actions, pytest

Snowflake configuration and Power BI DAX/model documentation are included in the airline repository. They are distinct from a verified cloud deployment or a published Power BI report.

## Contact

- **dhanushbattina09@gmail.com**
- [linkedin.com/in/dhanush-gopal-battina](https://www.linkedin.com/in/dhanush-gopal-battina)
