# 📊 Job Market Skill Demand Analysis — India (Naukri.com)
### Real-World HR Analytics | 60 Live JDs · 3 Roles · ATS-Inspired Skill Extraction · Excel · Pivot Tables

> **The most meta analytics project in this portfolio** — using data analyst skills to analyze what skills data analyst jobs actually demand. Built on 60 real, live job descriptions scraped from Naukri.com — zero assumptions, 100% market reality.

---

## 📌 Project at a Glance

| Metric | Value |
|---|---|
| 📋 Job Descriptions Analyzed | **60 real JDs** from Naukri.com — India's largest job portal |
| 🎯 Roles Covered | **3 roles** — Business Analyst · Data Analyst · IT Recruiter / Talent Acquisition |
| 📐 JDs per Role | **20 per role** — balanced sample ensuring fair cross-role comparison |
| 🧠 Skill Extraction Method | **ATS-inspired keyword matching** — SEARCH + ISNUMBER + binary skill flags |
| 📊 Skill Categories Mapped | **4 categories** — Tools · Technical/Functional · Business/Domain · Soft Skills |
| 🔁 Framework Type | **Reusable** — structured to apply on any new batch of JDs with no rework |
| 🛠️ Tools | **Microsoft Excel** — Formulas · Pivot Tables · Binary Skill Matrix |

---

## 🎯 The Problem This Solves

Every year, thousands of candidates upskill blindly — completing courses on tools that real job postings barely mention, while missing the skills that appear in 80% of JDs they apply for.

**This project answers what no course syllabus tells you:**

1. What skills appear in the **most job descriptions** — by role?
2. Which skills are **truly role-specific** vs. which are universal baselines?
3. Is **Excel really that important**, or is SQL taking over?
4. What does an IT Recruiter JD ask for that a Data Analyst JD never does?
5. Where is the **skill overlap** between roles — and what does it mean for career switchers?

---

## 🔍 Key Insights — What 60 Real JDs Reveal

### 📌 The Universal Baseline — Skills That Appear Across All 3 Roles
- **Excel** is the single most cross-functional skill — demanded in Business Analyst, Data Analyst, AND IT Recruiter JDs, making it the lowest common denominator of employability in India's analytics and HR job market
- **Communication skills** and **stakeholder management** appear as soft skill requirements across all 3 roles, confirming that no analytics role is purely technical in the Indian market context
- **MS Office proficiency** is a non-negotiable baseline — even in technically demanding Data Analyst JDs

### 📊 Data Analyst (20 JDs) — Technical Depth Required
- **SQL** emerged as the dominant technical differentiator — appearing in the majority of Data Analyst JDs while being nearly absent in IT Recruiter JDs
- **Reporting and dashboarding tools** (Power BI, Tableau, similar) appeared as explicit requirements, not preferences
- Data Analyst JDs had the **highest skill density** — more unique skills requested per JD compared to the other two roles, reflecting the multi-tool nature of the role
- **Python** presence was noted — signalling that even in India's mid-market, scripting expectations are entering analyst JDs

### 💼 Business Analyst (20 JDs) — The Hybrid Middle Ground
- Business Analyst JDs showed the **broadest skill spread** — balancing technical tools (Excel, SQL, reporting) with domain and soft skills (process improvement, requirement gathering, stakeholder management)
- **Requirement documentation and analysis** was the most role-specific functional skill — barely appearing in Data Analyst or IT Recruiter JDs
- Findings confirm that Business Analysts are hired as **connectors between data and decision-makers** — technical enough to pull data, communicative enough to explain it

### 🤝 IT Recruiter / Talent Acquisition (20 JDs) — People-First Skill Profile
- **ATS (Applicant Tracking System) proficiency** was the single most role-exclusive technical skill — appearing frequently in IT Recruiter JDs and essentially nowhere else
- **Sourcing skills** (Boolean search, job portal navigation, talent mapping) dominated the functional requirements
- **Communication and interpersonal skills** carried significantly more JD weight in IT Recruiter roles than in either analyst role — confirming a fundamentally different hiring profile
- Technical tool demand was **lowest among the 3 roles** — the majority of required skills were people-process oriented, not software oriented

### 🔁 Cross-Role Skill Overlap — What This Means for Career Switchers
- Skills shared across all 3 roles: Excel, Communication, MS Office, Basic Reporting
- Skills shared between BA & DA roles: SQL (partial), Data Analysis, Reporting Tools
- Skills exclusive to Recruiter: ATS, Sourcing, Resume Screening, Talent Mapping
- **Career switch insight:** A Data Analyst moving toward Business Analysis needs to add requirement documentation and stakeholder skills — not new technical tools. The gap is softer than candidates assume.

---

## 🛠️ Skill Extraction Methodology — ATS-Inspired Logic in Excel

This project replicates the **foundational keyword-parsing logic** that powers commercial ATS systems — built entirely in Excel, without any API, scraping tool, or code.

