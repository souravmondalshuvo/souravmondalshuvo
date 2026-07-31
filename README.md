<div align="center">

<img width="100%" src="https://capsule-render.vercel.app/api?type=waving&color=0:0f172a,50:0f766e,100:14b8a6&height=200&section=header&text=Sourav%20Mondal%20Shuvo&fontSize=48&fontColor=ffffff&fontAlignY=38&desc=Full-Stack%20Developer%20%7C%20CSE%20%40%20BRAC%20University&descAlignY=58&descSize=16&animation=fadeIn"/>

<a href="https://souravmondalshuvo.com">
  <img src="https://img.shields.io/badge/souravmondalshuvo.com-14b8a6?style=for-the-badge&logo=googlechrome&logoColor=white" alt="Portfolio"/>
</a>
&nbsp;
<a href="https://linkedin.com/in/souravmondalshuvo">
  <img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"/>
</a>
&nbsp;
<img src="https://img.shields.io/badge/Open_to-Internships-2DD4BF?style=for-the-badge&labelColor=0d1117" alt="Open to internships"/>

</div>

---

## About

CSE undergraduate at **BRAC University** building production software solo, end-to-end.

My main project is **Shohoj** — an academic planning platform used by BRACU students, currently migrating from a 65-module vanilla JS codebase to React 19 + TypeScript, backed by Cloudflare Workers and covered by 600+ automated tests. I also build **FRIDAY**, a privacy-first desktop AI assistant, and maintain my portfolio site with a hand-written GLSL shader hero.

I care about shipping things people actually use, and treating side projects like production software — tests, security rules, and CI included.

---

## Shohoj — সহজ

