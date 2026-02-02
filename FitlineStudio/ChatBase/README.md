# FitLife Studio AI Agent

AI Business Chatbot on Chatbase platform.

![Chat screen](./main.png)

---

## Overview
FitLife Studio AI Agent is a customer-facing AI assistant built on Chatbase for a fitness studio in Lviv, Ukraine.  
The bot serves as a 24/7 virtual consultant that answers client questions, promotes studio services, and primarily converts new visitors into leads by booking free trial workouts.

---

## Business context
FitLife Studio needed an automated solution to:
- Reduce administrator workload
- Handle repetitive questions
- Capture and qualify leads outside working hours
- Increase trial workout bookings through conversational AI

The AI agent replaces the first line of communication while preserving a human handoff when required.

---

## Platform
* **Industry**: Fitness / Wellness
* **Platform**: Chatbase
* **Primary Business Goal**:
  - Increase free trial workout bookings and lead collection
* **Secondary Goals**:
  - Provide instant answers to FAQs
  - Improve customer experience
  - Route complex or sensitive requests to a human administrator

---

## Implemented Logic

see : [README.md](./logic/README.md)

---

## Assistant Scope

### Assistant Role
- Acts as an official AI representative of FitLife Studio
- Guides users toward a free trial workout (priority conversion flow)
- Collects name, phone number, and preferred training type
- Provides accurate information about pricing, schedules, services, and policies
- Redirects users to an administrator when confidence is low or requests are complex

### Style Guidelines
- Friendly, motivating, and professional tone
- Short, clear answers without overload
- Empathy toward beginners
- Limited emoji usage (1–2 per message)
- Personalization using the client’s name when available

### Safety & Business Rules
- No medical, legal, or financial advice
- No promises of guaranteed results
- No competitor comparisons
- No fabricated information
- Mandatory handoff if information is missing or confidence score is low

---

## Key Skills Demonstrated
- AI prompt engineering for business goals
- Conversational UX design
- Lead generation via chat
- Knowledge base structuring (FAQ + website ingestion)
- Safety and compliance constraints in AI agents
- Human-in-the-loop escalation design

---

## Why This Case Matters
This project demonstrates how a well-structured system prompt and knowledge base can turn a simple chatbot into a conversion-focused AI sales assistant without external integrations or custom code.

---

## Possible Extensions
- CRM integration for automatic lead syncing
- Analytics-based optimization of conversion flows
- Multilingual support
- Integration with booking or calendar systems
