# 🦚 Saarthi - Your Own Charioteer AI

**Kaggle 5-Day AI Agents Intensive Capstone | Concierge Agents Track**

[![Demonstration Video](https://img.shields.io/badge/YouTube-Watch_Video-FF0000?style=for-the-badge&logo=youtube&logoColor=white)](INSERT_YOUR_YOUTUBE_LINK_HERE)

## 📖 Project Overview
Modern life is filled with invisible battles: burnout, severe stress, and career anxiety. In the epic Mahabharata, when Arjuna was overwhelmed on the battlefield, Lord Shri Krishna stepped in as his *Saarthi* (Charioteer)—not to fight the war for him, but to provide the philosophical clarity needed to proceed. 

**Saarthi AI** is a stateful, context-engineered philosophical guide built to be that steadfast companion for modern seekers. Operating under the **Concierge Agents Track**, it processes complex emotional dilemmas and delivers wisdom from the *Bhagavad Gita*. Crucially, it operates within a strict zero-trust perimeter, ensuring absolute data privacy and strictly refusing to make unauthorized medical or clinical inferences.

*(Insert your UI screenshot here by dragging and dropping the image file into the GitHub editor)*
![Saarthi UI](INSERT_IMAGE_LINK_HERE)

---

## ⚙️ Technical Architecture (Agentic Engineering)
This project abandons casual, unstructured "vibe coding" in favor of strict, production-grade **Agentic Engineering**[cite: 1]. It perfectly implements the core paradigm: `Agent = Model + Harness`[cite: 1].

The architecture is divided into 7 distinct biological metaphors to make the engineering accessible:

### 1. The Soul (Zero-Trust Identity)
We utilize secure secrets management (Google Colab Secrets) to establish LLM identity. This prevents unauthorized ambient access and mitigates the Confused Deputy problem by never hardcoding API keys in the execution environment[cite: 4].

### 2. The DNA (Spec-Driven Development)
To eliminate prompt ambiguity and the reasoning "format tax", the agent is guided by an absolute architectural North Star[cite: 5]. It utilizes a hybrid format: **Behavior-Driven Development (BDD)** specifications written in Gherkin syntax for narrative goals, alongside flat YAML blocks for tool configurations[cite: 5].

### 3. The Shield (Context Hygiene & Semantic Firewall)
Autonomous agents are prone to "Context Hallucination" and data leaks[cite: 5]. Saarthi implements a strict Context Hygiene middleware[cite: 5]. Regular expressions intercept execution turns to dynamically scrub Personally Identifiable Information (PII)[cite: 5]. Furthermore, a zero-tolerance Semantic Firewall actively blocks unprompted medical/clinical terminology, enforcing the Concierge Track's safety mandate[cite: 4, 5].

### 4. The Brain (Asynchronous Memory ETL Loop)
To mitigate "context rot" and lower OpEx token burn over long conversations, the architecture strictly separates the chronological **Session** log from persistent **Memory**[cite: 3]. An asynchronous ETL (Extract, Transform, Load) loop runs in the background to distill noisy chat history into a stable, consolidated philosophical anchor (e.g., *Dharma* or *Karma-Yoga*)[cite: 3].

### 5. The Face (A2UI v0.9 Standard)
The agent does not emit raw text blocks or risky executable frontend code. Instead, it utilizes the **Agent-to-User Interface (A2UI v0.9)** standard[cite: 2]. It safely outputs a framework-agnostic flat adjacency list of layout components (like `Column`, `Card`, and `TextField`)[cite: 2]. A native Javascript-to-Python bridge renders these JSON blueprints into beautiful, interactive HTML widgets dynamically.

### 6. The Conscience (Glass Box Trajectory Evaluation)
We do not rely on binary success metrics. A Glass Box Trajectory Evaluator simulates an **LLM-as-Judge** to score the agent's internal reasoning path[cite: 4]. It verifies that the agent successfully triggered background memory tools and emitted valid A2UI schemas, continuously measuring for Intent Drift against rubrics derived directly from the user's opening prompt[cite: 4].

---

## 🚀 How to Run Locally

1. Open the `Saarthi_Your_Own_Charioteer_AI.ipynb` file in Google Colab.
2. Click on the 🔑 **Secrets** tab on the left sidebar.
3. Add a new secret named `GEMINI_API_KEY` and paste your Google Gemini API key. Ensure the "Notebook access" toggle is turned on.
4. Go to the top menu and select `Runtime > Run all`.
5. Scroll to the bottom cell to interact with Saarthi's live Canvas interface!

---
*Built for the 2026 Kaggle 5-Day AI Agents Intensive with Google.*
