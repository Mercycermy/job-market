# Ethiopian Job Market Analysis 🇪🇹

An intelligent platform designed to scrape, analyze, and visualize the Ethiopian job market landscape using modern AI and data visualization techniques.

## 🚀 Vision
To provide a data-driven understanding of employment trends in Ethiopia by aggregating data from popular job posting channels and leveraging Large Language Models (LLMs) for deep analysis.

## ✨ Key Features
- **Data Collection**: Automated scraping from Telegram channels and LinkedIn job posts.
- **AI Analysis**: Utilizing LLMs to categorize jobs, extract skills, and identify market demands.
- **Visual Analytics**: Interactive dashboards showing salary trends, skill gaps, and industry growth.
- **Ethiopic Support**: Specialized processing for Amharic and other local languages used in job posts.

## � Recommended Product Features (Prioritized)
1. **Job Posting CRUD**
	- Create, edit, delete, and list job opportunities.
	- Suggested fields: title, company, location, salary range, employment type, description, required skills.

2. **Search and Filter Experience**
	- Keyword search across titles, skills, and descriptions.
	- Filters for location, remote/on-site, full-time/part-time/contract, and salary band.

3. **Candidate Profiles and Resume Support**
	- Candidate profile pages with bio, skills, experience, and CV upload.
	- Structured profile data to improve matching and analytics.

4. **Application Workflow Tracking**
	- Application lifecycle states: `applied`, `reviewing`, `interview`, `rejected`, `hired`.
	- Candidate and recruiter views for transparent status updates.

5. **Authentication and Role-Based Access**
	- Roles: `candidate`, `recruiter`, `admin`.
	- Role-specific permissions for posting jobs, moderating content, and applying.

6. **Saved Jobs and Job Alerts**
	- Bookmark jobs and receive alerts for new relevant postings.
	- Retention-focused feature for return usage.

7. **Admin Moderation and Trust Tools**
	- Flag suspicious listings, approve/reject posts, and enforce quality standards.

## �🛠️ Proposed Tech Stack
- **Languages**: Python (Data Science & Scraping)
- **Data Collection**: Scrapy, Selenium, Telegram API (Telethon/Pyrogram)
- **AI/LLM**: LangChain, OpenAI GPT or Anthropic Claude, HuggingFace
- **Visualization**: Streamlit / Dash, Plotly / Recharts
- **Database**: PostgreSQL / MongoDB

## 🧭 Implementation Guide (MVP-First)

### 1) Define a small architecture contract
- **Input**: Raw job posts from Telegram/LinkedIn (mixed English + Amharic).
- **Processing**: Normalize fields, classify roles, extract skills and salary signals.
- **Output**: Searchable job records + trend dashboards + API-ready datasets.
- **Success Criteria**: Reliable ingestion, explainable analytics, usable dashboard.

### 2) Build in phased slices
1. **Ingestion Layer**
	- Implement channel/page connectors.
	- Store raw source payloads for traceability.
2. **Normalization Layer**
	- Clean duplicated posts, standardize dates/locations, parse salaries.
3. **AI Enrichment Layer**
	- Skill extraction, role categorization, and demand scoring.
4. **Serving Layer**
	- Expose cleaned/enriched data for dashboard and future APIs.
5. **Dashboard Layer**
	- Add trend charts, filters, and category-level summaries.

### 3) Core edge cases to handle early
- Duplicate job posts across channels.
- Missing salary/location fields.
- Mixed-language content (Amharic + English).
- Rate limiting and temporary scraping failures.
- Delayed or partially malformed posts.

### 4) Suggested initial milestones
- [ ] Milestone A: Raw scraping and persistence pipeline.
- [ ] Milestone B: Cleaning + schema standardization.
- [ ] Milestone C: LLM enrichment prompts and evaluation.
- [ ] Milestone D: Interactive dashboard with filters.
- [ ] Milestone E: Scheduled automation and monitoring.

## 📂 Project Structure (Planned)
```text
job-market/
├── data/               # Raw and processed datasets
├── scrapers/           # Telegram and LinkedIn scraping scripts
├── analysis/           # LLM processing and data cleaning
├── dashboard/          # Visualization interface
├── README.md           # Project overview
└── requirements.txt    # Dependencies
```

## 📝 Roadmap
- [ ] Phase 1: Setup Telegram/LinkedIn Scrapers
- [ ] Phase 2: Data Cleaning & LLM Integration
- [ ] Phase 3: Dashboard Development
- [ ] Phase 4: Deployment & Automation

## 🤝 Contribution Guide
1. Fork the repository and create a feature branch.
2. Keep changes scoped to one feature/fix per pull request.
3. Add short notes in PR description: motivation, approach, and screenshots (if UI).
4. Ensure code style and basic checks pass before requesting review.

## 📌 GitHub Push Workflow
If you update this file locally, use:

```powershell
git add README.md
git commit -m "docs: add feature recommendations and implementation guide"
git push origin master
```

If remote is not configured yet:

```powershell
git remote add origin https://github.com/Mercycermy/job-market.git
git push -u origin master
```

---
Created with ❤️ for the Ethiopian Tech Community.
