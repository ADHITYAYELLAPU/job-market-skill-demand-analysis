📊 Job Market Skill Demand Analysis (India)

🔍 Project Overview

A real-world job market analytics project that analyzes live job descriptions from Naukri to identify in-emand skills, role-wise expectations, and skill patterns across:

Business Analyst

Data Analyst

IT Recruiter / Talent Acquisition

The project focuses on market reality, not assumptions — helping candidates, recruiters, and HR teams understand what skills are actually being asked for in today’s job market.

🎯 Business Problem

Candidates often upskill without visibility into real job market demand, resulting in:

Skill mismatch

Lower interview shortlisting

Inefficient hiring decisions

At the same time, recruiters and HR teams need clearer visibility into:

Skill overlap across roles

Role-specific expectations

Market-driven skill priorities

This project addresses that gap using real job description data.

🧠 Objectives

Analyze real job descriptions from a leading job portal

Convert unstructured JD text into structured skill data

Identify common vs role-specific skills

Compare skill demand across analyst and recruiter roles

Generate decision-oriented insights, not just counts

📂 Data Collection

Source: Naukri.com

Method: Semi-manual collection (ethical, transparent, and realistic)

Dataset Size:

Business Analyst – 20 JDs

Data Analyst – 20 JDs

IT Recruiter – 20 JDs

Total: 60 job descriptions

Data Schema

Column	Description

role	Job role category

company	Hiring organization

location	Job location

jd_text	Full job description text

🛠️ Skill Extraction Methodology

Skill extraction was performed using an Excel-based, rule-driven approach, similar to how HR analysts and business analysts work when automation is limited.

This approach mirrors the foundational parsing logic used in ATS systems, without claiming to be an ATS product.

Skill Categories

Tools / Software – Excel, SQL, Power BI, ATS, MS Office

Technical / Functional Skills – Data Analysis, Reporting, Sourcing, Resume Screening

Business / Domain Skills – Stakeholder Management, Process Improvement

Soft Skills – Communication, Problem Solving, Team Collaboration

Technique Used

Keyword matching using Excel formulas (SEARCH, ISNUMBER)

Binary skill indicators (1 = skill present, 0 = not present)

Pivot tables for role-wise aggregation and comparison

📈 Analysis & Key Insights

The analysis reveals clear market patterns:

Excel is a baseline skill across all three roles

Data Analyst roles strongly emphasize SQL and analytical skills

Business Analyst roles balance reporting skills and stakeholder communication

IT Recruiter roles prioritize communication and sourcing over technical tools

Technical skills are role-specific, while soft skills show strong cross-role demand

These insights reflect real hiring expectations, not theoretical skill lists.

📌 Key Outcomes

Analyzed 60 real job descriptions from a live job portal

Transformed unstructured JD text into structured skill data

Identified high-demand skill clusters per role

Mapped common vs role-specific skills

Built a reusable job market skill demand framework

🧠 Skills & Keywords Highlighted

Job Market Analysis, Skill Demand Analysis, HR Analytics, Talent Analytics,
Business Analysis, Data Analysis, Resume Screening, Skill Gap Analysis,
Excel, Pivot Tables, Data Cleaning, Text Analysis, Requirement Analysis,
Stakeholder Management, Communication Skills

(Optimized for recruiter scanning and GitHub search visibility)

👥 Who This Analysis Helps

Job Seekers – Focus learning on market-relevant skills

Recruiters – Understand role-specific hiring expectations

HR & Talent Teams – Identify skill demand trends and gaps

🧩 Tools Used

Microsoft Excel

Excel formulas (SEARCH, ISNUMBER)

Pivot Tables

(No automated scraping, APIs, or resume parsing used)

📁 Repository Structure

├── HR_Domain_Project.xlsx

├── README.md

🚀 Why This Is a Real-World Case Study

Uses live job market data

Solves a practical hiring and career problem

Follows industry-realistic workflows

Focuses on decision-making insights

ATS-inspired logic without overclaiming
