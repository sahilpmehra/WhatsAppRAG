# Creating a WhatsApp RAG Bot using GPT3.5, LangChain and ChromaDB

## Objective 🎯

This project utilizes GPT3.5 Turbo, LangChain and ChromaDB to establish a Retrieval Augmented Generation (RAG) system. This system empowers one to generate replies for the user based on their past conversations on the messaging platform. The RAG even generates appropriate emojis and can relate current messages to past conversations so as to reply in the most appropriate way. Retrieval Augmented Generation works by first performing a retrieval step when presented with a question. This step fetches relevant documents from a special vector database, where the documents have been indexed.

## Technology used

* **LLM** - GPT3.5 Turbo which is a LLM by OpenAI
* **LangChain** - Framework designed to streamline the creation of applications utilizing LLMs
* **ChromaDB** - Database that organizes data using high-dimensional vectors

## Usage Examples

Here are some screenshots of results from the bot based on my style of texting respective messengers with some context for you:



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