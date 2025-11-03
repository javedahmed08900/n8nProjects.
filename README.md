# **PROJECT NO. 01**

# ﻿**RAG AI Agent (n8n Workflow)**

# **Overview**

The RAG AI Agent, developed using the n8n automation platform, is an intelligent system designed to provide accurate, context-aware answers from large documents. This project integrates Retrieval-Augmented Generation (RAG) architecture with Google Gemini and Pinecone Vector Database to deliver precise information retrieval and conversational AI capabilities.

# **Objective**

The  primary  objective  of  this  project  is  to  create  an  automated  assistant  capable  of answering  user  queries  based  on  the  content  of  the  Microsoft  2024  Annual  Report, providing detailed and data-backed responses in real time through WhatsApp.

# **Core Components**

- **Platform:** n8n (No-Code Workflow Automation)
- **AI Model:** Google Gemini 
- **Vector Database:** Pinecone
- **Data Source:** Microsoft 2024 Annual Report (PDF stored on Google Drive)
- **User Interface:** WhatsApp (for queries and AI responses)


# **Key Features**

- Implements  a  Retrieval-Augmented  Generation  (RAG)  framework  for  highly  relevant responses.
- Automates document download, embedding generation, and data retrieval through n8n nodes.
- Enables real-time interaction with users via WhatsApp.
- Ensures accurate, context-based answers by leveraging document embeddings stored in Pinecone.
- Fully customizable   can be adapted for any document or dataset.

# **Workflow Process**

1. **Trigger:** The workflow starts when a WhatsApp message is received from the user.
1. **Data Retrieval:** The system downloads the Microsoft Annual Report from Google Drive.
1. **Embedding Creation:** The Google Gemini model generates vector embeddings for the document text.
1. **Storage:** These embeddings are stored in the Pinecone Vector Database.
1. **Question Processing:** When a user sends a query, the AI retrieves the most relevant sections from Pinecone.
6. **Response Generation:** The Gemini model crafts a clear, detailed response using the retrieved content.
6. **Delivery:** The AI s response is sent back to the user on WhatsApp automatically.

# **Technical Nodes Used in Workflow**

- Manual Trigger   Used for testing and manual execution.
- Google Drive Node   Downloads the document file.
- Embeddings Node (Google Gemini)   Converts text into vector representations.
- Pinecone Vector Store   Stores and retrieves embeddings for document-based queries.
- WhatsApp Trigger   Captures user messages as input.
- AI Agent Node   Processes questions and generates responses using Gemini.
- Send Message Node   Sends the generated answers to the user via WhatsApp.

# **Use Cases & Benefits**

- Enterprise Knowledge Assistants   Quickly extract insights from corporate reports.
- Customer Support Bots   Provide instant document-based responses.
- Educational Tools   Summarize and explain academic content interactively.
- Data Accessibility   Makes complex reports accessible to non-technical users through WhatsApp.




# **PROJECT NO. 02**
# ﻿**Doctor Appointment AI Agent**

# **Overview**

The  Doctor  Appointment  AI  Agent,  developed  on  the  n8n  automation  platform,  is  an intelligent  WhatsApp-based  assistant  that  automates  the  entire  doctor  appointment booking process. The system combines AI-powered conversation flow, Google Sheets database  integration and enabling  a  seamless digital clinic experience for patients.

# **Objective**

To design an intelligent and user-friendly WhatsApp agent that efficiently manages doctor appointment  scheduling,  rescheduling,  and  cancellations reducing  manual administrative work and improving patient experience.

# **Core Components**

- **Platform:** n8n (No-Code Automation Tool)
- **AI Model:** Google Gemini
- **Database:** Google Sheets (Patients, Appointments, Config)
- **Interface:** WhatsApp (for patient communication)
- **Memory Engine:** Used n8n Simple Memory but it may be customized


# **Key Features**

- Fully automated doctor appointment system on WhatsApp.
- Smart memory tracking that remembers each users progress in conversation.
- Dynamic slot availability based on date, time and doctors schedule.
- Google Sheets integration for storing and retrieving patient and appointment data.
- Payment flexibility supports both online and Cash at Clinic. We can customize for online payment as well.
- Polite WhatsApp-friendly AI tone for enhanced user engagement.
- Automatic confirmation, reschedule, and cancellation flows.

# **Workflow Process**

1. **Trigger:** The system activates when a WhatsApp message is received from a user.
2. **Greeting:** The AI welcomes the user and displays a menu of options:

 -  New Booking
 -  My Upcoming Bookings
 -  Reschedule Booking
 -  Cancel Booking

