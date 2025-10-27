**WhatsApp RAG AI Agent with n8n** 

I built a RAG (Retrieval-Augmented Generation) AI assistant that answers questions about Microsoft's 2024 Annual Report directly through WhatsApp.

**What This Project Does**

- **RAG System:** Uses Retrieval-Augmented Generation to provide accurate answers from the Microsoft 2024 Annual Report.
- **Used the Microsoft 2024 Annual Report (PDF)** as the primary data source for retrieval and context generation.
- **Chat with Document:** Ask questions on WhatsApp, and the AI finds specific answers from the report.
- **Built with n8n:** Created the entire RAG agent visually using n8n workflow tool.
- **WhatsApp Integration:** Used WhatsApp as the trigger for conversations.
- **Pinecone Vector DB**: Stored and searched document embedding in Pinecone.
- **Google Gemini:** Used Gemini model for embedding and generating responses.

**How It Works**

- You send a question on WhatsApp (trigger).
- My n8n RAG workflow searches Pinecone for relevant information from the Microsoft report.
- Google Gemini processes the context and sends accurate answers back to WhatsApp.
- This RAG project helped me learn how to build AI agents that can chat with documents and provide reliable information.
