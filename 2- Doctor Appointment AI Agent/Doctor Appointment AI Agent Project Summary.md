**Doctor Appointment AI Agent (n8n Workflow)**

**Overview**

The  Doctor  Appointment  AI  Agent,  developed  on  the  n8n  automation  platform,  is  an intelligent  WhatsApp-based  assistant  that  automates  the  entire  doctor  appointment booking process. The system combines AI-powered conversation flow, Google Sheets database  integration and enabling  a  seamless digital clinic experience for patients.

**Core Components**

- Platform: n8n (No-Code Automation Tool)
- AI Model: Google Gemini
- Database: Google Sheets (Patients, Appointments, Config)
- Interface: WhatsApp (for patient communication)
- Memory Engine: Used n8n Simple Memory but it may be customized

**Objective**

To design an intelligent and user-friendly WhatsApp agent that efficiently manages doctor appointment  scheduling,  rescheduling,  and  cancellations    reducing  manual administrative work and improving patient experience.

**Key Features**

- Fully automated doctor appointment system on WhatsApp.
- Smart memory tracking that remembers each users progress in conversation.
- Dynamic slot availability based on date, time and doctors schedule.
- Google Sheets integration for storing and retrieving patient and appointment data.
- Payment flexibility supports both online and Cash at Clinic. We can customize for online payment as well.
- Polite WhatsApp-friendly AI tone for enhanced user engagement.
- Automatic confirmation, reschedule, and cancellation flows.

**Workflow Process**

1. Trigger:The system activates when a WhatsApp message is received from a user.
2. Greeting: The AI welcomes the user and displays a menu of options:

 -  New Booking
 -  My Upcoming Bookings
 -  Reschedule Booking
 -  Cancel Booking

3. Patient Registration:
   1. If the user is new, the agent collects name, age, and gender, and stores details in Google Sheets.
   1. Existing users can select from previously registered patients.
3. Booking Flow:
   1. The AI provides available dates and time slots, excluding fully booked or unavailable times.
   1. The user selects a slot and payment method.
   1. The system records the appointment and sends a confirmation message.
3. Reschedule Flow:
   1. The  AI  fetches  all  upcoming  appointments  and  allows  the  user  to  select  one  for rescheduling.
   1. It provides available dates and times, then updates the appointment details.
3. Cancellation Flow:
   1. The user can view upcoming appointments and choose one to cancel.
   1. The AI updates the record in Google Sheets and confirms the cancellation.

**Technical Nodes Used in Workflow**

- WhatsApp Trigger   Initiates workflow from user messages.
- Google Gemini Chat Model   Generates natural, friendly AI responses.
- Simple Memory Node   Maintains context of the ongoing conversation.
- Google  Sheets  Nodes    Handle  CRUD  operations  for  Patients,  Appointments,  and Config.
- Date & Time Node   Manages time-based logic for slot availability.
- AI Agent Node   Central logic engine coordinating responses and actions.
- Send Message Node   Sends confirmations, updates, and reminders via WhatsApp.

**Use Cases & Benefits**

- Clinics and Hospitals   Automate front-desk appointment handling.
- Doctors   Manage multiple patients efficiently with zero manual scheduling.
- Patients   Book, reschedule, or cancel appointments instantly through WhatsApp.
- Scalability   Easily customizable for multiple doctors or clinic branches.


**Outcome**

This project demonstrates the potential of AI-driven automation in healthcare operations, combining  natural  language  processing,  no-code  workflow  design,  and  real-time  data management into a single seamless experience.



