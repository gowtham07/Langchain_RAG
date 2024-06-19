# Langchain_RAG
Uses Langchain, ChromaDB, Hugginsface LM 

The notebook shows why RAG is important in the context of Retreival from large language models. LLM's tend to hallucinate when they dont have any idea about particular information.
This could be a drawback as retraining or finetuning a LLM is costly, though we have PEFT methods to finetune only a part of weights we do need a gpu and memory requirements. Also keeping the model upto date is difficult, this is where the RAG is useful. We vectorize the documents with information and store them in a vector database ( different to a normal relational DB), upon the users prompt the relevant context is then added as context with the user prompt and sent to the LLM to answer the question, this helps the model in a way to curb hallucinating and provide with actual or near to actual answer. 

In the above notebbok I have embedded a text file related to telugu language, you can find the answers from the LLM before and after the RAG.

Update: Working on a sophisticated RAG for Question and Answer PipeLine
