---
title: "The Chunker (GitHub)"
excerpt: "Standalone chunking engine that turns code and text files into semantic, token-aware chunks for RAG and LLM pipelines."
collection: "portfolio"
---

the_chunker is a focused chunking engine for building LLM-friendly datasets without tying you to any embedding or vector store. It uses Tree-sitter for AST-aware chunking when possible, with reliable fallbacks for everything else.

## What it does

- Creates semantic chunks from code and text files
- Merges chunks with configurable overlap to preserve context windows
- Counts tokens in a model-aware way to hit target ranges

## Why it exists

Most pipelines mix chunking with embedding and storage logic. the_chunker keeps chunking independent so you can plug it into any RAG, summarization, or code search workflow without rewriting core logic.

**Github**: [https://github.com/QuarkCharmS/the_chunker](https://github.com/QuarkCharmS/the_chunker)
