# Workshop: Vision-RAG
Welcome to the repository. This work is created for participants of a workshop. 

This repository is tutorial to develop a visual augmented Question-Answering system: 
1. Vector DB based retriever
2. ColPali based re-ranker for document retrieval
3. Multi-modal LLM for generating answer using enriched prompt (with retrieved information).

There are multiple notebooks available there. Here are short descriptions which may help to quickly follow.

1. `1_search_with_colpali_late_interaction`: This notebook demostrate how to perform query search over a PDF which also includes searching over all the infographics provided in PDF.

2. `2_prompting_qa_using_multi_modal_llm`: This notebook demonstrate processing and integrating visual language information for Qwen Model to generate answers for given query.

3. `3_develop_vision_rag_end_to_end`: This notebook combines the first two notebooks to develop end-to-end process of Vision-RAG.
