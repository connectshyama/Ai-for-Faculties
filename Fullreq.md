# FILE: Fullreq.md
# Product Requirements Document: The AI-Habitathon

* **Version:** 2.1
* **Status:** Final Blueprint
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

## 5. Program Structure & Pacing
The daily commitment is 1-2 hours. The pacing adapts to the user's track, ensuring a balance of challenge and achievement.

| Track | Typical Task Mix | Implication for Daily Pacing (1-2 hr session) |
| :--- | :--- | :--- |
| **1. AI-Curious** | 90% Quick Wins | Can complete **2-3 tasks per day**. |
| **2. AI-Explorer** | 50% Quick Wins, 50% Standard Tasks | Can complete **1-2 tasks per day**. |
| **3. AI-Adopter**| 70% Standard Tasks, 30% Project Tasks | Will likely focus on **one significant task per day**. |
| **4. AI-Innovator** | 80% Project Tasks, 20% Standard Tasks | Will focus on **one major project task per day**. |
| **5. AI-Catalyst**| 40% Standard Tasks, 60% Project Tasks | Will focus on **one strategic task per day**. |

## 6. Detailed Feature Requirements

### 6.1. Core Platform & Architecture
* **FR1: Mobile-Only Application:** The LMS app must be built for and exclusively accessible on iOS and Android smartphones.
* **FR2: WhatsApp-First Interaction Model:** The system architecture must support deep integration with the WhatsApp Business API.

### 6.2. Feature: User Authentication
* **REQ-1.1:** Users must register and log in using their mobile number.
* **REQ-1.2:** The system must generate and send a time-sensitive (e.g., 10-minute) OTP via SMS for verification.
* **REQ-1.3:** Upon successful verification, the system must create a secure user session (e.g., using a JWT).

### 6.3. Feature: Onboarding & Assessment
* **REQ-2.1:** The app must present a sequence of escalating, practical tasks.
* **REQ-2.2:** The system must allow users to upload files (PDF, TXT, JPG) from their phone as part of the assessment.
* **REQ-2.3:** The system must automatically assign a user to one of the 5 Tracks based on their performance.
* **REQ-2.4:** The app must display a visually engaging "Cohort Reveal" screen post-assessment.

### 6.4. Feature: Curriculum & Learning Interface
* **REQ-3.1:** The app must display the curriculum in a structured format of Tracks and Modules.
* **REQ-3.2:** The task interface must provide a chat-like view for interacting with the AI.
* **REQ-3.3:** Users must be able to mark tasks as complete to track their progress through the 21-day program.

### 6.5. Feature: Custom Agent Builder (Mobile-First)
* **REQ-4.1:** Users must have an interface to create a new "Custom Agent."
* **REQ-4.2:** The interface must allow users to provide a Name, Description, and detailed Instructions (persona) for their agent.
* **REQ-4.3:** The interface must allow users to upload one or more documents (PDF, TXT) to serve as the agent's knowledge base.
* **REQ-4.4:** Users must be able to save, test, and iteratively refine their agents within the app.

### 6.6. Feature: Community Template Store
* **REQ-5.1:** The app must feature a gallery view to browse all community-published agents.
* **REQ-5.2:** The gallery must be searchable and sortable by categories, usage, and user ratings.
* **REQ-5.3:** Each template must display its creator's name, department, college, rating, and usage count.
* **REQ-5.4:** Users must be able to use a template with one click.
* **REQ-5.5:** Users must be able to rate a template (e.g., 1-5 stars) and flag it as "inappropriate" or "non-working."
* **REQ-5.6:** There must be an admin backend to review and manage flagged templates.
* **REQ-5.7:** Creators ("Innovators" and "Catalysts") must have a workflow to submit their custom agents for publication in the store.

### 6.7. Feature: WhatsApp Integration
* **REQ-6.1:** The system backend must be connected to the WhatsApp Business API.
* **REQ-6.2:** On successful user registration, the system must send an automated welcome message to the user's WhatsApp number.
* **REQ-6.3:** The system must be able to parse incoming WhatsApp messages from registered users.
* **REQ-6.4:** A user must be able to invoke a specific template via a command (e.g., `/use <template_name> <prompt>`).
* **REQ-6.5:** The backend must route the user's prompt to the correct AI agent, get the response, and deliver it back to the user within WhatsApp.

