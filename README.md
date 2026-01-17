# 🇨🇦 Custom Canada AI Agent  
### Production-Grade Multi-Modal 311-Style AI Intake System  
**Full-stack, AI-powered municipal issue reporting system with Salesforce case creation, Heroku inference routing, and real-time geocoded chat UI.**

---

## 🚀 Overview

**Custom Canada AI Agent** is a production-grade municipal intake platform that allows residents to report issues through natural language chat and photo uploads.  
The system intelligently routes different inputs to the correct inference provider, enriches data via geocoding, and creates **real Salesforce Cases** — all behind a polished web UI with a live map.

This is not a demo.  
This is a full enterprise-grade intake workflow built for speed, reliability, clarity, and safety.

---

## 🧠 Key Capabilities

### 1. Multi-Modal AI Routing
- Text → Heroku Managed Inference  
- Images → Claude (Anthropic)  

Routing is automatic — users don’t choose.

---

### 2. Salesforce Case Creation (REAL Cases)
After gathering:
- Issue type  
- Address or intersection  
- Description  
- Optional email for updates  

The agent immediately creates real Salesforce Cases via REST.

---

### 3. Advanced Geocoding
Supports:
- Exact addresses  
- Intersections  
- Ambiguous locations  

Includes retry logic and graceful fallback handling.

---

### 4. Hardened Security
- Input sanitization  
- Strict MIME validation for uploads  
- Secure headers (HSTS, XSS, no-sniff, frame protection)  
- Per-IP rate limiting  
- API quota enforcement  
- JWT and key-based Salesforce auth  

---

### 5. Polished Modern UI
- Map + chat split pane  
- Animated chat flow  
- Mobile-friendly scrolling  
- Inline photo uploads  

Feels like a modern consumer application.

---

## 🏗️ Architecture

Browser (Map + Chat UI)  
→ Flask API (Heroku)  
→ LLM Inference (Heroku / Claude)  
→ Geocoding (Nominatim)  
→ Salesforce Case Creation

---

## 📦 Project Structure

app/  
├── app.py  
├── keep_alive.py  
├── templates/index.html  
├── static/  
├── requirements.txt  
├── Procfile  
├── runtime.txt  

---

## 🚀 Deployment

Deployed on Heroku with:
- Web dyno (gunicorn)  
- Worker dyno  
- Config vars for secrets  
- GitHub or CLI deployment  

---

## 🏁 Summary

This project demonstrates:
- AI product engineering  
- Multi-modal inference routing  
- Secure enterprise integrations  
- Salesforce REST automation  
- Real-world public sector workflows  

---

## 👤 Author

Built by **Robert Smith** — AI Solutions Engineer focused on production-grade Agentforce and Heroku architectures.

