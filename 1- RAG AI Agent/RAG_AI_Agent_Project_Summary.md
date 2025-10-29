**Project Summary   RAG AI Agent (n8n Workflow)**

**Overview**

The RAG AI Agent, developed using the n8n automation platform, is an intelligent system designed to provide accurate, context-aware answers from large documents. This project integrates  Retrieval-Augmented  Generation  (RAG)  architecture  with  Google  Gemini (PaLM API) and Pinecone Vector Database to deliver precise information retrieval and conversational AI capabilities.

**Core Components**

- Platform: n8n (No-Code Workflow Automation)
- AI Model: Google Gemini (PaLM API)
- Vector Database: Pinecone
- Data Source: Microsoft 2024 Annual Report (PDF stored on Google Drive)
- User Interface: WhatsApp (for queries and AI responses)

**Objective**

The  primary  objective  of  this  project  is  to  create  an  automated  assistant  capable  of answering  user  queries  based  on  the  content  of  the  Microsoft  2024  Annual  Report, providing detailed and data-backed responses in real time through WhatsApp.

**Key Features**

- Implements  a  Retrieval-Augmented  Generation  (RAG)  framework  for  highly  relevant responses.
- Automates document download, embedding generation, and data retrieval through n8n nodes.
- Enables real-time interaction with users via WhatsApp.
- Ensures accurate, context-based answers by leveraging document embeddings stored in Pinecone.
- Fully customizable   can be adapted for any document or dataset.

  **Workflow Process**

1. Trigger: The workflow starts when a WhatsApp message is received from the user.
1. Data Retrieval: The system downloads the Microsoft Annual Report from Google Drive.
1. Embedding Creation: The Google Gemini model generates vector embeddings for the document text.
1. Storage: These embeddings are stored in the Pinecone Vector Database.
1. Question Processing: When a user sends a query, the AI retrieves the most relevant sections from Pinecone.
6. Response Generation: The Gemini model crafts a clear, detailed response using the retrieved content.
6. Delivery: The AI s response is sent back to the user on WhatsApp automatically.

   **Technical Nodes Used in Workflow**

- Manual Trigger   Used for testing and manual execution.
- Google Drive Node   Downloads the document file.
- Embeddings Node (Google Gemini)   Converts text into vector representations.
- Pinecone Vector Store   Stores and retrieves embeddings for document-based queries.
- WhatsApp Trigger   Captures user messages as input.
- AI Agent Node   Processes questions and generates responses using Gemini.
- Send Message Node   Sends the generated answers to the user via WhatsApp.

**Use Cases & Benefits**

- Enterprise Knowledge Assistants   Quickly extract insights from corporate reports.
- Customer Support Bots   Provide instant document-based responses.
- Educational Tools   Summarize and explain academic content interactively.
- Data Accessibility   Makes complex reports accessible to non-technical users through WhatsApp.

**Created by: Javed Ahmed**