3. **Patient Registration:**
   1. If the user is new, the agent collects name, age, and gender, and stores details in Google Sheets.
   1. Existing users can select from previously registered patients.
3. **Booking Flow:**
   1. The AI provides available dates and time slots, excluding fully booked or unavailable times.
   1. The user selects a slot and payment method.
   1. The system records the appointment and sends a confirmation message.
3. **Reschedule Flow:**
   1. The  AI  fetches  all  upcoming  appointments  and  allows  the  user  to  select  one  for rescheduling.
   1. It provides available dates and times, then updates the appointment details.

3. **Cancellation Flow:**
   1. The user can view upcoming appointments and choose one to cancel.
   1. The AI updates the record in Google Sheets and confirms the cancellation.

# **Technical Nodes Used in Workflow**

- WhatsApp Trigger   Initiates workflow from user messages.
- Google Gemini Chat Model   Generates natural, friendly AI responses.
- Simple Memory Node   Maintains context of the ongoing conversation.
- Google  Sheets  Nodes    Handle  CRUD  operations  for  Patients,  Appointments,  and Config.
- Date & Time Node   Manages time-based logic for slot availability.
- AI Agent Node   Central logic engine coordinating responses and actions.
- Send Message Node   Sends confirmations, updates, and reminders via WhatsApp.
 
# **Use Cases & Benefits**

- Clinics and Hospitals   Automate front-desk appointment handling.
- Doctors   Manage multiple patients efficiently with zero manual scheduling.
- Patients   Book, reschedule, or cancel appointments instantly through WhatsApp.
- Scalability   Easily customizable for multiple doctors or clinic branches.


# **Outcome**

This project demonstrates the potential of AI-driven automation in healthcare operations, combining  natural  language  processing,  no-code  workflow  design,  and  real-time  data management into a single seamless experience.



# **PROJECT NO. 03**
﻿# **Weather Prediction AI Agent**

# **Overview**

The Weather Prediction Agent is an AI-powered automation workflow developed in n8n that delivers real-time weather updates, short-term forecasts, and safety alerts through an interactive chat interface. It integrates OpenAI GPT-4.1-mini, SerpAPI, and Wikipedia tools to ensure precise, context-aware, and location-specific weather reports. The assistant intelligently interprets user queries and responds in a structured, professional, and concise manner.


# **Objective**

The main objective of the Weather Prediction Agent project is to develop an intelligent, AI-based system that simplifies access to accurate and timely weather information. The assistant aims to enhance user experience by delivering location-specific forecasts, actionable safety advice, and reliable meteorological insights. By combining AI reasoning with real-time data retrieval, the project demonstrates how automation can make complex information easily understandable and accessible through natural conversation.

# **Core Components**

-  Platform: n8n (No-Code Automation Tool)   
-  OpenAI GPT-4.1-mini Model for natural language understanding and text generation.   
-  SerpAPI & Wikipedia Integrations for live weather data and factual enhancement. 
-  Used Simple Memory, It can be customized.


# **Key Features**

-  **Real-Time Weather Data:** Retrieves live weather information from SerpAPI for any global location.   
-  **Conversational AI Interface:** Interprets user messages naturally and provides structured weather reports.   
-  **Contextual Memory:** Stores recent chat data for smooth, multi-turn conversations.   
-  **Knowledge Enhancement:** Uses Wikipedia for contextual meteorological explanations.   
-  **Smart Localization:** Automatically displays temperature in Celsius and wind speed in mph, depending on the users region.   


# **Workflow Process**

1. **Chat Trigger Activation:** The workflow begins when a user sends a message (e.g.,  What s the weather in Dubai? ).
2. **AI Agent Initialization:** The AI Agent interprets the query, identifies missing details such as location, and prepares a structured     response plan.
3. **Data Retrieval via Tools:** SerpAPI Node fetches live weather data and Wikipedia Node provides supporting background information or explanations.
4. **Response Generation:** The OpenAI GPT-4.1-mini model processes all retrieved information and generates a concise, professional weather  report.
5. **Memory Handling:** Used Simple memory but it may be customized.
6. **Final Output:** The assistant delivers the final message containing current weather, short-term forecast, and any alerts or advice.

# **Technical Nodes Used in Workflow**

-  **When Chat Message Received:** Triggers the workflow whenever a user sends a chat query.   
-  **AI Agent:** Acts as the main controller, processing user messages and managing responses.   
-  **OpenAI Chat Model:** Generates accurate and natural language responses.  
-  **Simple Memory:** Maintains short-term chat context for coherent conversation.  
-  **Wikipedia Tool:** Retrieves relevant meteorological knowledge for enhanced explanations.   
-  **SerpAPI Tool:** Collects live and accurate weather data for requested locations.