## 7. Out of Scope (For Version 1)
* A desktop version of the application.
* Email/Password-based login systems.
* Direct payment processing within the app.
* Bootcamps for non-engineering disciplines or K-12 schools.
* A formal, top-down quality approval gate for the Community Template Store (relying on community moderation instead).

## 8. Detailed Curriculum Blueprint: 150 Tasks
This section contains the full task list for the 21-day program, broken down by Track and Module.

---
### **Track 1: AI-Curious**
*Goal: To move from skepticism to seeing personal relevance across all three work pillars.*

#### **Module 1.1: AI for Teaching**
| Task # | Task Description (Mobile-First) | Concepts & Outcomes |
|:---:|:---|:---|
| 1 | Watch a 3-min demo of AI creating an analogy for a tough engineering topic. | Exposure, Myth Busting |
| 2 | Open your lecture notes in your phone's gallery. Imagine an AI reading your handwriting. | Mental Scaffolding, Personal Assets |
| 3 | View two AI-generated quiz questions. Select the one you feel is better for your students. | Critical Evaluation, Quality Awareness |
| 4 | Type a chapter name from your textbook. See the AI generate real-world examples. | Guided Prompting, Real-World Application |
| 5 | Take a photo of a paragraph from a book. Watch the AI instantly extract the text. | OCR, Mobile-Native AI |
| 6 | Ask the AI a common student question (e.g., "What are the prerequisites for this course?"). | AI as a Knowledge Base, Basic Interaction |
| 7 | Ask the AI for an interesting "fact of the day" related to your next lecture topic. | Classroom Engagement, Idea Generation |
| 8 | Ask a follow-up to the last task: "Can you make that fact simpler for me?" | Conversational Context, Differentiation |
| 9 | Tell the AI: "I need to make my lectures more interactive." Ask it for one simple idea. | Problem-Solving, AI for Pedagogy |
| 10 | Finish this sentence: "For my teaching, I hope AI can help me with..." | Goal Setting, Personal Mission |

#### **Module 1.2: AI for Administration**
| Task # | Task Description (Mobile-First) | Concepts & Outcomes |
|:---:|:---|:---|
| 1 | Watch a 2-min video showing AI sorting a messy inbox and highlighting urgent emails. | Exposure, Automation Potential |
| 2 | Open your email on your phone. Identify one type of email you wish you didn't have to write. | Pain Point Identification, Admin Burden |
| 3 | View two AI-drafted email replies to a leave request. Choose the one that fits your style. | Understanding Tone, Style Matching |
| 4 | Use a one-button prompt: "Draft a short, polite reminder email to students about a deadline." | Zero-Effort Prompting, Routine Communication |
| 5 | Type the name of a college event (e.g., "Department Symposium"). Ask AI to list 5 tasks to organize it. | AI for Planning, Task Management |
| 6 | Take a photo of a printed circular from a notice board. See the AI extract the text. | Information Capture, Physical to Digital |
| 7 | Ask the AI: "What are the key sections in a 'Minutes of Meeting' document?" | AI for Structure, Document Formatting |
| 8 | Look at the sections from the last task. Ask a follow-up: "Give me an example of a good 'Action Item'." | Follow-up Prompts, Action-Oriented Writing |
| 9 | Ask the AI: "How can AI help with preparing NAAC or NBA documentation?" | AI for Compliance, Major Pain Points |
| 10 | Finish this sentence: "For my admin work, I hope AI can help me with..." | Goal Setting, Focusing on Efficiency |