> **Academic planning platform for BRAC University students. Built and maintained solo.**
> **[shohoj.souravmondalshuvo.com](https://shohoj.souravmondalshuvo.com)**

<div align="center">

<!-- Replace ci.yml with your actual workflow filename if different -->
<img src="https://img.shields.io/github/actions/workflow/status/souravmondalshuvo/Shohoj/ci.yml?branch=main&style=for-the-badge&label=CI&labelColor=0d1117&color=22c55e" alt="CI status"/>
&nbsp;
<img src="https://img.shields.io/badge/Automated_Tests-600%2B-22c55e?style=for-the-badge&labelColor=0d1117" alt="600+ tests"/>
&nbsp;
<img src="https://img.shields.io/badge/Courses-851-2DD4BF?style=for-the-badge&labelColor=0d1117" alt="851 courses"/>
&nbsp;
<img src="https://img.shields.io/badge/Departments-16-14b8a6?style=for-the-badge&labelColor=0d1117" alt="16 departments"/>

<br/><br/>

<!-- Add a screenshot or GIF at docs/shohoj-preview.png in this repo -->
<img width="85%" src="docs/shohoj-preview.png" alt="Shohoj interface preview"/>

</div>

### What it does

| Feature | Detail |
| --- | --- |
| **Course Catalog** | 851 courses across 16 departments with prerequisite chains |
| **CGPA Calculator** | BRACU grading with retake-aware recalculation |
| **Semester Planner** | Credit validation and prerequisite checking |
| **CGPA Playground** | Grade Changer and Reverse Solver for what-if planning |
| **Degree Tracker** | Requirement progress against the full degree plan |
| **Goal Simulator** | Works backward from a target CGPA to required grades |
| **Transcript Import** | PDF parsing with transcript-aware extraction |
| **Seat-Drop Alerts** | Cron-triggered email notifications when seats open |
| **Shohoj Assistant** | In-app AI for CGPA modeling, prerequisite checks, and seat lookups |
| **Scoped Auth** | Firebase Auth restricted to verified `@g.bracu.ac.bd` accounts |

### Engineering decisions I'm proud of

- **Architecture migration in flight** — Moving a 65-module vanilla JS codebase to React 19 + TypeScript + Vite; 15+ components rebuilt so far without taking production down.
- **Real backend, not just BaaS** — Cloudflare Workers with token-verified APIs and cron triggers, sitting in front of Firestore rather than trusting the client.
- **Security rules treated as code** — Hand-written Firestore rules with a 69-test emulator suite, so access control is verified rather than assumed.
- **AI with server-enforced isolation** — Shohoj Assistant runs on Claude Haiku through a Worker that verifies Firebase ID tokens, with read-only tools and per-user data isolation enforced server-side.
- **Testing at three layers** — 600+ automated tests spanning unit, Firestore rules, and Playwright end-to-end, all running in CI on every push.
- **Data pipeline** — A Python LLM pipeline turns unstructured community posts into structured course review seed data.
- **Hardening pass** — XSS input escaping, Content-Security-Policy headers, Subresource-Integrity hashes, and tightened Firebase access rules.

**Stack:** React 19 · TypeScript · Vite · Cloudflare Workers · Firebase Auth · Firestore · Python · Playwright · Vitest · pdf.js · jsPDF · GitHub Actions

---

## Other Projects

| Project | Description | Stack | Links |
|:---|:---|:---|:---|
| **FRIDAY** | Privacy-first desktop AI assistant. Cross-platform Electron app with a sci-fi HUD, local-first sensor processing, no persisted biometric data, and a Cloudflare Worker backend. | Electron · JavaScript · Cloudflare Workers | [Repo](https://github.com/souravmondalshuvo/FRIDAY) |
| **The Signal** | Personal portfolio site with a custom GLSL point-field hero rendered in Three.js. Dark-only design system, eight sections, built from scratch. | React 19 · TypeScript · Vite · Three.js · GLSL | [Live](https://souravmondalshuvo.com) |
| **Chillox** | Branded restaurant site with responsive sections and an interactive menu. | HTML · CSS · JavaScript | [Repo](https://github.com/souravmondalshuvo/Restaurant_Website) |

---

## Tech

<div align="center">

**Frontend**

![React](https://img.shields.io/badge/React-61DAFB?style=for-the-badge&logo=react&logoColor=black)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![Vite](https://img.shields.io/badge/Vite-646CFF?style=for-the-badge&logo=vite&logoColor=white)
![Three.js](https://img.shields.io/badge/Three.js-000000?style=for-the-badge&logo=three.js&logoColor=white)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)

**Backend & Infrastructure**

![Cloudflare Workers](https://img.shields.io/badge/Cloudflare_Workers-F38020?style=for-the-badge&logo=cloudflare&logoColor=white)
![Firebase](https://img.shields.io/badge/Firebase-FFCA28?style=for-the-badge&logo=firebase&logoColor=black)
![Node.js](https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=node.js&logoColor=white)
![Electron](https://img.shields.io/badge/Electron-47848F?style=for-the-badge&logo=electron&logoColor=white)

**Testing & Tooling**

![Playwright](https://img.shields.io/badge/Playwright-2EAD33?style=for-the-badge&logo=playwright&logoColor=white)
![Vitest](https://img.shields.io/badge/Vitest-6E9F18?style=for-the-badge&logo=vitest&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=for-the-badge&logo=github-actions&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white)

**Languages**

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Java](https://img.shields.io/badge/Java-007396?style=for-the-badge&logo=openjdk&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black)

</div>

---

## GitHub Stats

<div align="center">

<img height="180em" src="https://github-readme-stats.vercel.app/api?username=souravmondalshuvo&show_icons=true&theme=tokyonight&include_all_commits=true&count_private=true&hide_border=true&bg_color=0d1117&title_color=2dd4bf&icon_color=2dd4bf&text_color=c9d1d9"/>
<img height="180em" src="https://github-readme-stats.vercel.app/api/top-langs/?username=souravmondalshuvo&layout=compact&theme=tokyonight&hide_border=true&bg_color=0d1117&title_color=2dd4bf&text_color=c9d1d9"/>

</div>

---

## Currently

- Completing Shohoj's React 19 + TypeScript migration
- Building FRIDAY's Electron shell and Worker backend toward real functionality, not demo data
- Strengthening Data Structures & Algorithms in Java
- Preparing a technical write-up on Shohoj's architecture and testing approach

---

## Beyond Code

- Ran an IEEE Computer Society seminar as a volunteer at the BRACU chapter (IEEE CS Seminar Volunteer Certificate)
- Freelance developer and music producer, 2020–2023, delivering paid work for international clients
- I also write and release music — that side of things lives at [souravmondalshuvo.com](https://souravmondalshuvo.com)

---

<div align="center">

<sub>For internships, collaboration, or project discussions, <a href="https://linkedin.com/in/souravmondalshuvo">LinkedIn</a> is the fastest way to reach me.</sub>

</div>
