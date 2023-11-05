# Experiments With Language Models

This repository is used to keep track of experiments with Language Models (LMs).

## Completed Experiments

- Fine-tuning the LLama2-13b model on SQL, primarily to test if it can produce correct output with a larger model on a Colab GPU. 28GBs was the max amount of memory used for the notebook.  I used LoRA attention dimension of 32 to produce answers that would contain a correct answer.  In the future, may consider if decreasing this or using Mistral/Zephyr + increasing it will keep or increase answer quality while allowing this to run on a T4/V100.

## In Progress

- RAG with LLama2 over some ArXiv papers in PDF format. Retrieving from a couple dozen ArXiv LLM papers. Currently, there is a working version with RecursiveCharacterTextSplitter (1000 chunks with 30 overlap), FAISS, and Llama2-13b. The answer quality seems to be good. I aim to increase the generation speed and see if we can add metadata to retrieval (expect retrieval over a large collection of documents to become a bottleneck).

    - Plan to experiment with Mistral or Zephyr models to increase speed. Self-Rag 7B may be another solution.
    - Next, I aim to see if we can use Pinecone/Elasticsearch to use metadata for retrieval.

## Forthcoming

- Describe the techniques used by Karphathy in the repo that goes along with his "GPT2 from Scratch" video.  Perhaps write up a Medium article about these.
- Include some of my other work on from-scratch training.
