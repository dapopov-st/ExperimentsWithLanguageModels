# Experiments With Language Models

This repository is used to keep track of experiments with Language Models (LMs).

## Completed Experiments

- Fine-tuning the LLama2-13b model on SQL, primarily to test if it can produce correct output with a larger model on a Colab GPU.

## In Progress

- RAG with LLama2 over some ArXiv papers in PDF format. Retrieving from a couple dozen ArXiv LLM papers. Currently, we have a working version with RecursiveCharacterTextSplitter (1000 chunks with 30 overlap), FAISS, and Llama2-13b. The answer quality seems to be good. We aim to increase the generation speed and see if we can add metadata to retrieval (as we expect retrieval over a large collection of documents to become a bottleneck).

    - Plan to experiment with Mistral or Zephyr models to increase speed. Self-Rag 7B may be another solution.
    - Next, we aim to see if we can use Pinecone/Elasticsearch to use metadata for retrieval.