# **Use Cases & Benefits**

-  **Daily Forecasting:** Provides users with up-to-date weather information anytime.
-  **Travel Planning:** Helps travelers and outdoor enthusiasts plan based on accurate forecasts.   
-  **Emergency Awareness:** Issues timely alerts and safety guidelines during severe weather.   
-  **Business Operations:** Supports logistics, agriculture, and event management sectors that depend on weather data.  

# **Outcome**

The Weather Prediction Agent successfully showcases how AI, automation, and real-time data integration can be combined within n8n to create a fully functional, conversational weather assistant. The system delivers accurate information with human-like interaction, offering an efficient and professional user experience. This project stands as a practical example of how no-code AI workflows can power intelligent digital solutions for both personal and enterprise applications.




# **PROJECT NO. 04**
﻿# **Inventory Management AI Agent**

# **Overview**

The Inventory Management AI Agent is an intelligent automation workflow built within n8n that manages inventory tracking, updates, and communication through WhatsApp. It integrates OpenAI GPT-4.1-mini, Google Sheets, and voice-to-text transcription to process both text and audio inputs from users. This system bridges human interaction and AI-powered automation, providing a seamless way to manage product data without manual effort.

# **Objective**

The primary objective of this project is to simplify inventory management using a conversational AI interface. Through WhatsApp messages, business owners can easily check stock, update item quantities, or add new entries without logging into spreadsheets. By combining AI reasoning, workflow automation, and real-time data handling, this solution ensures efficient, accurate, and effortless stock management for small and medium-sized businesses.

# **Core Components**

-  **Platform:** n8n (No-Code Automation Tool)
-  **OpenAI GPT-4.1-mini:** Handles natural language understanding and action interpretation. 
-  **Google Sheets Integration:** Acts as the centralized database for storing and updating product information.  
-  **WhatsApp Trigger & API:** Enables seamless user interaction via messages or voice notes.  
-  **Audio Transcription:** Converts voice inputs into text for further processing.  
-  **Switch & HTTP Nodes:** Manage data flow, detect message type, and handle file downloads.

# **Key Features**

-  **WhatsApp Trigger:** Captures incoming messages and starts the workflow.   
-  **Smart Message Handling:** Differentiates between text and voice messages automatically.   
-  **Audio Transcription:** Converts WhatsApp voice notes into text commands.   
-  **AI Agent:** Understands user intent and performs relevant inventory actions.   
-  **Google Sheets Integration:** Retrieves and updates records dynamically, supports both appending and modifying data.   
-  **Automated Response System:** Sends real-time confirmations and updates back to the user via WhatsApp.

# **Workflow Process**

1. **WhatsApp Trigger:** Activates when a user sends a message (text or voice).
2. **Switch Node:** Identifies message type and directs flow.
3. **Voice Message Path:** WhatsApp Node retrieves the audio URL, HTTP Node downloads the voice file, and OpenAI Transcription converts it into text.
4. **AI Agent Analysis:** Processes the text, identifies the command, and prepares an action.
5. **Google Sheets Update:** Automatically appends or modifies stock data.
6. **Message Response:** AI sends a structured confirmation message through WhatsApp.

# **Technical Nodes Used in Workflow**

-  **WhatsApp Trigger Node:** Captures incoming messages.  
-  **Switch Node:** Routes text and audio inputs.   
-  **HTTP Request Node:**  Downloads audio files.  
-  **OpenAI Transcription Node:** Transcribes voice to text.   
-  **AI Agent Node:** Processes intent and decides actions.  
-  **Google Sheets Nodes:** Fetch and update inventory data. 
-  **Send Message Node:** Sends final response back to WhatsApp.

# **Use Cases**

-  **Business Automation:** Manage stock directly through WhatsApp without manual entry.   
-  **Voice-Based Control:** Add or check items using simple voice commands.   
-  **Real-Time Updates:** Instantly reflect inventory changes in Google Sheets.  
-  **Accuracy & Efficiency:** Reduces manual data errors and improves speed.   
-  **Smart AI Workflow:** Demonstrates the potential of AI-powered, no-code business systems.

# **Outcome**

The Inventory Management AI Agent successfully demonstrates how AI, automation, and voice processing can work together to create a fully functional conversational inventory assistant. It allows users to manage products hands-free while maintaining synchronized data in real time. This project highlights the power of no-code AI automation in n8n for building intelligent business management systems that save time, reduce effort, and enhance productivity.










