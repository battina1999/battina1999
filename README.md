# Dhanush Gopal Battina

I work with SQL and Python. At Virtusa, I’ve used Talend and Oracle for airline reporting. On a separate project, I prepared video and log data for model training, including finding near-duplicate frames and checking which driving conditions were underrepresented.

The projects below are my own portfolio work. The flight warehouse uses records published by the U.S. Bureau of Transportation Statistics.

### Airline operations in SQL

Which busy routes had the most trouble arriving on time? In six selected months of flight records, San Diego to San Francisco had the lowest on-time rate among routes with at least 2,000 scheduled flights. The rate was **54.48%**. The route had **2,987 scheduled flights**, including 32 cancellations. The dbt model shows exactly which flights count toward each number.

[Explore the dashboard](https://battina1999.github.io/airline-data-platform/) · [Read the route SQL](https://github.com/battina1999/airline-data-platform/blob/main/dbt/airline_dwh/models/marts/analytics/route_performance.sql) · [Follow a flight through the warehouse](https://github.com/battina1999/airline-data-platform)

### A search assistant for data documentation

I built a Python service that looks up questions in the airline project’s docs and cites the passage it used. Adding BM25 keyword search to FAISS vector search brought the expected document into the first four results for **66 of 71** answerable questions, up from **61** with vectors alone. Both versions declined **26 of 32** questions outside the docs. The evaluation includes the misses.

[Run the assistant](https://github.com/battina1999/rag-data-docs-assistant) · [Inspect the evaluation questions](https://github.com/battina1999/rag-data-docs-assistant/blob/main/eval/eval_questions.yaml)

### Predicting departure delays

I used SQL to build features from earlier flights, then tested logistic regression and LightGBM on January 2025. When I ranked flights by risk and took the top tenth, **29.66%** of the logistic regression picks left at least 15 minutes late. LightGBM reached **29.11%** on the same measure. Across all **523,435** flights in the test set, **18.23%** left late.

[Read the model card](https://github.com/battina1999/airline-data-platform/blob/main/docs/model_card.md) · [Inspect the feature SQL](https://github.com/battina1999/airline-data-platform/blob/main/dbt/airline_dwh/models/ml/fct_features_flight.sql)

### Finding bad events in an airline feed

I replay synthetic events with missing fields, duplicate IDs, late arrivals, spikes and gaps. A DuckDB scorecard shows how many times each rule fires. The repository also includes a Kafka and Spark example that writes window counts and rows with missing fields to the console.

[Run the replay](https://github.com/battina1999/streaming-anomaly-pipeline) · [Read the monitoring SQL](https://github.com/battina1999/streaming-anomaly-pipeline/blob/main/sql/aggregations.sql)

I’m based in Denton, Texas, and interested in SQL development, data engineering, analytics and applied AI roles in DFW or remote in the U.S. [LinkedIn](https://www.linkedin.com/in/dhanush-gopal-battina/) · [Email](mailto:dhanushbattina09@gmail.com)
