---
layout: project
title: LLM-Powered Legal Research Chatbot
subtitle: RAG-based legal search built with Mistral and Streamlit
---

Having seen my meticulous lawyer friends dig through dense, jargon-heavy legal documents, I built a RAG-based chatbot to make legal research faster and easier. The tool lets users upload multiple legal PDFs, ask questions, and receive grounded responses with direct citations from the source texts. If the question is out of scope or unclear, the chatbot is less prone to hallucinations because of the prompting technique - it may simply say, *'I don’t know the answer.'* This behavior contrasts with generic language models, where memory is temporary and hallucinations are more common. Hence, such RAG based systems are also scalable.

Herein, legal documents are split into chunks and embedded using Nomic Embed, capturing the contextual meaning of the content. These embeddings are stored in a Chroma vector database, where we perform similarity based retrieval during inference. When a query is made, the most relevant chunks are retrieved and passed to Mistral-7B via Ollama, which generates a source-linked answer. This app runs fully offline and is deployed through a Streamlit interface, allowing users to upload documents, ask questions, and verify model responses against original sources.

<a href="https://github.com/jaivardhanschauhan/RAG-chatbot" target="_blank" class="button">Code</a>
