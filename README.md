<p align="center">
  <img src="assets/banner.svg" alt="Ghulam Mujtaba, AI Integration & Agent Engineer" width="100%">
</p>

<p align="center">
  <a href="https://github.com/MujtabaJ">
    <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=22&pause=900&color=6DA7EC&center=true&vCenter=true&width=720&lines=I+add+AI+to+real+products%2C+not+just+demos;RAG+assistants+that+cite+their+sources;AI+agents+%26+n8n+automations+that+save+hours;Document+%26+invoice+data+extraction;Flutter+apps+for+iOS+%26+Android" alt="What I build">
  </a>
</p>

<p align="center">
  <a href="https://www.upwork.com/freelancers/ghulammujtaba12"><img src="https://img.shields.io/badge/Hire_me-Upwork-14a800?style=for-the-badge&logo=upwork&logoColor=white" alt="Upwork"></a>
  <a href="https://www.hunarstack.com"><img src="https://img.shields.io/badge/Website-hunarstack.com-3987e5?style=for-the-badge&logo=googlechrome&logoColor=white" alt="Website"></a>
  <a href="https://x.com/ghulammujtaba"><img src="https://img.shields.io/badge/X-@ghulammujtaba-000000?style=for-the-badge&logo=x&logoColor=white" alt="X"></a>
  <img src="https://komarev.com/ghpvc/?username=MujtabaJ&style=for-the-badge&color=b48efa&label=Profile+views" alt="Profile views">
</p>

---

## 👋 About me

I'm a software engineer from **Karachi, Pakistan** with **8+ years** of shipping mobile apps for clients worldwide. Today I help SaaS companies and growing businesses **put AI to work inside the products they already have**:

- 🤖 **AI chatbots & RAG assistants** that answer from *your* documents, cite sources and refuse to guess
- 🧠 **AI agents & automation** (OpenAI, Claude, n8n) that take repetitive work off your team
- 📄 **Document & invoice extraction** with validation and a human review queue
- 📱 **AI-powered Flutter apps** for iOS & Android, plus RevenueCat subscriptions
- 🛠️ **Fixing & finishing apps built with Lovable / Bolt** so they're ready for real users

<p align="center"><img src="assets/stack.svg" alt="Tech stack" width="100%"></p>

---

## 🚀 Featured AI projects

### 📚 [Knowledge Base Assistant (RAG)](https://github.com/MujtabaJ/kb-assistant)
An assistant that answers **only from a company's own documents**: every answer has citations, it refuses when the documents don't cover the question, and it filters prompt-injection text before the model sees it. Multi-tenant API, tests, an evaluation gate in CI, structured logs and cost tracking.

<p align="center"><img src="assets/mockup-kb-assistant.svg" alt="Knowledge Base Assistant UI preview" width="80%"></p>

```mermaid
flowchart LR
    U([User question]) --> API[FastAPI · tenant auth]
    API --> R[Retriever<br/>embeddings + pgvector]
    D[(Company docs)] -->|chunk · embed · clean injections| R
    R -->|score ≥ threshold| L[LLM<br/>answer only from sources]
    R -->|score too low| X[Refuse politely]
    L --> G{Citations match<br/>real sources?}
    G -->|yes| A([Answer + citations])
    G -->|no| F([Flag: not grounded])
    L -.-> O[(Logs · cost · evals in CI)]
```

### 🧾 [Invoice Extractor](https://github.com/MujtabaJ/invoice-extractor)
OCR + LLM extraction of invoice fields with **validation rules and confidence scores**. Clean invoices are approved automatically; anything uncertain goes to a human review queue.

<p align="center"><img src="assets/mockup-invoice-review.svg" alt="Invoice review queue UI preview" width="80%"></p>

```mermaid
flowchart LR
    P[PDF / photo] --> O[OCR]
    O --> E[LLM field extraction<br/>structured JSON]
    E --> V{Validation<br/>totals · dates · vendor}
    V -->|high confidence| OK([Auto-approve → export])
    V -->|low confidence| Q[Human review queue]
    Q -->|fix & approve| OK
```

---

## 📱 Mobile apps

<p align="center"><img src="assets/mockup-mobile-apps.svg" alt="Mobile app UI concepts" width="100%"></p>

| Project | What it is | Stack |
|---|---|---|
| [Student Guide](https://github.com/MujtabaJ/studentguide) | Student companion app | Flutter · Dart |
| [AA Maka](https://github.com/MujtabaJ/aamaka) | Music app | TypeScript |
| [HunarStack](https://github.com/MujtabaJ/hunarstack) | Website & product hub | JavaScript |
| Business Card Reader | Scans business cards into contacts ([privacy pages](https://github.com/MujtabaJ/business-card-reader-legal)) | Android |
| [Africa](https://github.com/MujtabaJ/Africa) · [Fruits](https://github.com/MujtabaJ/Fruits) | SwiftUI showcase apps | Swift · SwiftUI |

---

## 🛠️ How I work

<p align="center"><img src="assets/delivery-flow.svg" alt="Delivery process" width="100%"></p>

---

## 📊 By the numbers

<p align="center">
  <img src="assets/timeline.svg" alt="Career path" width="49%">
  <img src="assets/languages.svg" alt="Public repos by primary language" width="49%">
</p>

<p align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=MujtabaJ&show_icons=true&theme=github_dark&hide_border=true&bg_color=0d1117&title_color=6da7ec&icon_color=b48efa&include_all_commits=true&count_private=true" alt="GitHub stats" height="170">
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=MujtabaJ&layout=compact&theme=github_dark&hide_border=true&bg_color=0d1117&title_color=6da7ec" alt="Top languages" height="170">
</p>

<p align="center">
  <img src="https://streak-stats.demolab.com?user=MujtabaJ&theme=github-dark-blue&hide_border=true&background=0d1117&ring=b48efa&fire=e87ba4&currStreakLabel=6da7ec" alt="Contribution streak">
</p>

<p align="center">
  <img src="https://github-readme-activity-graph.vercel.app/graph?username=MujtabaJ&bg_color=0d1117&color=c9d1d9&line=6da7ec&point=e87ba4&area=true&area_color=3987e5&hide_border=true" alt="Contribution activity graph" width="100%">
</p>

---

## 🤝 Let's work together

Have an AI idea, a half-finished app, or a manual process that eats your team's time? I offer a **free 30-minute call** to scope it, then a fixed-price audit or pilot so you see results before committing to a bigger build.

<p align="center">
  <a href="https://www.upwork.com/freelancers/ghulammujtaba12"><img src="https://img.shields.io/badge/Start_a_project_on_Upwork-14a800?style=for-the-badge&logo=upwork&logoColor=white" alt="Start a project on Upwork"></a>
</p>

<p align="center"><sub>Mockups above illustrate my demo projects with sample data · Stats update automatically</sub></p>
