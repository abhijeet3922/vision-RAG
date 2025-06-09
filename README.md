# Vision-RAG: Developing Visual Augmented Q&A using Vision & Multimodal LLM
Welcome to the repository. This work is created for participants of a workshop.

*Problem Statement*: Traditional information extraction systems face challenges with text only language models as it does not consider infographics (visual elements of information) such as tables, charts, images etc. often used to convey complex information to readers. 
Multimodal LLM (MLLM) face challenges of finding needle in the haystack problem i.e., either longer context length or substantial number of documents as search space.

## Outline
In this workshop, we develop a visual augmented Question-Answering system as step by step process:
1. Usecase & Quick overview of the workshop
2. Introduction to Visual Language Embedidng Models (brief talk)
3. **Module 1**: Develop visual-augmented search using ColPali.
4. Introduction to Multi-modal LLMs (brief talk) 
5. **Module 2**: Prompting Multi-modal LLM for Visual Q&A using Qwen-2.5-VL-3B
6. **Module 3**: Develop end to end visual augmented Q&A using Vision-RAG.
7. **Module 4**: Setting up vector database as retriever for vision-RAG.
8. **Module 5**: Using Vector DB as Retriever and ColPali as re-ranker.
9. Key Takeaways & Conclusion 

There are multiple notebooks available there. Here are short descriptions which may help to quickly follow.

1. `1_search_with_colpali_late_interaction`: This notebook demostrate how to perform query search over a PDF which also includes searching over all the infographics provided in PDF.

2. `2_prompting_qa_using_multi_modal_llm`: This notebook demonstrate processing and integrating visual language information for Qwen Model to generate answers for given query.

3. `3_develop_vision_rag_end_to_end`: This notebook combines the first two notebooks to develop end-to-end process of Vision-RAG.