#### **Module 1.3: AI for Research**
| Task # | Task Description (Mobile-First) | Concepts & Outcomes |
|:---:|:---|:---|
| 1 | Watch a video of a researcher using AI to find relevant papers from a database instantly. | Exposure, AI in Research Workflows |
| 2 | Open a research paper PDF on your phone. Think about how long it takes to summarize it. | Pain Point Identification, Research Bottlenecks |
| 3 | View two AI-generated titles for a research paper. Pick the one that sounds more impactful. | Critical Evaluation, Research Communication |
| 4 | Open a paper and type in its title. Ask AI: "What are the likely keywords for this paper?" | Guided Prompting, Keyword Analysis |
| 5 | Take a photo of the "Conclusion" section of any research paper. Watch the AI extract the text. | Information Extraction, Data Ingestion |
| 6 | Ask the AI a simple question: "What are the recent trends in 'VLSI design'?" | AI as a Knowledge Discovery Tool |
| 7 | Look at the trends from the last task. Ask a follow-up: "Can you explain 'low-power design' simply?" | Simplifying Complexity, Deeper Understanding |
| 8 | Tell the AI: "I need to write a literature review." Ask it: "What are the typical steps?" | AI for Process Guidance, Research Methodology |
| 9 | Ask the AI: "How can AI help me avoid plagiarism in my writing?" | Academic Integrity, Ethical Research |
| 10 | Finish this sentence: "For my research, I hope AI can help me with..." | Goal Setting, Research Ambition |

---
### **Track 2: AI-Explorer**
*Goal: To learn the foundational craft of effective prompting and apply it to simple, daily tasks.*

#### **Module 2.1: AI for Teaching**
| Task # | Task Description (Mobile-First) | Concepts & Outcomes |
|:---:|:---|:---|
| 1 | Open lecture notes. Ask AI: "Acting as a professor, explain [your topic] in three different ways." | Role Prompting, Alternative Explanations |
| 2 | Take a photo of a textbook diagram. Ask AI to generate three quiz questions based on that diagram. | Image-to-Text Analysis, Assessment Generation |
| 3 | Provide a list of 5 topics. Ask AI to create a "2-marks question bank" in a numbered list. | Format Control, Bulk Content Creation |
| 4 | Ask AI to act as a curious student. Explain a concept to it and ask: "What was confusing?" | Role-Playing, Getting Feedback |
| 5 | Upload your course's learning objectives. Ask AI to design an innovative hands-on lab session. | Instructional Design, Outcome-based Planning |
| 6 | Ask AI to write a script for a 1-min video for the student WhatsApp group about the next chapter. | Micro-learning, Student Communication |
| 7 | Provide a student's wrong answer. Ask AI to explain the misconception in a helpful tone. | Feedback Generation, Pedagogy |
| 8 | Give AI a complex term (e.g., 'Heuristic Algorithm'). Ask it for a simple analogy and a metaphor. | Creative Comparison, Simplification |
| 9 | Provide a student list. Ask AI for random lab pairs with the constraint: "A & B cannot be a pair." | Constrained Logic, Data Manipulation |
| 10 | Share the most creative teaching idea you generated using AI this week with your cohort. | Peer Learning, Showcasing Creativity |

#### **Module 2.2: AI for Administration**
| Task # | Task Description (Mobile-First) | Concepts & Outcomes |
|:---:|:---|:---|
| 1 | Open an email asking for an extension. Ask AI to draft a polite but firm reply stating your policy. | Persona-driven Drafting, Policy Communication |
| 2 | Take a photo of an expense list. Ask AI to extract items/amounts, format as a table, and find the total. | Data Extraction from Image, Calculation |
| 3 | You need to schedule a meeting. Provide constraints (people, time). Ask AI to draft a proposal email. | Constraint-based Planning, Scheduling |
| 4 | Take a photo of your handwritten To-Do list. Ask AI to digitize and categorize it. | Handwriting Recognition, Prioritization |
| 5 | Ask AI to write the "Vote of Thanks" speech for a seminar, mentioning key people. | Formal Content Generation, Public Speaking |
| 6 | Provide a list of marks. Ask AI to write encouraging comments for high-scorers and supportive ones for low-scorers. | Conditional Content Generation, Feedback at Scale |
| 7 | Ask AI to create a checklist of all documents needed for faculty promotion applications. | Checklist Generation, Career Progression |
| 8 | Copy a long email chain. Ask AI to summarize the problem, people, and last action item. | Email Thread Summarization, Action Extraction |
| 9 | Ask AI to create a formal agenda for the first meeting of the "Discipline Committee." | Agenda Creation, Formal Meeting Structure |
| 10 | Find a long university circular. Ask AI to simplify it into 5 easy-to-understand bullet points. | Simplifying Jargon, Effective Communication |

