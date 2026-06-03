# QA Portfolio
# Software Quality Assurance Portfolio

Welcome to my QA Testing Portfolio. I am a detail-oriented Manual QA Tester focused on ensuring seamless user experiences, robust functionality, and high performance across web and mobile platforms. 

This repository showcases my practical experience in comprehensive test documentation, exploratory testing, and rigorous bug reporting, with a strong specialized focus on **AI-integrated systems**, **complex e-commerce logic**, and **mobile app environments**.

---

## 🛠️ Tools & Technologies
* **Testing Methodologies:** Functional, UI/UX, Exploratory, Integration, End-to-End (E2E), Boundary Value Analysis, Compatibility, Interrupt, and API Testing
* **Project & Bug Management:** Jira, ClickUp, Notion, Git/GitHub
* **Technical QA Tools:** Postman (API Validation), Chrome DevTools, Jam.dev (Session Capturing)
* **Testing Hardware & OS:** macOS (MacBook Air), iOS (iPhone 13 native environment), Android emulation, Cross-Browser Staging (Chrome, Safari, Firefox)

---

## 📁 Featured Projects (Anonymized under NDA)

### 1. Project Alpha – AI-Augmented Enterprise Writing & Workspace Studio (Web Application)
**Project Description:** A next-generation, cloud-based digital workspace built for technical writers, content creators, and researchers. The ecosystem features advanced text editors, local/cloud research repositories, and multi-tier AI integrations for real-time semantic analysis, outline generation, and automated structural research.

* **QA Focus & Core Competencies:**
  * **AI Non-Deterministic Behavior Testing:** Validating system resiliency and state preservation when complex large-language model (LLM) prompts fail. Specifically tested and isolated critical edge cases where an initial prompt request triggers backend generation timeouts/errors, ensuring the front-end gracefully recovers instead of freezing or rendering broken empty states.
  * **State & Synchronization Management:** Verifying real-time cloud auto-save mechanisms, rich-text formatting boundaries, and data persistence during concurrent document operations.
  * **Asynchronous Integration:** Assessing how background AI research agents fetch and summarize data without degrading the core text editor's client-side performance.


---

### 2. Project Beta – Holistic Emotional Wellness & Behavioral Tracking Ecosystem (Native Mobile Application)
**Project Description:** A highly personalized, secure mobile platform engineered for mental health tracking, pattern analysis, and emotional wellness optimization. The app features localized lifestyle tracking, rich multimedia guided sessions, data encryption protocols, and interactive community networks.

* **QA Focus & Core Competencies:**
  * **Mobile Hardware & Interrupt Testing:** Extensively tested on native iOS hardware (iPhone 13) to monitor app behavior during critical operational disruptions, including sudden voice calls, background state suspension, swift transitions between Cellular (4G/5G) and Wi-Fi networks, and low-battery background throttling.
  * **UI/UX & Accessibility Compliance:** Validating visual responsiveness, multi-touch gestures, and cross-device scaling across diverse high-resolution viewports.
 

---

## 3. Project Gamma – AI-Conversational E-Commerce & B2C Retail Platform (Web Platform)
**Project Description:** A high-traffic consumer e-commerce ecosystem integrating an intelligent conversational AI chatbot that manages end-to-end customer workflows—from product personalization and direct-to-cart query execution to automated inventory updates and customer care management.

* **QA Focus & Core Competencies:**
  * **Advanced Search & SKU Identification Validation:** Deep-dive exploratory testing of the main search infrastructure. Isolated system faults regarding alphanumeric handling, exact and partial string matches, and technical bugs where the engine failed to map correct model numbers and specific SKU configurations to live product databases.
  * **Chatbot-to-Database Integration:** Verifying end-to-end data integrity when the AI agent mutates user baskets, ensuring live catalog syncing, cart persistence, and preventing asynchronous UI lockups during heavy API payloads.
  * **Transactional Resiliency:** Simulating sudden network drops, browser session refreshes, and API timeout scenarios during critical phases of the checkout pipeline and payment gateway responses.


---

## 🐛 Standardized Bug Reporting Framework
To maintain maximum engineering efficiency, every defect logged within this portfolio adheres to strict industry-standard QA lifecycles:
* **Defect Title:** Concise, component-isolated, and high-level summary.
* **Defect Metadata:** Explicit environment variables (Hardware, OS build, Browser version, Staging URL).
* **Reproduction Steps:** Unambiguous, sequential steps designed to minimize reproduction time.
* **Expected vs. Actual Outcome:** Clear technical delta backed by network payloads, console stack traces (via DevTools), or visual session logs (via Jam.dev).

---
📫 **Connect with me:** [LinkedIn](www.linkedin.com/in/anna-bagbaia-1824747b) | 
