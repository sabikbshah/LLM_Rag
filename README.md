**Question/Answering RAG Application using Huggingface langchain.**
Setup Steps:

1. huggingface website-> signup-> login-> settings-> access token -> Copy  token,
   Inside ColabNotebook -> make two secrect key at left most keyshape icon-> copy and put into  secretkey two times with two variable names.

2. You need to run all the above using run all to run Huggingface with pipeline. As its dependencies are somewhere along used in huggingface with endpoint.

**Overview**
Used two methods HuggingFaceEndpoints and HuggingFacePipeline 
**HugginFaceEndpoints:**
An endpoint in Hugging Face refers to a REST API endpoint that allows users to deploy and interact with machine learning models   over the web such as llms models. Used for Production.
**HuggingFacePipeline:**
A pipeline in Hugging Face is a high-level abstraction that simplifies the usage of pre-trained models. can be used locally or in a hosted environment. They provide a simple interface to load and use models from the Hugging Face Model Hub. less flexibility, However, they can be fine-tuned and customized for specific requirements.
Retreival Augment Generation -> steps include:
Document -> transform to text -> Split into Chunks -> **Embedd -> Store in Vectordatabase -> 
Userquery -> **Embedd -> SimilaritySearch in Vectordatabase -> Query +  Relevant Document passed to LLM + prompt -> Response

