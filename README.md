# Vision-RAG: Developing Visual Augmented Q&A using Vision & Multimodal LLM
Welcome to the repository. This work is created for participants of a workshop.

***Problem Statement***: Traditional information extraction systems face challenges with text only language models as it does not consider infographics (visual elements of information) such as tables, charts, images etc. often used to convey complex information to readers. Conventional RAG solutions uses multiple complex models such as OCR, Layout detection and table extraction models to convert visual elements in text.

The emergence of multi-modal LLMs (MLLMs) resolves the issue of visual document understanding by mapping text queries to provided multi-modal context. But multimodal LLMs (MLLM) face challenges of finding needle in the haystack problem i.e.,
* longer context length
* substantial number of documents as search space.

**Visual Language Models** (like ColPali, ColQwen) can encode text and images together in an embeddings are state-of-the-art retrievers for complex documents understanding.


***How do we retrieve a page with such information in infographics ?***

<u>Text Query</u>
What is Ipad's revenue contribution in Apple's total revenue for Q1 2024 ?

![alt text](https://g.foolcdn.com/image/?url=https%3A%2F%2Fg.foolcdn.com%2Feditorial%2Fimages%2F765160%2Fapple-revenue-q124-final.png&w=700)


## Outline
In this workshop, we develop a visual augmented Question-Answering system as step by step process:
1. Usecase & Quick overview of the workshop
2. Introduction to Visual Language Embedidng Models (brief talk)
3. ***Module 1***: Develop visual-augmented search using ColPali.
4. Introduction to Multi-modal LLMs (brief talk) 
5. ***Module 2***: Prompting Multi-modal LLM for Visual Q&A using Qwen-2.5-VL-3B
6. ***Module 3***: Develop end to end visual augmented Q&A using Vision-RAG.
7. ***Module 4***: Setting up vector database as retriever for vision-RAG (coming soon)
8. Practical challenges with Vision based RAG (talk)
9. ***Module 5***: Using Vector DB as Retriever and ColPali as re-ranker (coming soon)
10. Key Takeaways & Conclusion 

## Workshop Notebooks
There are multiple notebooks available there. Here are short descriptions which may help to quickly follow.

🔽 `1_search_with_colpali_late_interaction`: This notebook demostrates to perform query search over a PDF which also includes searching over all the infographics provided in PDF.

🔽 `2_prompting_qa_using_multi_modal_llm`: This notebook demonstrates processing and integrating visual language information for Qwen Model to generate answers for given query.

🔽 `3_develop_vision_rag_end_to_end`: This notebook combines the first two notebooks to develop end-to-end process of Vision-RAG.

🔽 `4_setup_vectordb_as_retriever` (coming soon): This notebook demostrates setting up a vector database for the multi-vector embeddings (visual augment retrieval).

🔽 `5_vectordb_colpali_as_reranker` (coming soon): This notebook employs best of both worlds.
    * Faster retrieval using vector DB (1st pass)
    * In-memory ColPali like model for re-ranking (since its state-of-art performance).

## Hardware Requirements
1. All you need is a device with internet connection.
2. All notebooks can be run from Google collab.

## Workshop Pre-Reads
We will be using the following tools during the workshop. Participants might find it useful to make themselves familiar with these prior to the workshop.

1. [ColPali](https://github.com/illuin-tech/colpali): Open source visual embedding model. This has demostrated state-of-the-art performance on complex document retrieval.
2. [Qwen 2.5VL 3B](https://huggingface.co/Qwen/Qwen2.5-VL-3B-Instruct): A multi-modal language model: Prompt such LLM for image based document understanding task.
3. [FAISS Vector DB](https://github.com/facebookresearch/faiss): Vector DB used for demostration here. Similary Chroma DB or any other open source DB can be implemented.
4. [ColPali Paper](https://arxiv.org/abs/2407.01449): Original paper on which the solution is based. 


<details>
<summary>🔽 Additional Pre-Readings</summary>
   
- [ViDoRe](https://github.com/illuin-tech/vidore-benchmark): A benchmark of 10 tasks to evaluate the performance of document retrieval systems on visually rich documents across various tasks, domains, languages, and settings.
   
- Few other Vector DB implementations of ColPali integrations can be checked here: 
   [Elastic Search](https://www.elastic.co/search-labs/blog/elastiacsearch-colpali-document-search)
   [Qdrant](https://qdrant.tech/documentation/advanced-tutorials/reranking-hybrid-search/)
</details>
