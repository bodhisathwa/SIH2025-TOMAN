# SIH2025-TOMAN

🌿 Ojas Health Aid (MedTrack on WhatsApp)
AI-driven multilingual public health companion for preventive care, disease awareness, and vaccination guidance.

Ojas Hero Banner

🧾 Brief Overview
Ojas Health Aid is an AI-powered chatbot tailored for rural and semi-urban communities. It delivers safe, empathetic, and multilingual counseling on preventive healthcare, emerging outbreaks, vaccination schedules, and lifestyle awareness. The platform integrates with government health systems to surface real-time alerts while nurturing community health literacy across WhatsApp, SMS, and web channels.

🤔 Why Ojas / MedTrack?
🌍 Community-Centric – Designed for India’s linguistic and cultural diversity.
⚕️ Safety-First Guidance – Encourages professional medical care, never self-diagnosis.
📡 Real-Time Intelligence – Syncs with government datasets for outbreak and vaccination updates.
📈 Impact-Driven Goals – Targets 80% query accuracy and 20% awareness growth in key communities.
✨ Key Features
| Icon | Capability | Description | |------|------------|-------------| | 🗣️ | Multilingual Conversations | Converses across major Indian languages with empathetic tone. | | 🩺 | Preventive Health Guidance | Shares symptom education, vaccine reminders, and lifestyle tips. | | 🧭 | Smart Intake & Triage | Progressive questioning to assess severity and recommend next steps. | | 🚨 | Emergency Protocols | Detects critical symptoms and suggests nearby emergency services. | | 🔗 | Government API Integrations | Pulls verified vaccination schedules and outbreak alerts. | | 🧠 | Safety Guardrails | Uses sanitized, ethics-aligned responses with moderation filters. | | 🖼️ | Media & Education Hub | Hosts infographics, field guides, and community outreach assets. | | 📊 | Insights & Reporting | Tracks awareness metrics and user engagement for impact evaluation. |

🛠️ Tech Stack
💻 Frontend
React 18 with TypeScript
Vite build tooling
Tailwind CSS, shadcn/ui, Radix UI
React Router DOM, React Hook Form + Zod
Framer Motion animations
TanStack Query for data fetching
Recharts for analytics dashboards
React Markdown with remark-gfm
🧠 AI & Intelligence Layer
Google Gemini 2.5 Flash (Lite + Full variants)
AI Router for intent classification and model selection
Health Intake, Text Analysis, and Search services
Safety prompts, content sanitization filters, memory manager
☁️ Backend & Infrastructure
Firebase Authentication, Firestore, Cloud Storage
Express development bot, Firebase Hosting
Google Custom Search API integration
Text-to-Speech services for voice responses
🧰 Tooling & DevOps
TypeScript 5.8
ESLint 9
npm / bun workflows
Smoke tests via tsx
Detailed architecture docs in design.md
🏗️ Architecture Snapshot
System interactions flow from conversational channels through the AI router, which orchestrates model usage, intake workflows, and safety guardrails before responding to the user. Memory and profile stores maintain context while integrations fetch trusted health information.

flowchart TD
    A[User Channels: WhatsApp / SMS / Web] --> B[AIRouter]
    B --> C{Health Query?}
    C -- Yes --> D[Health Intake Engine]
    D --> E[Gemini Full Model + Web Search]
    C -- No --> F[Gemini Lite Model]
    E --> G[Safety & Compliance Layer]
    F --> G
    G --> H[Response Formatter + Sources]
    H --> I[Chat UI / Messaging Channel]
    B --> J[Memory Store + Profile Context]
    J --> B
    E --> K[Government Health APIs]
    G --> L[Awareness Metrics Dashboard]
🔍 Core Components
AI Router – Classifies intent, manages follow-ups, selects AI models.
Health Intake Engine – Generates structured symptom questionnaires.
Safety & Compliance Layer – Enforces medical guardrails and privacy controls.
Memory Store – Syncs user context across sessions (local + cloud).
Government Integrations – Retrieves outbreak alerts, vaccination drives, and facility directories.
👥 Team
🧭 Product Lead – Vision, community partnerships, outcome metrics.
🧠 AI/ML Lead – Model orchestration, safety workflows, search integration.
🎨 Frontend Lead – Multichannel UI, multilingual support, accessibility.
🛡️ Backend & Integrations Engineer – Firebase services, Express API bridges, deployment.
🔐 Compliance Analyst – Medical accuracy checks, HIPAA-aligned data governance.
📢 Outreach & UX Research – Field testing, adoption programs, behavior-change insights.
(Update with actual names and contacts as needed.)

🖼️ Gallery
| Preview | Description | |---------|-------------| |Landing| Landing page highlighting value proposition and key CTAs. | |Chat Flow| Multilingual chat conversation showing symptom intake. | |Emergency| Emergency protocol screen with nearby facility guidance. | |Dashboard| Awareness metrics and community impact dashboard. |

(Replace placeholders with real assets located in docs/gallery/.)

🔗 Useful Links
🌐 Live Demo / Deployment: TBD – add cloud URL or WhatsApp link
🎥 Product Walkthrough Video: TBD – link to recorded demo
📄 Architecture & Workflow: design.md
📋 Project Tracker: TBD – Notion / Jira / Trello board
📣 Community Awareness Kit: TBD – content repository link
🎯 Expected Outcomes
Achieve 80% accuracy on health queries through Gemini models and curated datasets.
Deliver 20% awareness uplift in target communities via outreach campaigns.
Provide real-time outbreak alerts and vaccination schedule reminders backed by government data.
Uphold privacy and safety compliance with stringent guardrails and audit trails.
📡 Future Enhancements
Expand voice and dialect-specific support for low-literacy users.
Automate vaccination reminders and appointment booking workflows.
Add offline-first tooling for areas with limited connectivity.
Grow specialist referral networks and continuous medical content updates.


