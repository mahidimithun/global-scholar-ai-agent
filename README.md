# GlobalScholar: Grounded AI Concierge for Affordable Study Abroad

## 📝 About the Project
GlobalScholar is an intelligent, autonomous relocation concierge designed to eliminate the stress and guesswork of international university planning. For many students, researching higher education options requires manually scraping hundreds of disparate university websites just to track fluid tuition rates, local rental indices, and regional living costs.

GlobalScholar addresses this challenge directly by utilizing the production-ready `google-genai` SDK paired with the high-speed `gemini-2.5-flash` model. By incorporating **Native Google Search Grounding**, the agent completely bypasses static knowledge cutoff limitations. It functions as an autonomous query planner that parses a student's unstructured profile parameters, generates highly optimized live search queries, and synthesizes real-world data into cohesive, custom budget blueprints and relocation timelines.

---

## 🏗️ System Architecture

GlobalScholar uses a streamlined, factual feedback-driven agent pipeline that strictly enforces data correctness by verifying live web facts before generating the user's report interface:
### 🧠 Architectural Components Breakdown
1. **User Interaction Layer (`Standard Input`):** Captures unstructured input strings containing the student's background, desired major, and target destination parameters.
2. **Agent Intelligence Center (`gemini-2.5-flash`):** Evaluates user criteria against rigid, hardcoded system instructions that prevent conversational hallucinations and mandate structured layout rules.
3. **Grounding Router (`types.GoogleSearch()`):** The functional tool framework allows the agent to dynamically decide exactly what missing facts it needs to pull and execute those target strings live via Google.
4. **Context Synthesis & Presentation Layer:** Merges retrieved live factual data payloads with layout constraints to display a clean, scannable **Cost Matrix** alongside an itemized **Pre-Departure Checklist**.

---

## ⚙️ How It Works

GlobalScholar runs as a highly focused, interactive loop in four distinct steps:

### Step 1: Profile Initialization
When executed, the program establishes an authenticated instance via the official `genai.Client()`. It holds execution at the command line or within the Google Colab runtime interface using an interactive prompt:
```text
👉 Enter your relocation inquiry (e.g., My degree is CSE, show me cheap options...)