#### **Module 2.3: AI for Research**
| Task # | Task Description (Mobile-First) | Concepts & Outcomes |
|:---:|:---|:---|
| 1 | Find a research paper PDF. Copy the abstract. Ask AI to rewrite it for a conference "Call for Papers". | Tone Modification, Audience-Specific Rewriting |
| 2 | Provide your draft "Introduction" section. Ask AI to suggest where to add a stronger problem statement. | AI as a Writing Coach, Structural Feedback |
| 3 | List 3-4 research keywords. Ask AI to generate 10 potential paper titles. | Ideation, Title Generation |
| 4 | Take a photo of a graph from a paper. Ask AI to describe the key trend shown in the image. | Chart-to-Text, Data Interpretation |
| 5 | Ask AI to act as a journal reviewer. Give it your research question and ask for two critical questions. | Pre-submission Review, Critical Self-Evaluation |
| 6 | Writing a grant proposal? Ask AI to write the "Broader Impacts" section for your technical research. | Grant Writing Support, Societal Benefit |
| 7 | Provide a list of references. Ask AI to format them all consistently in APA style. | Formatting Correction, Attention to Detail |
| 8 | Describe your research simply. Ask a web-connected AI to find 3 recent, highly-cited papers. | AI for Literature Search, Staying Current |
| 9 | Ask AI to help you write the "Limitations of the Study" section for your paper. | Critical Thinking, Acknowledging Boundaries |
| 10 | Share the most useful research prompt you created with your cohort and explain how it helped. | Peer Learning, Sharing Research Hacks |

---
### **Track 3: AI-Adopter**
*Goal: To build consistent habits and integrate AI into recurring, multi-step professional workflows.*

#### **Module 3.1: AI for Teaching**
| Task # | Task Description (Mobile-First) | Concepts & Outcomes |
|:---:|:---|:---|
| 1 | Prompt AI to co-create a complete lesson plan: objectives, hook, activities, and summary. | Workflow Integration, End-to-End Creation |
| 2 | Upload a student's project abstract. Ask AI to evaluate it against a 3-point rubric you provide. | AI as an Evaluative Tool, Rubric-based Analysis |
| 3 | Take a photo of a complex circuit diagram. Ask AI to generate a detailed textual explanation of it. | Image Analysis, Visual-to-Textual Translation |
| 4 | Take a photo of a messy whiteboard after a brainstorming session. Ask AI to organize the ideas into themes. | Unstructured Data Synthesis, Idea Clustering |
| 5 | Upload the problem statement for an assignment. Ask AI to generate a step-by-step guide for students. | Scaffolding, Student Support |
| 6 | Open an Excel sheet of student marks. Ask AI to identify students who are "at-risk" based on a rule you provide. | Data Analysis, Proactive Intervention |
| 7 | Describe a lab experiment. Ask AI to generate a list of potential safety hazards and precautions. | Risk Assessment, Safety Planning |
| 8 | Use AI to create a script for a 5-minute educational video, complete with visual cues. | Multimedia Scripting, Content Diversification |
| 9 | Upload your course objectives. Ask AI to map them to Program Outcomes (POs) for NBA documentation. | Compliance Documentation, Mapping |
| 10 | Create a personal "Prompt Library" in your notes app with your top 5 teaching prompts. | Personal Knowledge Management, Habit Formation |

