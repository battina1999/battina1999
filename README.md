# Dhanush Gopal Battina

I work with SQL and Python on reporting pipelines and ML training data. At Virtusa, I’ve used Talend and Oracle for airline reporting. On a separate project, I prepared video and log data for model training, including near-duplicate detection and checks for underrepresented driving conditions.

I’m based in Denton, Texas, and looking for SQL, data engineering, analytics and applied AI roles in DFW or remote in the U.S.

[LinkedIn](https://www.linkedin.com/in/dhanush-gopal-battina/) · [Email](mailto:dhanushbattina09@gmail.com)

## Projects you can try

These are independent portfolio projects, separate from my employer work. Each repository includes setup instructions, tests, and the assumptions behind its results.

| Project | What to look at | Try it / source |
| --- | --- | --- |
| **Settlement reconciliation** | SQL joins and control totals, late corrections, repeatable loads, and an exception queue with source evidence. All payment records are synthetic. | [Demo](https://battina1999.github.io/settlement-reconciliation/) · [Code](https://github.com/battina1999/settlement-reconciliation) |
| **Support Routing Lab** | A trained text classifier, a held-out benchmark, and a review policy for uncertain tickets. Runs in your browser with no API key. | [Demo](https://battina1999.github.io/support-routing-lab/) · [Code](https://github.com/battina1999/support-routing-lab) |
| **Airline data platform** | A dbt warehouse over 3.45 million public flight records, route analytics, and a departure-delay model evaluated on a later month. | [Dashboard](https://battina1999.github.io/airline-data-platform/) · [Code](https://github.com/battina1999/airline-data-platform) |
| **Data documentation search** | BM25 and FAISS retrieval, citations, a data catalog, and an evaluation that includes unsupported questions. | [Browser preview](https://huggingface.co/spaces/battina1999/data-docs-assistant) · [Code](https://github.com/battina1999/rag-data-docs-assistant) |
| **Streaming anomaly checks** | A synthetic event replay with five quality rules and SQL monitoring. Includes a separate Kafka/Spark console example. | [Code](https://github.com/battina1999/streaming-anomaly-pipeline) |

## A few results worth inspecting

**Settlement reconciliation:** the synthetic scenario starts with **182 open checks**. Late records and corrections reduce that to **eight duplicate bookings** that still need review. Replaying the six source files imports **zero rows** and leaves the report unchanged. [Read the reconciliation SQL](https://github.com/battina1999/settlement-reconciliation/blob/main/sql/04_issues.sql).

**Support routing:** on the official BANKING77 test set, the classifier got **88.12% of 3,080 tickets** right. With the review policy enabled, it routed **2,008 tickets** and got **1,970** of those right (**98.11%**). It sent the other **1,072** to review. The threshold was selected on a separate calibration split; the report includes wrong routes and unsupported-topic probes. [Read the evaluation](https://github.com/battina1999/support-routing-lab/blob/main/docs/evaluation.json).

**Airline analytics:** across six selected months, San Diego–San Francisco had the lowest on-time rate among routes with at least 2,000 scheduled flights: **54.48%**, with 2,987 scheduled flights and 32 cancellations. The SQL makes the denominator explicit. [Inspect the query](https://github.com/battina1999/airline-data-platform/blob/main/dbt/airline_dwh/models/marts/analytics/route_performance.sql).

**Document search:** hybrid retrieval found the expected source in the first four results for **66 of 71** answerable questions, versus **61** using vectors alone. Both declined **26 of 32** questions outside the documentation. These measure retrieval and refusal behavior; the development set was used for tuning. [Inspect the questions](https://github.com/battina1999/rag-data-docs-assistant/blob/main/eval/eval_questions.yaml).
