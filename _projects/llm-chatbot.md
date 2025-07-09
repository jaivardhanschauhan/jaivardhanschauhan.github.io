---
layout: project
title: LLM-Powered Legal Research Chatbot
subtitle: RAG-based legal search built with Mistral and Streamlit
---

Having seen my meticulous lawyer friends dig through dense, jargon-heavy legal documents, I built a RAG-based chatbot to make legal research faster and easier. The tool lets users upload multiple legal PDFs, ask questions, and receive grounded responses with direct citations from the source texts. Unlike generic LLMs that often hallucinate due to limited context and no persistent memory, this RAG setup is more reliable - if a question is out of scope, it simply says, “I don’t know.” This design makes the system not just trustworthy but also scalable.

Herein, legal documents are split into chunks and embedded using Nomic Embed, capturing the contextual meaning of the content. These embeddings are stored in a Chroma vector database, where we perform similarity based retrieval during inference. When a query is made, the most relevant chunks are retrieved and passed to Mistral-7B via Ollama, which generates a source-linked answer. This app runs fully offline and is deployed through a Streamlit interface, allowing users to upload documents, ask questions, and verify model responses against original sources.

<a href="https://github.com/jaivardhanschauhan/RAG-chatbot" target="_blank" class="button">Code</a>
