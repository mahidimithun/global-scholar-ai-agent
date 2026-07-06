
# GlobalScholar: Grounded AI Concierge for Affordable Study Abroad

## 📝 About the Project
GlobalScholar is an intelligent, autonomous relocation concierge designed to eliminate the stress and guesswork of international university planning. For many students, researching higher education options requires manually scraping hundreds of disparate university websites just to track fluid tuition rates, local rental indices, and regional living costs.

GlobalScholar addresses this challenge directly by utilizing the production-ready `google-genai` SDK paired with the high-speed `gemini-2.5-flash` model. By incorporating **Native Google Search Grounding**, the agent completely bypasses static knowledge cutoff limitations. It functions as an autonomous query planner that parses a student's unstructured profile parameters, generates highly optimized live search queries, and synthesizes real-world data into cohesive, custom budget blueprints and relocation timelines.

---

## 🏗️ System Architecture

<img width="582" height="307" alt="diagram" src="https://github.com/user-attachments/assets/3993b3e6-c209-4fe5-8fae-8aed67fa67e8" />

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
👉 Enter your relocation inquiry (e.g., My degree is CSE, show me cheap options...) 

## ⚙️ Output:

<img width="1892" height="897" alt="ai1" src="https://github.com/user-attachments/assets/94c66fea-84c7-493f-9d1f-4f9aad1f3f6d" />
<img width="1891" height="562" alt="ai2" src="https://github.com/user-attachments/assets/6a04f1b8-ab48-4d62-94f5-efe842b67a60" />
<img width="1912" height="692" alt="ai3" src="https://github.com/user-attachments/assets/561b2e06-294c-4e44-815d-da026a52351a" />
<img width="1781" height="242" alt="ai4" src="https://github.com/user-attachments/assets/c331f571-fcde-4eeb-ada6-b842f2bb6d89" />

