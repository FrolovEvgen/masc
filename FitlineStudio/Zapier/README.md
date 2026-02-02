# FitLife Studio Chatbot

AI Business Chatbot with Zapier Automation

![Chat screen](./main.png)

## Overview

**FitLife Studio Chatbot** is a business-oriented AI chatbot built with Zapier to automate lead generation, client communication, and administrative workflows for a fitness studio.

The chatbot conducts structured dialogs, collects leads, stores conversation transcripts, and notifies administrators via email when a client requests contact or a trial session.

This case demonstrates conversational design, automation logic, structured data collection, and KPI-driven chatbot behavior.

## Business Context

* **Industry**: Fitness / Wellness
* **Location**: Lviv, Ukraine
* **Primary Business Goal**: Increase bookings for free trial sessions
* Secondary Goals:
  - Reduce administrator workload
  - Capture and structure leads
  - Maintain consistent client communication

## Implemented Logic (Zapier-Based)

The chatbot is fully integrated with Zapier and implements the following automations:

* Lead collection into Google Sheets
* Conversation transcript storage in Google Sheets
* Email notification to the administrator when:
  - A client submits name + phone number
  - A callback request is created
* Button-driven dialog flows
* Structured data validation for automation triggers

## Goals

* Convert conversations into free trial session bookings
* Collect structured contact data for follow-up
* Automate responses to 60–70% of typical client questions
* Maintain a friendly, motivating brand experience
* Ensure predictable automation behavior

## User Greeting

see : [greeting.md](./instructions/greeting.md)

## Prompt Design

see : [directive.md](./instructions/directive.md)

## Assistant Role

The chatbot acts as a **business assistant** for FitLife Studio and is designed to:

1. Answer common questions about the studio
2. Book clients for a free trial session (primary objective)
3. Collect contact details for lead generation
4. Inform about pricing, services, and policies
5. Support existing clients with basic administrative information
6. Reduce administrator workload via automation

## Style Guidelines

* Clear and polite communication
* Friendly and motivational tone
* Address users by name when available
* No pressure or aggressive sales language
* Emojis used sparingly (1–2 per message max)
* Short, concise responses
* Empathy for beginners and hesitant users

## Safety & Business Rules

The chatbot must never:

* Provide medical or health advice
* Promise specific fitness results
* Compare FitLife Studio to competitors
* Provide legal or financial advice
* Invent information not present in the knowledge base

If a user asks to speak with a human, the chatbot immediately provides administrator contact details.

## Core Conversion Flow (Free Trial Session)

```text
[ User expresses interest ]
        ↓
[ Confirm availability of free trial ]
        ↓
[ Collect name ]
        ↓
[ Collect phone number ]
        ↓
[ Ask preferred workout type ]
        ↓
[ Confirm data ]
        ↓
[ Notify administrator ]
        ↓
[ Save lead to Google Sheets ]
```

The administrator contacts the client to finalize scheduling.

## Callback Request Handling (Critical Logic)

Zapier automation **requires strictly structured input**.

### Required format:

```text
Name: [client name]
Phone: [phone]
Type: Callback
```

### Behavior rules:

* Free-form messages are rejected
* The bot reformats extracted data into a copy-ready template
* Automation triggers only after correct formatting
* A Zapier-generated button appears automatically

This guarantees reliable downstream processing.

## Interaction Options (Predefined Buttons)

Users can interact via predefined dialog buttons, such as:

* Book a free trial session
* Learn about the studio
* View pricing
* Request a callback

Button-based interaction ensures clarity and reduces user friction.

Here used "Suggestios"

![Chat screen](./logic/suggestions.png)

## ZAP Logic

### Display button

![Zap button](./logic/zap_button.png)

see : [ZAP Logic Details](./logic/zap_button.md)

### Collect leads

![Collect Leads](./logic/collect_leads.png)

see : [ZAP Logic Details](./logic/collect_leads.md)

### Run zap

![Run Zap](./logic/run_zap.png)

see : [ZAP Logic Details](./logic/run_zap.md)

## Data Stored (Google Sheets)

Each successful interaction stores:

* Date and time
* Client name
* Phone number
* Email
* Preferred workout type
* Full conversation transcript

## Administrator Notifications

When a lead is created, Zapier sends an email to the administrator containing:

* Client name
* Phone number
* Request type
* Instruction to contact the client

This ensures zero lead loss.

## Key Skills Demonstrated

* Zapier-based chatbot orchestration
* Structured data collection and validation
* Lead generation workflows
* Button-driven conversational UX
* KPI-oriented chatbot design
* Automation reliability and error prevention
 
## Why This Case Matters

This chatbot is designed as a **conversion-focused business tool**, not just a conversational demo.

It demonstrates:

* Real-world automation constraints
* Human-in-the-loop handoff
* Scalable lead generation
* Measurable business impact

## Possible Extensions

* Online scheduling integration
* CRM synchronization
* Multi-language support
* Analytics dashboard for conversion tracking
* A/B testing of dialog flows

## Summary

* FitLife Studio Chatbot showcases the ability to design AI-powered business chatbots that combine conversation, automation, and measurable outcomes.
* It complements healthcare-oriented bots by demonstrating:
* Commercial logic
* Automation-first thinking
* Reliable integration design