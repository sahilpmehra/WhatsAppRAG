# Creating a WhatsApp RAG Bot using GPT3.5, LangChain and ChromaDB

## Objective 🎯

This project utilizes GPT3.5 Turbo, LangChain and ChromaDB to establish a Retrieval Augmented Generation (RAG) system. This system empowers one to generate replies for the user based on their past conversations on the messaging platform. The RAG even generates appropriate emojis and can relate current messages to past conversations so as to reply in the most appropriate way. Retrieval Augmented Generation works by first performing a retrieval step when presented with a question. This step fetches relevant documents from a special vector database, where the documents have been indexed.

## Technology used

* **LLM** - GPT3.5 Turbo which is a LLM by OpenAI
* **LangChain** - Framework designed to streamline the creation of applications utilizing LLMs
* **ChromaDB** - Database that organizes data using high-dimensional vectors

## Usage Examples

Here are some screenshots of results from the bot based on my style of texting respective messengers with some context for you:

* **Context**: The sender (Puneet) had asked the user (Sahil) to contact another friend (Shubhankar) for some help the sender required. The RAG was able to understand what the sender was referring to without any reference of the subject in the message and also reply accurately based on another contact's (Bua's) messages with the user (Sahil).

  ![Screenshot 2024-06-17 at 3 32 50 AM](https://github.com/sahilpmehra/WhatsAppRAG/assets/25867566/85d5fdb8-bcba-4de3-a1c6-ad3e1b7ad02d)

* **Context**: The sender (Cchinmayy) sends the user a message which is a mix of Hindi and English. The RAG not only understands the message but also replies uncannily similarly to how the user (Sahil) would have in this situation. The second image shows another equally plausible reply to the message (again in a mix of Hindi and English) - this can be used to provide the user with options before sending a reply.
  
  ![Screenshot 2024-06-17 at 3 27 19 AM](https://github.com/sahilpmehra/WhatsAppRAG/assets/25867566/bc87e1d7-098b-469c-b7ad-2dbf5efb2009)

  ![Screenshot 2024-06-17 at 3 27 32 AM](https://github.com/sahilpmehra/WhatsAppRAG/assets/25867566/8612aca9-e8f9-431a-8a91-22ebe9250a8f)


* **Context**: This is a rare case where the RAG is hallucinating. The sender (Shubham) and the user (Sahil) had plans for the evening in San Diego but the RAG replies that the user is in India instead. Further optimization of data embeddings required to mitigate such hallucinations.
  
  ![Screenshot 2024-06-17 at 5 03 39 AM](https://github.com/sahilpmehra/WhatsAppRAG/assets/25867566/f1944da7-f532-4211-9e8d-adb9ddaa2a8e)


## How to use

I have used Python 3.12 to build the backbone of the bot on a Jupyter notebook. All the required dependencies for this bot can be installed using requirements.txt file.

In addition to the installation, you will also need a LangChain and a OpenAI API key available. Further versions will support other LLMs such as Llama3 and Gemini.

Add your whatsapp chats with different contacts in the Whatsapp_Chats folder in .txt format (further versions will support other media formats).

Finally, pass your message (along with sender's name) as the parameter to the rag_chain.invoke("Type Message Here") function.

## Conclusions 💯🔥

This project successfully implemented a Retrieval Augmented Generation (RAG) solution by leveraging Langchain, ChromaDB, and Llama3 as the LLM. To evaluate the system's performance, we utilized the EU AI Act from 2023. The results demonstrated that the RAG model delivers accurate answers to questions posed about the Act.

## Future Work ⚡✨

* Integration with the WhatsApp Business API to let the app directly reply on WhatsApp (waiting for access from WhatsApp).
* Android and iOS apps to make this service available on your phone.
* Better mitigation of hallucinations by the LLM by optimizing the document embeddings.
* Replies based on relation with user.
* Ability to edit replies prior to sending them.

---

#### **If you like this LLM Project do drop ⭐ to this repo**
[![LinkedIn](https://img.shields.io/badge/linkedin-%230077B5.svg?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/sahil-mehra/) &nbsp; [![GitHub](https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white)](https://github.com/sahilpmehra/)

---
