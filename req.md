# FILE: req.md
# Product Requirements Document: The AI-Habitathon

* **Version:** 2.0
* **Status:** Final Draft
* **Author:** Shyam & Shyam's Ideation Partner
* **Date:** July 24, 2025

## 1. Introduction & Executive Summary
The "AI-Habitathon" is a 21-day, in-person, mobile-first Faculty Development Program (FDP) designed to empower engineering college faculty in India. The current academic environment places immense pressure on faculty to excel in teaching, administration, and research, often with limited time and resources. While aware of AI, many lack a practical, structured path to integrate it into their daily work.

This project solves this by providing a hands-on, gamified learning journey that transforms faculty from AI-curious novices into AI-proficient innovators. The core experience is delivered via a mobile LMS app, but its true innovation lies in a "WhatsApp-first" interaction model and a community-driven ecosystem where advanced users build and share AI tools for their peers.

## 2. Strategic Goals & Success Metrics

### 2.1. Business Goals
* Secure institutional contracts for the 21-day FDP at the target price point.
* Achieve high satisfaction and generate powerful testimonials from the initial client (Sairam Institutions).
* Build a defensible moat through a vibrant, self-sustaining "Community Template Store".
* Establish the AI-Habitathon as the premier AI training program for academic institutions in the region.

### 2.2. User Goals
* **For Faculty:** To save significant time on repetitive tasks, enhance the quality of their teaching materials, accelerate their research process, and gain the confidence to lead AI adoption in their departments.
* **For Institutions:** To upskill their faculty, improve overall academic productivity, and enhance their reputation as a forward-thinking, tech-enabled institution.

### 2.3. Key Success Metrics (First 3 Bootcamps)
* **Engagement:** >80% Daily Active Users (DAU) within the app/WhatsApp during the 21-day program.
* **Completion:** >90% of participants complete the full 21-day journey.
* **Proficiency:** >20% of users reaching "AI-Innovator" or "AI-Catalyst" track by the end of the program.
* **Community Growth:** >50 community-generated templates published to the "Template Store" per bootcamp.
* **Satisfaction:** Net Promoter Score (NPS) of +50 or higher from participating faculty.

## 3. Target Audience & User Personas
The primary audience is full-time faculty at engineering colleges in Tamil Nadu. Users will be segmented into one of five personas (Tracks) upon entering the program.

* **Persona 1: The AI-Curious:** Skeptical or unsure where to start. Goal is to understand the relevance of AI.
* **Persona 2: The AI-Explorer:** Have tried AI casually. Goal is to learn foundational prompting skills.
* **Persona 3: The AI-Adopter:** Use AI periodically. Goal is to build a consistent habit and integrate it into their workflow.
* **Persona 4: The AI-Innovator:** Proficient users. Goal is to learn how to build their own custom AI agents.
* **Persona 5: The AI-Catalyst:** Advanced users. Goal is to learn how to lead AI adoption and mentor others.

## 4. User Journey & High-Level Flow

1.  **Ignition Session (Pre-Bootcamp):** Faculty attend a 90-minute in-person workshop one week before the program. This session builds excitement and crowdsources their real-world tasks via an interactive sticky-note exercise.
2.  **Onboarding (Day 1):**
    * Users download the mobile app and register using their mobile number and a one-time password (OTP).
    * The system sends a welcome message to their WhatsApp, establishing the primary interaction channel.
    * Users complete a 10-minute, hands-on "AI Aptitude Test" within the app.
    * Based on the test, they are assigned to one of the 5 Tracks and see a celebratory "Cohort Reveal" screen.
3.  **The 21-Day Habitathon:**
    * For 1-2 hours each day, users engage with the curriculum.
    * They complete tasks within their assigned module (Teaching, Admin, or Research).
    * Interaction can happen within the app or, for many tasks, directly via WhatsApp.
4.  **Graduation & Beyond:**
    * Users receive a tiered "AI Belt" certificate based on their final proficiency level.
    * Innovators and Catalysts are encouraged to publish their tools to the "Community Template Store."
    * All users remain part of the community, able to use the tools and continue their learning.

## 5. Detailed Feature Requirements

### 5.1. Core Platform & Architecture
* **FR1: Mobile-Only Application:** The LMS app must be built for and exclusively accessible on iOS and Android smartphones.
* **FR2: WhatsApp-First Interaction Model:** The system architecture must support deep integration with the WhatsApp Business API.

### 5.2. Feature: User Authentication
* **REQ-1.1:** Users must register and log in using their mobile number.
* **REQ-1.2:** The system must generate and send a time-sensitive (e.g., 10-minute) OTP via SMS for verification.
* **REQ-1.3:** Upon successful verification, the system must create a secure user session (e.g., using a JWT).

### 5.3. Feature: Onboarding & Assessment
* **REQ-2.1:** The app must present a sequence of escalating, practical tasks.
* **REQ-2.2:** The system must allow users to upload files (PDF, TXT, JPG) from their phone as part of the assessment.
* **REQ-2.3:** The system must automatically assign a user to one of the 5 Tracks based on their performance.
* **REQ-2.4:** The app must display a visually engaging "Cohort Reveal" screen post-assessment.

### 5.4. Feature: Curriculum & Learning Interface
* **REQ-3.1:** The app must display the curriculum in a structured format of Tracks and Modules.
* **REQ-3.2:** The task interface must provide a chat-like view for interacting with the AI.
* **REQ-3.3:** Users must be able to mark tasks as complete to track their progress through the 21-day program.

### 5.5. Feature: Custom Agent Builder (Mobile-First)
* **REQ-4.1:** Users must have an interface to create a new "Custom Agent."
* **REQ-4.2:** The interface must allow users to provide a Name, Description, and detailed Instructions (persona) for their agent.
* **REQ-4.3:** The interface must allow users to upload one or more documents (PDF, TXT) to serve as the agent's knowledge base.
* **REQ-4.4:** Users must be able to save, test, and iteratively refine their agents within the app.

### 5.6. Feature: Community Template Store
* **REQ-5.1:** The app must feature a gallery view to browse all community-published agents.
* **REQ-5.2:** The gallery must be searchable and sortable by categories, usage, and user ratings.
* **REQ-5.3:** Each template must display its creator's name, department, college, rating, and usage count.
* **REQ-5.4:** Users must be able to use a template with one click.
* **REQ-5.5:** Users must be able to rate a template (e.g., 1-5 stars) and flag it as "inappropriate" or "non-working."
* **REQ-5.6:** There must be an admin backend to review and manage flagged templates.
* **REQ-5.7:** Creators ("Innovators" and "Catalysts") must have a workflow to submit their custom agents for publication in the store.

### 5.7. Feature: WhatsApp Integration
* **REQ-6.1:** The system backend must be connected to the WhatsApp Business API.
* **REQ-6.2:** On successful user registration, the system must send an automated welcome message to the user's WhatsApp number.
* **REQ-6.3:** The system must be able to parse incoming WhatsApp messages from registered users.
* **REQ-6.4:** A user must be able to invoke a specific template via a command (e.g., `/use <template_name> <prompt>`).
* **REQ-6.5:** The backend must route the user's prompt to the correct AI agent, get the response, and deliver it back to the user within WhatsApp.

## 6. Out of Scope (For Version 1)
* A desktop version of the application.
* Email/Password-based login systems.
* Direct payment processing within the app.
* Bootcamps for non-engineering disciplines or K-12 schools.
* A formal, top-down quality approval gate for the Community Template Store (relying on community moderation instead).
