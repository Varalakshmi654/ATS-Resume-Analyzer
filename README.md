# 📄 ATS Resume Analyzer


**A browser-based tool that helps job seekers optimize their resumes by comparing them against role-specific skill requirements — and scoring them like a real ATS.**

[🚀 Live Demo](#) · [🐛 Report Bug](../../issues) · [✨ Request Feature](../../issues)

</div>

---

## 📑 Table of Contents

- [📌 Project Overview](#-project-overview)
- [✨ Features](#-features)
- [🛠️ Technologies Used](#️-technologies-used)
- [📁 Project Structure](#-project-structure)
- [⚙️ Installation & Usage](#️-installation--usage)
- [📊 How the ATS Score is Calculated](#-how-the-ats-score-is-calculated)
- [📸 Screenshots](#-screenshots)
- [🔮 Future Enhancements](#-future-enhancements)
- [🎓 Learning Outcomes](#-learning-outcomes)
- [👤 Author](#-author)

---

## 📌 Project Overview

In today's competitive job market, most companies use **Applicant Tracking Systems (ATS)** to automatically filter resumes before a human recruiter ever sees them. Resumes that don't include the right keywords get rejected — even if the candidate is well-qualified.

**ATS Resume Analyzer** is a lightweight, client-side web application that empowers job seekers to:

- Understand what skills each job role demands
- Instantly check how well their resume matches those requirements
- Identify the exact keywords they're missing
- Improve their resume before submitting applications

> 💡 Built entirely with HTML, CSS, and Vanilla JavaScript — no frameworks, no backend, no data sent anywhere. Your resume stays private on your device.

---

## ✨ Features

| Feature | Description |
|---|---|
| 🎯 **Role Selection** | Choose from multiple job roles (Data Scientist, Data Analyst, Web Developer, etc.) |
| 📋 **Skill Display** | Instantly view the required skills for the selected role |
| 📝 **Resume Input** | Paste your resume text directly into the analyzer |
| 🔍 **Keyword Matching** | Compares your resume content against required skills using smart keyword detection |
| 📊 **ATS Score** | Calculates a percentage-based ATS compatibility score |
| ✅ **Matched Skills** | Highlights which required skills your resume already contains |
| ❌ **Missing Skills** | Clearly shows which skills are absent so you know exactly what to add |
| 📱 **Responsive Design** | Works seamlessly on desktops, tablets, and mobile devices |
| ⚡ **Instant Results** | All processing happens in-browser — no loading, no waiting |

---

## 🛠️ Technologies Used

| Technology | Purpose |
|---|---|
| **HTML5** | Page structure and semantic markup |
| **CSS3** | Styling, layout, animations, and responsiveness |
| **Vanilla JavaScript (ES6+)** | Core logic — keyword matching, score calculation, DOM manipulation |
| **GitHub Pages** | Free static site hosting for the live demo |

> No external libraries, no npm packages, no build tools. This project proves you can build something genuinely useful with just the fundamentals.

---

## 📁 Project Structure

```
ats-resume-analyzer/
│
├── index.html          # Main HTML file — app structure and layout
├── style.css           # All styling, responsive breakpoints, animations
├── script.js           # Core logic: roles, skills data, matching algorithm, scoring
├── README.md           # Project documentation (you are here)
└── assets/             # (Optional) Screenshots, icons, or images
    └── screenshots/
        ├── home.png
        ├── results.png
        └── mobile.png
```

---

-

### 📝 How to Use the App

1. **Select a Job Role** from the dropdown menu (e.g., *Data Scientist*)
2. **Review the required skills** displayed for that role
3. **Paste your resume text** into the text area
4. **Click "Analyze Resume"** to run the ATS check
5. **View your ATS Score**, matched skills ✅, and missing skills ❌
6. **Update your resume** to include missing keywords and re-analyze

---

## 📊 How the ATS Score is Calculated

The ATS score is calculated using a straightforward keyword-matching algorithm:

```
ATS Score (%) = (Number of Matched Skills ÷ Total Required Skills) × 100
```

### Step-by-Step Breakdown

```
1. Load skill list  →  Each job role has a predefined set of required keywords/skills

2. Normalize text   →  Both the resume text and skill keywords are converted to 
                       lowercase to ensure case-insensitive matching

3. Keyword search   →  Each required skill is checked against the full resume text
                       using JavaScript's .includes() or regex matching

4. Score calculation →  Matched skills ÷ Total skills × 100 = ATS Score %

5. Categorize results → Skills are sorted into "Matched" and "Missing" lists
```

### Score Interpretation

| Score Range | Interpretation |
|---|---|
| 🟢 **80% – 100%** | Excellent match — your resume is well-optimized |
| 🟡 **60% – 79%** | Good match — a few more keywords would help |
| 🟠 **40% – 59%** | Moderate — significant gaps to address |
| 🔴 **0% – 39%** | Low match — resume needs major keyword optimization |

> **Note:** This tool uses keyword frequency matching, which mirrors how many real-world ATS platforms work. Adding missing keywords naturally into your resume (in context, not just listed) is always the best strategy.

---

## 📸 Screenshots

> 📌 *Replace the placeholder text below with actual screenshots after deployment.*

### 🏠 Home Screen — Role Selection
```
[ Screenshot: Home page with job role dropdown and required skills panel ]
```
![Home Screen](assets/screenshots/home.png)

---

### 📊 Results View — ATS Score & Skill Breakdown
```
[ Screenshot: Score percentage, matched skills in green, missing skills in red ]
```
![Results View](assets/screenshots/results.png)

---

### 📱 Mobile View — Responsive Layout
```
[ Screenshot: App displayed on a mobile screen ]
```
![Mobile View](assets/screenshots/mobile.png)

---

## 🔮 Future Enhancements

Here's what's planned for upcoming versions:

- [ ] 🤖 **AI-Powered Analysis** — Integrate an LLM API to give contextual resume feedback, not just keyword matching
- [ ] 📂 **PDF Upload Support** — Allow users to upload a `.pdf` resume instead of pasting text
- [ ] 🗂️ **More Job Roles** — Expand the skill database to cover 20+ roles across tech, finance, and healthcare
- [ ] 📈 **Score History** — Let users save and compare multiple analysis sessions
- [ ] 💡 **Rewrite Suggestions** — Suggest how to reword bullet points to include missing keywords naturally
- [ ] 🌙 **Dark Mode** — Add a toggle for light/dark themes
- [ ] 🌐 **Multi-language Support** — Support resume analysis in languages beyond English
- [ ] 📤 **Export Report** — Download a PDF summary of the ATS analysis

---

## 🎓 Learning Outcomes

Building this project developed and reinforced the following skills:

**Technical Skills**
- Writing clean, semantic **HTML5** structure
- Building responsive layouts with **CSS Flexbox/Grid** and media queries
- Implementing **DOM manipulation** and event handling with Vanilla JavaScript
- Designing and applying a **text-processing algorithm** (keyword extraction & matching)
- Structuring a **data-driven application** — managing role-to-skills mappings in JavaScript
- Using **string methods and regex** for case-insensitive text comparison

**Soft & Portfolio Skills**
- Translating a real-world problem (ATS filtering) into a working software solution
- Designing a tool from scratch with **user experience** in mind
- Writing professional **technical documentation** (this README)
- Deploying a project to **GitHub Pages** for public access

---

## 👤 Author

<div align="center">

**Eetha Vara Lakshmi**
*Data Science Student | Aspiring ML Engineer*


## 🌟 Show Your Support

If this project helped you or gave you ideas, please consider:

- ⭐ **Starring this repository** — it helps others find the project
- 🍴 **Forking it** to build your own version
- 🐛 **Opening an issue** if you find a bug or have a feature request
- 📢 **Sharing it** with fellow students or job seekers who might benefit

---

<div align="center">

*Built with ❤️ and a lot of ☕ by [Eathe Vara Lakshmi](https://github.com/Varalakshmi654)*

*⭐ If you found this useful, a star means a lot!*

</div>
