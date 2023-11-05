# ExperimentsWithLanguageModels
Just a repo to keep track of experiments with LMs
* Finetune LLama2-13b model on SQL, mostly to see if can produce correct output with a larger model on a Colab GPU
  
In progress:
* RAG with LLama2 over some ArXiv paper in PDF format.  Retrieving from a couple dozen ArXiv LLM papers.  Currently have RecursiveCharacterTextSplitter (1000 chunks with 30 overlap) + FAISS + Llama2-13b version working. The answer quality seems to be good.  Would like to increase generation speed and see if can add metadata to retrieval (expect retrieval over a large collection of documents to become a bottleneck).

&emsp; * Plan to experiment with Mistral or Zephyr models to increase speed.  It could be that Self-Rag 7B may be anothe solution. 
&emsp; * Next to see if can use Pinecone/Elasticsearch to use metadata to retrieval
