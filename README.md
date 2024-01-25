# myRAG

Exploring RAG.

## Roadmap

### Short-term goal

This is a personal project that will not be backed by fundings like a research project, so I need to minimize the cost.

The first step is getting rid of commercial vector store. I have successfully gone through the pgvector pipeline, now I can store and query vectors in postgres locally.

Next step is figuring out how to replace OpenAI embedding with open-source embedding models, if possible. Two options:

1. Run the model on local CPU. It can be slow, but easier to manage data.
2. Run the model on Colab GPU. It should be faster, but I'm using Colab in many places so I want to save its usage, and I still want to keep all my vector data locally, meaning the comm between cloud and local is an issue.

At this moment, I prefer using CPU and exploring optmizations for embedding to make it faster.

### Long-term goal

[Advanced RAG Techniques: an Illustrated Overview](https://pub.towardsai.net/advanced-rag-techniques-an-illustrated-overview-04d193d8fec6) is a great article that explained _many_ techniques in a RAG pipeline. Long term goal is trying various techniques introduced in the article and using benchmarks to see how they perform.

## Reading List

- [Retrieval-Augmented Generation for Large Language Models: A Survey](https://arxiv.org/abs/2312.10997)
- [Pinecone blog explains VDB](https://www.pinecone.io/learn/vector-database/)
- [LangChain's list of vector databases](https://python.langchain.com/docs/integrations/vectorstores)
- [LlamaIndex's tutorial on building a retriever](https://docs.llamaindex.ai/en/stable/examples/low_level/retrieval.html) (llama_idx_sample.ipynb copied this)
- [CMU-DB seminar in 23 Fall](https://db.cs.cmu.edu/seminar2023/) has a lot of VDBs
- [Advanced RAG Techniques: an Illustrated Overview](https://pub.towardsai.net/advanced-rag-techniques-an-illustrated-overview-04d193d8fec6)
- [Comparison between fine-tuning and RAG](https://www.superannotate.com/blog/llm-fine-tuning)