#### **Module 3.2: AI for Administration**
| Task # | Task Description (Mobile-First) | Concepts & Outcomes |
|:---:|:---|:---|
| 1 | Upload a photo of handwritten meeting notes. Ask AI to convert them into formal "Minutes of Meeting". | Handwriting to Formal Document, Workflow Automation |
| 2 | Open your calendar. List your meetings for the week. Ask AI to create a prioritized "preparation list". | Time Management, Personal Productivity |
| 3 | Draft an email to the Principal. Ask AI to refine the tone to be highly formal and respectful. | Advanced Tone & Style Modification |
| 4 | You need to write a report. Use your voice to dictate the key findings. Ask AI to structure it into a formal report. | Voice-to-Text, Report Generation |
| 5 | Upload a list of faculty names and their preferences. Ask AI to create a fair invigilation duty roster. | Constraint Optimization, Complex Scheduling |
| 6 | Ask AI to create a survey to gather student feedback on a course, including different question types. | Survey Design, Feedback Mechanisms |
| 7 | Upload last year's department budget (as a picture or text). Ask AI to highlight the top 3 areas of expenditure. | Financial Data Analysis, Budget Review |
| 8 | You are organizing a national conference. Ask AI to draft a professional "Call for Papers" announcement. | Event Management, Professional Communication |
| 9 | Ask AI to create a project plan (Gantt chart style, in a table) for obtaining NAAC accreditation. | Project Planning, Strategic Documentation |
| 10 | Create a weekly recurring reminder to use AI for at least one administrative task each day. | Habit Reinforcement, Systemizing Use |

#### **Module 3.3: AI for Research**
| Task # | Task Description (Mobile-First) | Concepts & Outcomes |
|:---:|:---|:---|
| 1 | Upload a research paper PDF. Ask AI to extract all tables into a structured format you can copy. | Data Extraction, Document Deconstruction |
| 2 | Take a photo of a complex formula. Ask AI to explain each component of the formula and its role. | Equation Analysis, Deep Comprehension |
| 3 | Provide AI with your raw experiment data (e.g., a list of readings). Ask it to perform a basic statistical analysis (mean, median, std dev). | Statistical Analysis, Data Interpretation |
| 4 | You're stuck in your research. Describe your problem to the AI and ask it to suggest three novel methodologies you could explore. | Ideation, Methodological Expansion |
| 5 | Draft the "Methodology" section of your paper. Ask AI to review it for clarity, completeness, and reproducibility. | Peer Review Simulation, Scientific Rigor |
| 6 | Ask AI to help you write a rebuttal to a reviewer's comments, maintaining a constructive and professional tone. | Rebuttal Writing, Scholarly Communication |
| 7 | Upload your completed paper. Ask AI to generate a 10-slide presentation outline for a conference. | Content Repurposing, Presentation Prep |
| 8 | Use AI to find potential journals for your paper. Give it your abstract and keywords and ask for a list of 5 suitable, indexed journals. | Journal Selection, Publication Strategy |
| 9 | Ask AI to help you write the "Acknowledgements" section, ensuring you thank all relevant parties appropriately. | Professional Etiquette, Finalizing Manuscripts |
| 10 | Schedule a recurring "research hour" in your calendar where you use AI to explore new papers. | Systemizing Research, Habit Formation |

---
### **Track 4: AI-Innovator**
*Goal: To move from using AI to creating custom, solution-oriented AI agents and tools.*

#### **Module 4.1: AI for Teaching**
| Task # | Task Description (Mobile-First) | Concepts & Outcomes |
|:---:|:---|:---|
| 1 | Define a problem: "My first-year students constantly struggle with [specific topic]." | Problem Definition, Solution-Oriented Thinking |
| 2 | Gather 3-4 key documents (notes, textbook chapters) about this topic to serve as a Knowledge Base. | Knowledge Base Curation, Data Prep |
| 3 | Create your first Custom Agent: "The [Topic] Tutor Bot". Upload the knowledge and give it its persona. | Custom Agent Creation, System Prompting |
| 4 | Test your Tutor Bot. Ask it a question you know is in the documents, and one you know isn't. | Testing and Validation, Guardrails |
| 5 | Refine your Tutor Bot's instructions: "Always ask the student a question back to check their understanding." | Iterative Refinement, Interactive Pedagogy |
| 6 | Design a more complex agent: A "Lab Assistant Bot" that can answer safety questions and explain procedures. | Advanced Solution Design |
| 7 | Create an AI workflow: Use AI to generate a case study, then feed that case study to another AI to create discussion questions. | AI Chaining, Multi-step Workflows |
| 8 | Create a "user guide" for students on how to interact with your Tutor Bot for maximum benefit. | User Experience (UX), Documentation |
| 9 | Design an assignment where students must use your Tutor Bot to find answers and cite their interaction. | AI-native Assessment Design |
| 10 | Prepare a 2-minute pitch for your Tutor Bot, explaining how it will improve student pass rates. | Solution Pitching, Value Proposition |

