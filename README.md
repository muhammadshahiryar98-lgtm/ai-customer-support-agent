 #ai-customer-support-agent
An AI-powered customer support agent that automatically answers customer queries and provides relevant solutions using Artificial Intelligence and Natural Language Processing (NLP). Developed as a BSIT Final Year Project at The Islamia University of Bahawalpur.


 SRS(Software Requirements Specification)

1. Introduction

1.1 Purpose
The purpose of this document is to define the Software Requirements Specification (SRS) for the AI Customer Support Agent. This system will automatically handle customer queries using Artificial Intelligence, provide instant responses, and reduce the workload of human support teams.

1.2 Scope
This project is a web-based AI support system. Customers can chat with the AI agent, get answers to FAQs, track orders, and create support tickets. Admin can manage FAQs, view chats, and monitor tickets. If AI fails to answer, the query is transferred to a human agent.

1.3 Target Users
1. Customers / End Users
2. Human Support Agents
3. Admin / Business Owner

1.4 Technologies Used
Frontend: HTML, CSS, JavaScript, React
Backend: Python / http://Node.js
Database: MongoDB / MySQL
AI: NLP, LLM API (OpenAI / Gemini)
Tools: GitHub, Vercel

2. Overall Description

2.1 Product Perspective
The system will be a standalone web application integrated with a business website as a chat widget.

2.2 Product Functions
- AI Chatbot for 24/7 support
- FAQ Answering System
- Ticket Creation & Tracking
- Human Handover
- Admin Dashboard

3. Functional Requirements

3.1 User Module
- FR1: User can start chat without login / with login
- FR2: User can ask questions in natural language
- FR3: User can view previous chat history
- FR4: User can create a support ticket
- FR5: User can rate the AI response

3.2 AI Agent Module
- FR6: AI shall understand user intent using NLP
- FR7: AI shall answer from Knowledge Base / FAQs
- FR8: AI shall provide order status if order ID is given
- FR9: AI shall escalate to human agent if confidence is low
- FR10: AI shall support English and Urdu

3.3 Human Agent Module
- FR11: Agent can view live chats assigned to him
- FR12: Agent can reply to customer in real-time
- FR13: Agent can close / resolve tickets

3.4 Admin Module
- FR14: Admin can add / edit / delete FAQs
- FR15: Admin can view all chats and tickets
- FR16: Admin can view analytics: total chats, resolved, pending
- FR17: Admin can manage agents and users

4. Non-Functional Requirements*
- *Performance:* Response time should be less than 3 seconds.
- *Availability:* System should be available 24/7.
- *Security:* User data should be secure, passwords encrypted.
- *Usability:* Simple and mobile-friendly UI.
- *Scalability:* System should handle multiple users at same time.
- *Reliability:* System should not crash on invalid input.

5. Use Cases
1. Customer asks FAQ -> AI replies instantly
2. Customer asks order status -> AI asks Order ID -> Shows status
3. Customer complaint -> AI creates ticket -> Assigns to human agent
4. Admin adds new FAQ -> AI starts using it

6. Database Design
- *Users:* user_id, name, email, password
- *Chats:* chat_id, user_id, message, sender, timestamp
- *Tickets:* ticket_id, user_id, issue, status, assigned_agent
- *FAQs:* faq_id, question, answer, category

7. Future Enhancements
- Voice support
- WhatsApp integration
- Sentiment analysis

8. Conclusion
AI Customer Support Agent will improve customer experience by providing fast, accurate, and 24/7 support while reducing cost for businesses.