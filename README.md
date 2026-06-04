# 🤖 Finance Content AI Agent Team
> A fully autonomous 4-agent AI pipeline that researches real Instagram + YouTube trends and writes viral Indian finance scripts — powered by Gemini 2.0 Flash + Groq Llama 3.3 70B

![n8n](https://img.shields.io/badge/n8n-EA4B71?style=for-the-badge&logo=n8n&logoColor=white)
![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)
![Google Gemini](https://img.shields.io/badge/Gemini_2.0_Flash-4285F4?style=for-the-badge&logo=google&logoColor=white)
![Groq](https://img.shields.io/badge/Groq_Llama_3.3-F55036?style=for-the-badge&logo=groq&logoColor=white)

---

## 🎯 What It Does

Type any finance topic in chat → the system automatically:

1. 🔍 **Researches** real Instagram posts from @pranjal.kamra, @warikoo, @sharan_hegde
2. 📺 **Fetches** trending YouTube finance videos with view counts
3. 🧠 **Finds** content gaps competitors have NOT covered yet
4. ✍️ **Writes** 3 full 40-second scripts with Indian context and Hinglish CTAs
5. 📊 **Scores** every script using Meta's TRIBE v2 virality framework
6. ✨ **Refines** scripts fixing every weakness identified
7. 💾 **Saves** full report to `finance_scripts.txt` automatically

**Zero human intervention. One chat message. Full output.**

---

## 🏗️ Architecture

```
Chat Input (topic)
       ↓
Setup Input
       ↓
Search Instagram → Search Google Trends → Search YouTube
                         ↓
                   Merge Research
                         ↓
       Agent 1 — Strategy (Gemini 2.0 Flash via OpenRouter)
       Output: Top 5 content ideas + content gaps
                         ↓
       Agent 2 — Script Writer (Groq Llama 3.3 70B)
       Output: 3 full 40-second scripts with dual CTAs
                         ↓
       Agent 3 — Analyst (Groq Llama 3.3 70B)
       Output: Standard /50 + TRIBE v2 /50 + virality prediction
                         ↓
       Agent 4 — Refiner (Groq Llama 3.3 70B)
       Output: Final polished production-ready scripts
                         ↓
                finance_scripts.txt ✅
```

---

## 🤖 The 4 Agents

| Agent | Role | Model | Output |
|---|---|---|---|
| Agent 1 | Strategy | Gemini 2.0 Flash (OpenRouter) | Top 5 ideas + content gaps |
| Agent 2 | Script Writer | Groq Llama 3.3 70B | 3 full 40-sec scripts |
| Agent 3 | Analyst | Groq Llama 3.3 70B | TRIBE v2 scores + virality prediction |
| Agent 4 | Refiner | Groq Llama 3.3 70B | Final polished scripts |

---

## 📊 TRIBE v2 Virality Framework

Agent 3 scores every script using Meta's TRIBE v2 model:

| Letter | Criteria | What it measures |
|---|---|---|
| T | Trigger | Does hook stop scroll in 3 seconds? |
| R | Relevance | Is this timely for Indian audience right now? |
| I | Information Gap | Does it create curiosity to watch till end? |
| B | Benefit | What does viewer gain from watching? |
| E | Emotion | Does it trigger fear, hope, anger, or surprise? |

Scripts scoring **45+/50** = predicted **VIRAL** 🔥

---

## 📝 Sample Output

**Topic:** How banks legally steal from you every month

**Best Script (TRIBE Score: 46/50 — STRONG 🔥)**

```
Hook: ₹50,000 salary. ₹40,000 EMI. Phas gaye?

Body:
EMI = karza trap
Budgeting = azadi
Needs over wants always.
PPF = safe investing yaar.

Instagram CT: Comment EMI if this hit different yaar.
YouTube CTA: Subscribe to never get trapped again.
```

---

## 🛠️ Tech Stack

| Tool | Purpose | Cost |
|---|---|---|
| n8n self-hosted | Workflow automation | Free |
| Gemini 2.0 Flash | Agent 1 via OpenRouter | Free tier |
| Groq Llama 3.3 70B | Agents 2, 3, 4 | Free tier |
| Tavily Search API | Instagram + YouTube research | Free tier |

**Total cost: $0** 💰

---

## 🚀 Quick Setup

### 1. Get Free API Keys
- Groq → [console.groq.com](https://console.groq.com)
- OpenRouter → [openrouter.ai](https://openrouter.ai)
- Tavily → [tavily.com](https://tavily.com)

### 2. Import Workflow
```
n8n → Import → Finance_Content_AI_agent_team.json
```

### 3. Add Your Keys
```javascript
const groqKey = 'your_groq_key';
const openrouterKey = 'your_openrouter_key';
```

### 4. Create Output Folder
```bash
mkdir C:\Scripts
```

### 5. Run It
```
Open chat → type finance topic → get full report!
```

---

## 📈 TRIBE Scores Across Test Runs

| Topic | Best TRIBE Score | Virality |
|---|---|---|
| Why people are broke in 30s | 38/50 | Average |
| How 9-5 keeps you poor | 44/50 | Strong |
| Indian EMI trap | 45/50 | Strong 🔥 |
| Banks legally stealing | 43/50 | Strong |
| Insurance scams India | 46/50 | Strong 🔥 |

---

## 🇮🇳 Indian Context Features

- ✅ INR amounts not dollars
- ✅ Real Indian products: EMI, SIP, PPF, FD, Zerodha, Groww
- ✅ Indian salary ranges: 30k/month, 8LPA, 1 crore
- ✅ Indian cities: Mumbai rent, Bangalore IT jobs
- ✅ Hinglish naturally: yaar, bhai, sach mein, phas gaye
- ✅ Top creators referenced: @pranjal.kamra, @warikoo, @sharan_hegde

---

## 🔮 Paid Upgrade Path

| Current Free | Paid Upgrade |
|---|---|
| Groq rate limits | Claude 3.5 Sonnet — no limits |
| Gemini free quota | Gemini 1.5 Pro — deeper research |
| Tavily 1000/month | Unlimited real-time research |
| 2 min pipeline | Under 30 seconds |

---

## 📜 License

MIT — free to use and modify

---

*Built  by [Sai Pattnaik](https://github.com/saipattnaik24cse-alt) · B.Tech CSE @ BML Munjal University · *