#### **Module 4.2: AI for Administration**
| Task # | Task Description (Mobile-First) | Concepts & Outcomes |
|:---:|:---|:---|
| 1 | Define a problem: "Faculty waste hours answering the same questions about department policies." | Problem Definition for Admin Solutions |
| 2 | Gather the relevant documents: Department handbook, circulars about policies, etc. | Admin Knowledge Base Curation |
| 3 | Create a "Department Policy FAQ Bot". Upload the docs and set its persona. | Admin Agent Creation |
| 4 | Test the FAQ Bot with common and edge-case questions about policies. | Robustness Testing, Validation |
| 5 | Refine the FAQ Bot: "If you cannot answer, direct the user to email the Head of Department at [email]." | Fallback Mechanisms, Error Handling |
| 6 | Design an "Event Coordinator Bot" that can answer questions about an upcoming symposium. | Event Management Automation |
| 7 | Create a workflow: Upload a photo of a filled-out leave form, have AI extract the data, and then draft an approval email. | OCR to Action, Full Workflow Automation |
| 8 | Create a simple UI mockup (on paper) of how faculty would interact with your FAQ Bot in an app. | UI/UX Prototyping |
| 9 | Write the "Help" section for your FAQ bot. | User Support, Documentation |
| 10 | Pitch your FAQ Bot to your cohort, focusing on the number of man-hours it would save per month. | ROI Calculation, Efficiency Pitch |

#### **Module 4.3: AI for Research**
| Task # | Task Description (Mobile-First) | Concepts & Outcomes |
|:---:|:---|:---|
| 1 | Define a problem: "It takes too long for new PhD scholars to get up to speed on our lab's past work." | Research Problem Definition |
| 2 | Gather the knowledge base: 5-10 abstracts of papers published by your lab in the last 3 years. | Specialized Knowledge Base Curation |
| 3 | Create a "Lab Research Assistant Bot". Upload the abstracts and set its instructions. | Research Agent Creation |
| 4 | Test the bot: Ask it "Which paper deals with [specific method]?" | Content-based Querying |
| 5 | Refine the bot: "Always provide the title and year of the paper when answering." | Precise Output Formatting |
| 6 | Design a "Grant Proposal Helper Bot" that is fed with successful past proposals from your college. | Pattern Recognition, Advanced Tool Design |
| 7 | Create a workflow: Use AI to summarize a paper, then feed the summary to another prompt to generate a tweet about the findings. | AI for Social Media Outreach (Research Comms) |
| 8 | Design the ideal "input form" for your Research Assistant Bot. What info would a user need to provide? | Input Design, User-centric Tools |
| 9 | Create a video walkthrough on your phone screen, showing how to use your bot. | Screen Recording, Demo Creation |
| 10 | Pitch your Research Assistant Bot, focusing on how it can accelerate research and increase publication rates. | Pitching for Innovation, Impact Focus |

---
### **Track 5: AI-Catalyst**
*Goal: To scale impact by leading AI adoption, mentoring others, and driving strategic change.*

