# OreGlow — Multi-channel AI Agent (n8n Workflow)

The n8n backend for OreGlow Skincare's AI customer support agent. One workflow handles customer messages from **Website, Email and WhatsApp**, remembers each customer across channels, answers from a knowledge base, and escalates to a human when needed.

🔗 **Live website:** https://oreglow-website.vercel.app
🎥 **Demo video:** https://www.loom.com/share/7727fae0b5734c138df59a11338bd9c2
💻 **Website repo:** https://github.com/Ziko67890/oreglow-website

## How it works
Customer Message (Website / Email / WhatsApp)
↓
Extract & Standardize Info
↓
Search / Create Customer Profile (Supabase)
↓
Fetch Knowledge Base (Products / FAQs / Policies)
↓
Fetch Conversation History
↓
AI Brain (OpenAI GPT-4o-mini)
↓
Detect Intent + Generate Response
↓
Escalation Check
↓
Route Response to Correct Channel
↓
Update CRM + Conversation Log


## Key features
- **Cross-channel memory** — one customer profile across Website, Email and WhatsApp
- **Intent detection** — 8 intents classified automatically
- **Knowledge base grounding** — answers come from real product, FAQ and policy data
- **Smart escalation** — a human is notified for serious issues
- **Channel formatting** — reply style adapts to each channel
- **CRM logging** — every interaction is saved to Supabase

## Tech stack
n8n · OpenAI GPT-4o-mini · Supabase · Gmail · WhatsApp · Railway · Postman

## Workflow
<img width="960" height="436" alt="Screenshot 2026-10-05 064344" src="https://github.com/user-attachments/assets/d0ce901d-d1b4-42ef-a416-9911581d77bb" />
<img width="960" height="444" alt="Screenshot 2026-10-05 071858" src="https://github.com/user-attachments/assets/c124a686-67b4-48bc-ae17-b0f058784179" />
<img width="960" height="437" alt="Screenshot 2026-10-05 074007" src="https://github.com/user-attachments/assets/2d0450f1-42d5-4096-b159-08270e517160" />
<img width="960" height="436" alt="Screenshot 2026-10-05 073944" src="https://github.com/user-attachments/assets/5b391641-d800-46ea-9232-d4362f9f4c26" />

## Import it into your own n8n
1. Download `multi-ai-channel.json` from this repo
2. In n8n, create a new workflow, click **⋯ → Import from File** and select the JSON
3. Add your own credentials: OpenAI, Supabase, Gmail and WhatsApp
4. Set up the Supabase tables the workflow reads from and writes to
5. Activate the workflow

## Results
- 30 test scenarios completed successfully
- 3 channels fully automated
- Escalation working across all 3 channels

## Built as part of
Big Brains Learning AI Automation Internship — 30 days, 10 phases, completed October 2026.



