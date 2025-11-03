# **Inventory Management AI Agent (n8n Workflow)**

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