#### **Module 5.1: AI for Teaching**
| Task # | Task Description (Mobile-First) | Concepts & Outcomes |
|:---:|:---|:---|
| 1 | Evaluate a new AI-based educational app. Write a review for your colleagues on its pros, cons, and pedagogical fit. | AI Tool Evaluation, Technology Scouting |
| 2 | Create a "Best Practices for AI in the Classroom" one-page guide for your department. | Knowledge Dissemination, Best Practices |
| 3 | Design an innovative assignment that requires students to "debate" an AI on a technical topic. | AI-native Pedagogy, Critical Thinking |
| 4 | Draft a clear "Policy on Use of AI for Final Year Projects," including guidelines on citation. | Ethical Frameworks, Academic Integrity |
| 5 | Prepare materials (slides, task) for a 30-min mini-workshop to help "AI-Curious" colleagues. | Mentorship, Training Material Design |
| 6 | Record a 5-minute segment of the workshop on your phone, explaining a core concept clearly. | Asynchronous Training, Communication |
| 7 | Analyze your course curriculum. Identify 3 modules where AI integration could lead to a 20% improvement in student understanding. | Curriculum Analysis, Strategic Integration |
| 8 | Create a business case for a department-wide subscription to an advanced AI educational tool. | Business Case Development, ROI |
| 9 | Draft a charter for a "Teaching with AI" community of practice within the college. | Community Building, Sustained Adoption |
| 10 | Write a "Vision 2026" memo for the Dean of Academics on making the college a leader in AI-integrated teaching. | Strategic Vision, Thought Leadership |

#### **Module 5.2: AI for Administration**
| Task # | Task Description (Mobile-First) | Concepts & Outcomes |
|:---:|:---|:---|
| 1 | Research 3 different AI tools for automating administrative tasks. Write a comparative analysis. | Comparative Tool Analysis, Tech Evaluation |
| 2 | Create a "Quick Start Guide" for your department on using AI for email management. | Peer Support, Documentation |
| 3 | Design a new, AI-streamlined workflow for the entire student leave application and approval process. | Workflow Re-engineering, Process Optimization |
| 4 | Draft a college-wide "Acceptable Use Policy" for using AI with sensitive administrative data. | Data Governance, Policy Making |
| 5 | Mentor a junior colleague. Sit with them and help them build their first administrative AI prompt. | One-on-One Mentorship, Skill Transfer |
| 6 | Host a 30-minute "Admin Hacks" session for your department, showcasing 3 AI-powered shortcuts. | Peer Training, Showcasing Value |
| 7 | Map out the entire faculty promotion application process. Identify the top 3 bottlenecks that AI could solve. | Process Mapping, Bottleneck Analysis |
| 8 | Calculate the potential ROI (in hours saved per faculty per year) of automating department-level report generation. | ROI Calculation for Admin, Business Case |
| 9 | Launch the "AI for Admin Efficiency" interest group on the college's internal communication platform. | Grassroots Community Building |
| 10 | Write a formal proposal to the Registrar on a pilot project to use AI for streamlining admissions paperwork. | Pilot Project Proposal, Driving Change |

#### **Module 5.3: AI for Research**
| Task # | Task Description (Mobile-First) | Concepts & Outcomes |
|:---:|:---|:---|
| 1 | Compare two AI-powered research assistant tools (like Elicit, Scite). Recommend one for your department. | Comparative Analysis, Research Infrastructure |
| 2 | Create an "AI for Literature Review" flowchart to guide new PhD scholars. | Process Documentation, Mentoring Researchers |
| 3 | Design a seminar series on "The Future of AI in [Your Engineering Field]". | Curriculum Design for Peers, Leadership |
| 4 | Draft a departmental policy on the ethics of co-authorship with AI in research publications. | Research Ethics, Policy Leadership |
| 5 | Mentor a PhD student by helping them use AI to find gaps in current research for their thesis proposal. | High-level Mentorship, Research Direction |
| 6 | Organize and lead a "Journal Club" session where you use AI to summarize and critique a new paper. | Leading Scholarly Discussion, AI-assisted Critique |
| 7 | Analyze your department's research output for the last 5 years. Use AI to identify thematic clusters and areas for potential collaboration. | Strategic Research Analysis, Data-driven Insights |
| 8 | Write a grant proposal for a project to build a specialized AI tool for your lab, justifying the need and impact. | Grant Writing for Tech Development |
| 9 | Create a "Community of Practice" for AI in research, inviting faculty from other departments to join. | Interdisciplinary Collaboration, Community Leadership |
| 10 | Write a white paper on a vision for how AI can transform engineering research at the university level. | Thought Leadership, Vision Setting |
