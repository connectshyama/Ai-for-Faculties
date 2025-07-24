# FILE: plan.md
# Project Blueprint: The AI-Habitathon LMS

## 1. Project Vision
To build a mobile-only LMS and community platform that delivers a 21-day AI habit-formation bootcamp for engineering faculty. The platform will feature a core mobile app for management/creation and will leverage WhatsApp for high-engagement daily interactions.

## 2. Major Phases
* **Phase 0: Foundation & Setup.** Establish the technical groundwork, including project structures, dependencies, and basic server setup.
* **Phase 1: Core MVP - The Onboarding & Learning Experience.** Build the absolute minimum required to run the bootcamp for a single user. This includes mobile OTP authentication, the ability to display curriculum content, and a basic interface for AI interaction.
* **Phase 2: The Community Engine.** Develop the features that create a network effect: the Custom Agent Builder and the Community Template Store with its rating and moderation systems.
* **Phase 3: The WhatsApp Integration.** Tackle the complex but strategic integration with the WhatsApp Business API to enable conversational interaction with AI agents.
* **Phase 4: Content & Curriculum Implementation.** A parallel track to input the 150+ tasks and all curriculum content into the CMS/database.

## 3. Iterative Breakdown (Phase 0 & 1 - The MVP)

This breakdown details the small, incremental steps to build a functional Minimum Viable Product.

### Phase 0: Foundation
* **Chunk 0.1:** Set up the Node.js/Express backend project with basic dependencies.
* **Chunk 0.2:** Create a basic Express server and define the User model in MongoDB.
* **Chunk 0.3:** Set up the React Native mobile app project.

### Phase 1: Core MVP
* **Epic 1: User Authentication (Mobile OTP)**
    * **Chunk 1.1:** Create the 'Enter Mobile Number' screen in the React Native app.
    * **Chunk 1.2:** Create the backend API endpoint (`/api/auth/generate-otp`) that generates an OTP and sends it via an SMS service (e.g., Twilio).
    * **Chunk 1.3:** Wire the mobile app screen to the backend API.
    * **Chunk 1.4:** Create the 'Enter OTP' screen in the React Native app.
    * **Chunk 1.5:** Create the backend API endpoint (`/api/auth/verify-otp`) that verifies the OTP and returns a JWT (JSON Web Token).
    * **Chunk 1.6:** Implement token storage on the mobile app and create a basic authenticated "Home" screen.

* **Epic 2: Curriculum Display**
    * **Chunk 2.1:** Create backend models for Tracks, Modules, and Tasks.
    * **Chunk 2.2:** Create a backend API endpoint to fetch the curriculum for a user's assigned track.
    * **Chunk 2.3:** Create a UI in the React Native app to display the list of modules and tasks for the user's journey.

* **Epic 3: Basic AI Interaction**
    * **Chunk 3.1:** Create a backend API endpoint (`/api/ai/chat`) that takes a user prompt and securely forwards it to a foundational LLM (like Google's Gemini API).
    * **Chunk 3.2:** Create a simple chat interface screen in the React Native app.
    * **Chunk 3.3:** Wire the chat UI to the backend chat API, allowing a logged-in user to send a prompt and receive a response.
