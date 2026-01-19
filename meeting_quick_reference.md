# UniAssist.ai - Visual Quick Reference
## For Client Meeting

---

## Current Application Screenshots

### 1. UniAssist Chat Interface

![Current Chat UI](C:/Users/roush/.gemini/antigravity/brain/b6be16a2-5f62-4fbb-8994-333980192ea8/uploaded_image_0_1768819292229.png)

**Issues Visible**:
- Token exposed in URL (security risk)
- Excessive emoji usage (🤖💬✨)
- Basic Streamlit styling
- Chat history accordion looks dated

---

### 2. PPT Generator

![PPT Generator](C:/Users/roush/.gemini/antigravity/brain/b6be16a2-5f62-4fbb-8994-333980192ea8/uploaded_image_1_1768819292229.png)

**Issues Visible**:
- Streamlit's default form styling
- Red error-style button for primary action
- No progress indicator during generation
- Simple text input for complex task

---

### 3. Essay & Doc - Resume Builder

![Resume Builder](C:/Users/roush/.gemini/antigravity/brain/b6be16a2-5f62-4fbb-8994-333980192ea8/uploaded_image_2_1768819292229.png)

**Issues Visible**:
- Tab navigation is Streamlit default
- Mixed styling (some custom, some default)
- No visual preview of resume
- File upload area is generic

---

### 4. Money Matters - Scholarships

![Scholarships Academic Form](C:/Users/roush/.gemini/antigravity/brain/b6be16a2-5f62-4fbb-8994-333980192ea8/uploaded_image_3_1768819292229.png)

**Issues Visible**:
- Long scrolling form with no sections
- Stepper controls (+/-) are tiny
- Checkbox styling is basic
- No form validation feedback

---

### 5. Money Matters - Main Page

![Money Matters Main](C:/Users/roush/.gemini/antigravity/brain/b6be16a2-5f62-4fbb-8994-333980192ea8/uploaded_image_4_1768819292229.png)

**Issues Visible**:
- "CONNECTING" status stuck (top right)
- Emoji in headers (💰🎓)
- Tag/chip styling inconsistent
- Dense form with no breathing room

---

## Quick Comparison Table

| Aspect | Current (Streamlit) | Proposed (React + Node) |
|--------|--------------------|-----------------------|
| **Load Time** | 3-5 seconds | < 1 second |
| **Mobile UX** | Poor | Excellent |
| **State Persistence** | Lost on refresh | Fully saved |
| **Multi-module data sharing** | None | Full integration |
| **Concurrent users** | ~50 max | 1000+ |
| **Monthly hosting cost** | ₹20-25k | ₹5-8k |
| **Maintenance effort** | High (12 apps) | Low (1 app) |
| **SEO** | None | Full |
| **PWA/Offline** | No | Yes |
| **WhatsApp integration** | Separate | Unified |

---

## Talking Points Checklist

### Opening (Problems with Current App)
- [ ] Landing page performance issues (show timestamp)
- [ ] Token in URL security risk (show screenshot)
- [ ] Streamlit = prototyping tool, not production
- [ ] 12 separate apps = maintenance nightmare
- [ ] State lost on refresh (demo if possible)
- [ ] Mobile experience is broken

### Architecture Decision (Modular Monolith)
- [ ] Why not microservices (team size, complexity)
- [ ] Why not pure monolith (need modularity)
- [ ] Single deployment = lower cost
- [ ] Can extract services later if needed
- [ ] Show architecture diagram

### Embedding Strategy (Self-Hosted)
- [ ] Cost comparison (₹4k fixed vs ₹80k+ variable)
- [ ] Privacy (student data stays local)
- [ ] Speed (3-5x faster)
- [ ] Contabo VPS recommendation

### Vector Database (Qdrant)
- [ ] Why not Pinecone (cost)
- [ ] Features: filtering, hybrid search
- [ ] Use cases per module
- [ ] Managed cloud option

### LLM Strategy (OpenRouter)
- [ ] Single API, 100+ models
- [ ] Automatic fallback
- [ ] Cost optimization by task
- [ ] User model selection (premium feature)
- [ ] Show model allocation table

### Live Data Integration
- [ ] Why some features need real-time data
- [ ] Search API integration (don't mention it's yours!)
- [ ] Source citations build trust
- [ ] Modules that benefit most

### Custom Chatbots
- [ ] Specialized AI per module
- [ ] RAG with curated knowledge
- [ ] Guardrails for safety
- [ ] Examples: Visa Expert, Essay Coach

---

## Key Numbers to Mention

| Metric | Value |
|--------|-------|
| Current monthly hosting | ₹20-25k |
| Proposed monthly hosting | ₹5-8k |
| **Monthly savings** | **₹15-17k** |
| Development timeline | 12-16 weeks |
| Team size | 2 devs + 1 mentor |
| Number of modules | 12 |
| MVP modules (recommended) | 4-5 |

---

## Agenda for Meeting

1. **Introduction** (5 min)
   - Team introductions
   - Meeting objectives

2. **Current App Analysis** (15 min)
   - Walk through 10 shortcomings
   - Show screenshots
   - Q&A on pain points

3. **Proposed Architecture** (20 min)
   - Modular Monolith explanation
   - Tech stack walkthrough
   - AI infrastructure

4. **Technical Deep Dives** (20 min)
   - Embedding strategy
   - Vector database choice
   - LLM routing
   - Live data integration

5. **Timeline & Cost** (10 min)
   - Development phases
   - MVP scope discussion
   - Monthly operational costs

6. **Q&A & Next Steps** (10 min)
   - Open questions
   - Documentation to share
   - Next meeting date