```
📦 Skill Extraction Pipeline
│
├── STEP 1 → Data Collection
│            60 JDs manually collected from Naukri.com
│            Fields captured: Role | Company | Location | JD Text
│
├── STEP 2 → Skill Dictionary Design
│            4 categories defined:
│            ├── Tools / Software      (Excel, SQL, Power BI, ATS, MS Office)
│            ├── Technical / Functional (Data Analysis, Reporting, Sourcing)
│            ├── Business / Domain     (Stakeholder Management, Process Improvement)
│            └── Soft Skills           (Communication, Problem Solving, Collaboration)
│
├── STEP 3 → Binary Skill Flag Matrix
│            For each skill × each JD:
│            =IF(ISNUMBER(SEARCH("skill_keyword", jd_text_cell)), 1, 0)
│            → 1 = skill mentioned in JD
│            → 0 = skill not mentioned
│
├── STEP 4 → Role-Wise Aggregation
│            Pivot Tables aggregate skill frequency per role
│            → "How many of the 20 Data Analyst JDs mention SQL?"
│            → "How many of the 20 BA JDs mention Power BI?"
│
└── STEP 5 → Cross-Role Comparison
             Skill presence rate (%) calculated per role
             Common vs. role-specific skills mapped
             Skill overlap identified for career path analysis
```

**Why this approach matters:** The SEARCH + ISNUMBER + binary flag method is the same conceptual logic used in commercial ATS keyword scoring — doing this in Excel demonstrates understanding of how automated screening actually works, not just that it exists.

---

## 📊 Dashboard & Analysis Previews

### HR Domain — Skill Demand Overview
![HR Domain Analysis 1](HR%20Domain%201.png)
![HR Domain Analysis 2](HR%20Domain%202.png)
![HR Domain Analysis 3](HR%20Domain%203.png)

### Raw Data & Extraction Workbook
![Extraction Workbook View 1](Screenshot%202026-02-10%20020234.png)
![Extraction Workbook View 2](Screenshot%202026-02-10%20020247.png)

---

## 👥 Who This Directly Helps

| Audience | What They Get From This |
|---|---|
| 🎓 **Job Seekers** | Stop guessing — know exactly which skills appear in the most JDs for your target role before you spend time upskilling |
| 📋 **Recruiters & TA Teams** | Understand which skills truly differentiate candidates vs. which are baseline noise across all JDs |
| 🏢 **HR & L&D Teams** | Identify skill gap patterns across roles — inform training investment with market data, not assumptions |
| 🔄 **Career Switchers** | Map skill overlap between roles to identify the shortest upskilling path from current role to target role |

---

## 💼 Skills Demonstrated (Recruiter Checklist ✅)

- ✅ **Real Data Collection** — 60 live JDs from Naukri.com; market reality, not synthetic datasets
- ✅ **Unstructured → Structured Transformation** — Free-form JD text converted into a clean binary skill matrix
- ✅ **ATS Logic Understanding** — Keyword extraction methodology mirrors how applicant tracking systems score candidates
- ✅ **Multi-Role Comparative Analysis** — 3 roles analyzed side-by-side with a controlled 20 JD sample per role
- ✅ **Skill Taxonomy Design** — 4-category skill classification framework built from scratch
- ✅ **Advanced Excel Execution** — SEARCH, ISNUMBER, nested IF logic, and Pivot Tables for aggregation
- ✅ **Decision-Oriented Insights** — Output framed as actionable guidance for candidates, recruiters, and L&D teams
- ✅ **Reusable Framework** — Methodology designed to scale to new roles, new JD batches, or new geographies

---

## 🧩 Tools & Techniques

![Excel](https://img.shields.io/badge/Excel-217346?style=for-the-badge&logo=microsoft-excel&logoColor=white)

| Tool / Technique | Usage |
|---|---|
| **Microsoft Excel** | Full analysis environment — data storage, skill extraction, aggregation, comparison |
| **SEARCH + ISNUMBER** | Keyword presence detection across JD text — ATS-inspired logic |
| **Binary Skill Flag Matrix** | 1/0 encoding of skill presence per JD — enables frequency analysis |
| **Pivot Tables** | Role-wise skill aggregation, cross-role comparison, percentage calculation |
| **Skill Taxonomy Design** | 4-category framework: Tools · Technical · Business · Soft Skills |

> **Design Note:** No automated scraping, APIs, or ML libraries were used. This is intentional — the project demonstrates that rigorous, decision-quality analytics is achievable with tools available in any workplace, not just in Python notebooks.

---

## 📁 Repository Structure

```
📂 job-market-skill-demand-analysis/
│
├── 📊 HR Domain Project.xlsx         # Full analysis workbook — data, extraction, pivots
│
├── 🖼️ HR Domain 1.png                # Skill demand overview — cross-role view
├── 🖼️ HR Domain 2.png                # Role-wise skill frequency breakdown
├── 🖼️ HR Domain 3.png                # Common vs. role-specific skill mapping
├── 🖼️ Screenshot 2026-02-10 020234.png  # Raw extraction workbook view
├── 🖼️ Screenshot 2026-02-10 020247.png  # Binary skill matrix view
│
└── 📄 README.md                      # This file
```

---

## 👤 About the Author

**Adhitya Yellapu** — Data & Business Operations Analyst

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/adhitya-yellapu)
[![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/ADHITYAYELLAPU)
[![Portfolio](https://img.shields.io/badge/Portfolio-FF5722?style=for-the-badge&logo=google-chrome&logoColor=white)](https://adhityayellapu.github.io/Portfolio/)

---

*Self-initiated project demonstrating HR analytics and job market intelligence — the kind of structured skill demand analysis used by talent strategy teams at top recruitment firms, L&D consultancies, and workforce planning departments across India's analytics industry.*
