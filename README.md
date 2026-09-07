# n8n
Web Lead Spam Checker
# 🚀 Web Lead Spam Checker (AI Automation with n8n)

This project demonstrates how **low‑code automation** combined with **AI classification** can streamline lead management, reduce manual effort, and improve productivity.  
Built using **n8n**, **OpenAI API**, and **Google Sheets**, the workflow automatically filters spam leads and routes genuine enquiries for review.

---

## 📌 Project Overview
- **Goal**: Automate spam filtering for website leads.  
- **Outcome**: Reduced manual validation, improved accuracy, and faster lead management.  
- **Approach**: Integrated OpenAI’s GPT model with n8n to classify leads, then routed results into Google Sheets.

---

## 🔑 Key Steps in Setup
1. **OpenAI API key** — obtained from [platform.openai.com](https://platform.openai.com) to enable intelligent text classification.  
2. **Google Cloud Console credentials** — created Client ID and Client Secret for secure Sheets access.  
3. **Enable Google Drive API** — Sheets access requires Drive permissions; missing this caused initial errors.  
4. **OAuth consent screen** — configured to meet Google’s strict authentication rules.  
5. **Workflow design in n8n** — integrated OpenAI for spam detection, routed clean leads into Sheets, flagged suspicious entries for review.

---

## ⚡ Challenges Faced
- **Authentication hurdles**: Missing Drive permissions blocked Sheets access until corrected.  
- **Strict API rules**: OAuth consent screen setup was mandatory to avoid credential rejection.  
- **Local vs Cloud setup**: Running n8n locally required Node.js/Docker knowledge, while cloud hosting offered convenience but less control.  
- **Cost considerations**: Leveraged OpenAI’s $5 free API credit to test workflows without upfront cost.  

---

## 🖥️ Extended Project Details
### Core Workflow
- **Form Trigger**: Captures enquiries (Name, Email, Company, Project Brief).  
- **IF Node**: Blocks empty project briefs.  
- **OpenAI Spam Classification**: GPT‑4.1 Mini model returns simple `yes` (spam) or `no` (genuine).  
- **Switch Node**: Routes results into separate Google Sheets tabs: *Genuine* and *Spam*.  

### Desktop Installation Option
- n8n can run locally using **Node.js** or **Docker**.  
- Benefits: full control, enhanced privacy, zero subscription cost.  
- Suitable for organizations with strict compliance or budget constraints.  

### Cloud vs Local
- **Cloud hosting**: Convenience and scalability.  
- **Local installation**: Ensures workflows and data remain on the user’s machine.  

### OpenAI API Credit
- New users receive **$5 free credits** on signup.  
- Enables experimentation with AI classification at no cost.  
- Ideal for proof‑of‑concept projects before scaling.  

---

## 📊 Value Proposition
- **Cost‑effective automation**: Local n8n + free API credits reduce expenses.  
- **Scalable design**: Workflow can expand to include agents that decide which Sheets tool to use.  
- **Practical application**: Real‑world use case of filtering spam vs genuine leads, improving productivity and data quality.  

---

## 📢 Research & Learnings
This project highlights the **intersection of AI and low‑code automation**:
- AI models can be embedded into workflows for real‑time decision making.  
- Low‑code tools like n8n reduce development overhead while maintaining flexibility.  
- Free API credits and local installation options lower the barrier to entry, making experimentation accessible to individuals and small teams.  

---

## 🏷️ Tags
`AI Automation` `n8n` `OpenAI` `Google Sheets` `Spam Filtering` `Workflow Automation` `Low Code`
