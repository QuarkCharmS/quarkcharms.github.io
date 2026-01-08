---

title: "The Embedder (GitHub)"
excerpt: "End-to-end Retrieval-Augmented Generation stack that handles ingestion, chunking, indexing, and serving results through Open WebUI. This monorepo packages every moving part: a production-grade ingestion CLI, a reusable chunker library, a FastAPI connector for Qdrant, and local/Docker/AWS deployment assets."
collection: "portfolio"
---
The Embedder is a full RAG pipeline in one repo: it ingests sources, chunks them, builds embeddings, stores vectors, and serves retrieval results to a chat UI. The goal is to make end-to-end retrieval work feel like a single, coherent system rather than a pile of scripts.

## What it includes

- **Ingestion CLI:** pulls files and repos, chunks them, embeds content, and upserts vectors into Qdrant.
- **Semantic chunker library:** Tree-sitter aware chunking that can be reused independently.
- **Retrieval API:** FastAPI service that embeds queries, searches Qdrant, and returns context.
- **Open WebUI integration:** pipeline script to connect the retriever to a chat experience.
- **Deployment assets:** Docker Compose for local demos and Terraform modules for AWS Batch.

## How it works (high level)

1. Source content is ingested and chunked.
2. Chunks are embedded and stored in Qdrant.
3. User queries hit the retrieval API.
4. Top matches are sent to the chat UI for responses.

## Why it exists

Most RAG setups are split across multiple repos and ad-hoc docs. This project packages the core building blocks in one place so you can stand up a working pipeline quickly, then scale it with the same architecture.

**Github**: [https://github.com/QuarkCharmS/the_embedder](https://github.com/QuarkCharmS/the_embedder)
