# Timescale Vector
Timescale Vector is a `PostgreSQL++` vector database for AI applications. It combines pgvector with a new faster index type and a rock-solid cloud hosting platform built for production applications.

Timescale Vector empowers efficient storage, querying and management of millions of vector embeddings within PostgreSQL. Because Timescale Vector is built upon PostgreSQL, it support all of standard SQL for working with vector data and combining it with other data types.

## Timescale Vector builds on top of pgvector

Timescale vector uses the pgvector datatype and supports the `ivfflat` and `hnsw` indexes provided by pgvector.

We boost pgvector performance in several ways:
- By providing a quicker and more precise similarity searches across 100M+ vectors through an indexing algorithm inspired by DiskANN.
- By improving queries that combine time-based filters with vector similarity search by using automatic time-based partitioning and indexing.

## The Timescale cloud platform

Timescale Vector provides a cloud PostgreSQL solution that grows from proof of concept to full-scale production:

- Streamlines operations by allowing the integration of relational metadata, vector embeddings, and time-series data within a single database.
- Leverages the robust PostgreSQL foundation, incorporating enterprise-level features such as streaming backups, replication, high availability, and row-level security.
- Delivers peace of mind with top-tier security and compliance standards.

# Using Timescale Vector

Timescale Vector is accessible via [Timescale](https://www.timescale.com/ai?utm_campaign=vectorlaunch&utm_source=aicookbook&utm_medium=referral), the cloud-based PostgreSQL service. (A self-hosted version is currently unavailable.)

We offer a 90-day free trial for Timescale Vector.

Get started by [creating an account](https://console.cloud.timescale.com/signup?utm_campaign=vectorlaunch&utm_source=aicookbooks&utm_medium=referral) on Timescale, initiating a new database, and following the provided notebooks.

View our [documentation](https://docs.timescale.com/ai/latest/?utm_campaign=vectorlaunch&utm_source=aicookbooks&utm_medium=referral) for more information:
- Learn [key vector database concepts](https://docs.timescale.com/ai/latest/key-vector-database-concepts-for-understanding-pgvector/?utm_campaign=vectorlaunch&utm_source=aicookbooks&utm_medium=referral)
- Get instruction on using our [SQL interface](https://docs.timescale.com/ai/latest/sql-interface-for-pgvector-and-timescale-vector/?utm_campaign=vectorlaunch&utm_source=aicookbooks&utm_medium=referral)
- Find out more about how to use our [Python library](https://docs.timescale.com/ai/latest/python-interface-for-pgvector-and-timescale-vector/?utm_campaign=vectorlaunch&utm_source=aicookbooks&utm_medium=referral)

For more insights and performance benchmarks, refer to the Timescale Vector [explainer blog](https://www.timescale.com/blog/how-we-made-postgresql-the-best-vector-database/?utm_campaign=vectorlaunch&utm_source=aicookbook&utm_medium=referral).

## Examples

This folder contains examples of using Timescale Vector and OpenAI together.

| Name | Description | Google Colab |
| --- | --- | --- |
| [Time-based filtering with LangChain](./time_based_filtering_with_langchain.ipynb) | How to perform semantic similarity search with filters on time or metadata using LangChain | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/openai/openai-cookbook/blob/master/examples/vector_databases/timescale/time_based_filtering_with_langchain.ipynb) |
| [Time-based filtering with LlamaIndex](./time_based_filtering_with_llamaindex.ipynb) | How to perform semantic similarity search with filters on time with LlamaIndex | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/openai/openai-cookbook/blob/master/examples/vector_databases/timescale/time_based_filtering_with_llamaindex.ipynb) |