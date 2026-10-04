# Hi, I'm Bao 👋 🎵 My profile picture is drawn by my dear younger sister ❤️

Software Engineer based in Melbourne 🇦🇺 — I love to build systems that actually work in the real world.

Graduated as the **Highest Achieving Computer Science student at Swinburne**, and currently working across cloud-native systems, event-driven microservice-based architectures, and full-stack applications at SONIQ Digital.

I don’t really define myself by a specific tech stack — I care more about:
- breaking down complex problems
- designing clean, scalable systems
- debugging things until they *actually make sense*
- and...vibe-code

I also keep my problem-solving sharp with regular [LeetCode practice](https://github.com/giabaobui-nedy/LeetCode-Solutions).

---

## 🧠 What I enjoy working on

Right now, most of my time goes into:

- ⚙️ **Cloud-native systems** — AWS, microservices, event-driven design  
- 🔄 **System refactoring** — turning messy frontend codebase into structured architectures  
- 📊 **Real-world constraints** — cost optimisation, legacy systems, scalability & feasibility  
- 🧩 **End-to-end thinking** — from UI → backend → infrastructure → hardware devices

---

## 💼 What I’ve been building at work

### SONIQ Digital · Junior Software Engineer · Feb 2026 – now

I build the React frontend and the event-driven microservices behind a digital signage CMS. It is sold as SaaS and runs on AWS.

**☁️ Cloud & cost**
- Re-architected a transactional-outbox pipeline. A managed DMS → Kinesis → Lambda fan-out became a small poller on each service’s existing Fargate task, publishing straight to EventBridge.
- Built an event-driven scheduler (Lambda + EventBridge, as a CDK stack) that shuts non-production environments down overnight and at weekends.
- Found why an Aurora Serverless cluster sat at 5× idle capacity all day: a once-per-second query scanning a 1.7 GB table with no index. One composite index, rolled out across 4 services and 12 databases.

**🔄 Event-driven integrations**
- Wired Shopify webhooks into internal microservices (EventBridge + SQS), so buying a device starts a software trial on its own.
- Built a card-free Stripe trial flow, with deterministic idempotency keys so a customer is never created twice.
- Built a media pipeline that transcodes 4K uploads to Full HD for a legacy CMS.

**🧩 Frontend architecture**
- Led a TypeScript migration with one clear data path: DTO → mapper → domain → API → TanStack Query → hook.
- Generated TypeScript types from 4 microservices’ OpenAPI specs, so a backend contract change is a one-place edit.
- Merged two parallel component libraries into one hierarchy, and moved the codebase onto design tokens with a custom lint guard.
- Fixed an N+1 request pattern in the media library and rebuilt it as a Drive-style browser.

**🐛 Debugging things until they make sense**
- Fixed a production bug where recurring events disappeared. Schedules are set in Melbourne time but checked in UTC, so a local day spans two UTC days. Added boundary tests to CI.
- Caught a silently broken activation flow in development, by tracing CloudWatch logs across services to a renamed event topic.
- Found why 30 of 1,153 videos stayed stuck during a staging migration, by following the dead-letter queue, MediaConvert jobs and worker logs.

**🚀 Shipping features**
- A TypeScript + Playwright CLI that migrates customers off a legacy CMS, with dry runs, verification, rollback and 189 tests.
- Device grouping end to end (FastAPI + React), with bulk actions and a group filter.
- Priority-based schedule playback with fallback content, so screens never go blank.

### CSIRO · Software Engineering Intern → Casual Software Engineer · Mar 2024 – Jun 2025

I built a **lab automation system** for researchers. It turned a manual experimental workflow into a real-time, traceable platform.

- Led full-stack development across Vue/Nuxt, Python (Flask), PostgreSQL and InfluxDB.
- Designed a configuration-driven firmware layer (UI → server → firmware → Modbus), so new hardware setups need no major refactor.
- Added hardware locks and firmware-level caching. The system then ran for three months straight in a live lab.
- Streamed live telemetry into ECharts dashboards over WebSockets.
- Added Azure Entra ID SSO with role-based middleware, and shipped everything in Docker.
- Led the research and UI/UX design of a React Native app for copper refinery operators, after comparing Flutter, .NET MAUI and React Native.

---

## 📈 GitHub activity

<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://github-readme-stats.vercel.app/api?username=giabaobui-nedy&show_icons=true&include_all_commits=true&count_private=true&hide_border=true&bg_color=00000000&theme=dark" />
    <img height="170" alt="GitHub stats" src="https://github-readme-stats.vercel.app/api?username=giabaobui-nedy&show_icons=true&include_all_commits=true&count_private=true&hide_border=true&bg_color=00000000" />
  </picture>
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://github-readme-stats.vercel.app/api/top-langs/?username=giabaobui-nedy&layout=compact&langs_count=8&hide_border=true&bg_color=00000000&theme=dark" />
    <img height="170" alt="Top languages" src="https://github-readme-stats.vercel.app/api/top-langs/?username=giabaobui-nedy&layout=compact&langs_count=8&hide_border=true&bg_color=00000000" />
  </picture>
</p>

<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://streak-stats.demolab.com?user=giabaobui-nedy&theme=dark&hide_border=true&background=00000000" />
    <img alt="Contribution streak" src="https://streak-stats.demolab.com?user=giabaobui-nedy&hide_border=true&background=00000000" />
  </picture>
</p>

<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://github-profile-summary-cards.vercel.app/api/cards/profile-details?username=giabaobui-nedy&theme=github_dark" />
    <img width="100%" alt="Contribution summary" src="https://github-profile-summary-cards.vercel.app/api/cards/profile-details?username=giabaobui-nedy&theme=default" />
  </picture>
</p>

<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/giabaobui-nedy/giabaobui-nedy/output/github-contribution-grid-snake-dark.svg" />
    <img width="100%" alt="Contribution snake" src="https://raw.githubusercontent.com/giabaobui-nedy/giabaobui-nedy/output/github-contribution-grid-snake.svg" />
  </picture>
</p>

---

## 🛠️ Tech I’ve worked with

**Languages**  
TypeScript, Python, Java  

**Frontend**  
React, Next.js, Vue, Nuxt, React Native  

**Backend**  
Node.js, NestJS, FastAPI, Flask, GraphQL, REST  

**Cloud / DevOps**  
AWS (Lambda, EventBridge, ECS, ECR, ALB, SES, CDK), Docker, Terraform, CI/CD, GitHub Actions  

**Databases**  
PostgreSQL, MySQL, InfluxDB  

---

## 🎤 Outside of engineering

I sing. A lot.

Not trying to be perfect — just enjoy it.

👉 YouTube: [My Youtube](https://www.youtube.com/@giabaobui4283)

---

## 📫 Let’s connect

I enjoy conversations about:
- system design  
- architecture decisions  
- real-world engineering trade-offs  
- or just music  

🌐 Portfolio: [baobuild.dev](https://baobuild.dev)  
💼 LinkedIn: [My LinkedIn](https://www.linkedin.com/in/gia-bao-bui-227476227/)
